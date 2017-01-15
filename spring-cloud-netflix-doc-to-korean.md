Spring Cloud Netflix
===========

# 원본
http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html

**1.3.0.BUILD-SNAPSHOT**


이 프로젝트는 자동 환경 설정과 스프링 환경 및 기타 스프링 프로그래밍 모델 관용구에 대한 바인딩을 통해 스프링 부트 애플리케이션을 위한 Netflix OSS 통합을 제공합니다.
몇 가지 간단한 주석을 사용하면 애플리케이션 내부의 공통 패턴을 신속하게 활성화 및 구성하고 전투 테스트를 거친 Netflix 구성 요소로 
대규모 분산 시스템을 구축 할 수 있습니다.
제공되는 패턴에는 서비스 발견 (Eureka), 회로 차단기 (Hystrix), 지능형 라우팅 (Zuul) 및 클라이언트 측로드 균형 조정 (리본)이 포함됩니다.


## 서비스 발견 : 유레카 클라이언트

서비스 검색은 마이크로 서비스 기반 아키텍처의 핵심 교리 중 하나입니다.
각 클라이언트 또는 일부 형식의 컨벤션 구성을 손으로 처리하는 것은 매우 어려울 수 있으며 매우 취성이 있습니다.
유레카는 Netflix 서비스 검색 서버 및 클라이언트입니다.서버는 등록 된 서비스에 대한 상태를 다른 서버로 복제하여 각 서버가 고 가용성으로 구성 및 배치 할 수 있습니다.




### 유레카 클라이언트를 포함시키는 방법



프로젝트에서 유레카 클라이언트를 포함하는 그룹과 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-eureka`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.







### 유레카 등록



클라이언트가 유레카에 등록하면 호스트 및 포트, 상태 표시기 URL, 홈 페이지 등과 같은 메타 데이터를 제공합니다. 유레카는 서비스에 속한 각 인스턴스에서 하트 비트 메시지를받습니다.하트 비트가 구성 가능한 시간표에 실패하면 보통 인스턴스는 레지스트리에서 제거됩니다.





예시 유레카 클라이언트 :







    @Configuration
    @ComponentScan
    @EnableAutoConfiguration
    @EnableEurekaClient
    @RestController
    public class Application {

        @RequestMapping("/")
        public String home() {
            return "Hello world";
        }

        public static void main(String[] args) {
            new SpringApplicationBuilder(Application.class).web(true).run(args);
        }

    }







(즉, 완전히 정상적인 스프링 부트 응용 프로그램).우리가 사용하는이 예에서`@EnableEurekaClient`명시 적으로 만 유레카 사용할 수와 함께 당신은 또한 사용할 수 있습니다`@EnableDiscoveryClient`.Eureka 서버를 찾으려면 구성이 필요합니다.예:





application.yml



<pre>유레카:고객:serviceUrl :defaultZone : http : // localhost : 8761 / eureka /</pre>







여기서 "defaultZone"은 기본 설정을 나타내지 않는 클라이언트 (즉 유용한 기본값)에 대한 서비스 URL을 제공하는 마법 문자열 대체 값입니다.





기본 프로그램 이름 (서비스 ID)는 가상 호스트와 비보안 포트는 상기에서 촬영`Environment`하고,`${spring.application.name}`,`${spring.application.name}`및`${server.port}`는 각각.





`@EnableEurekaClient`응용 프로그램을 유레카 "인스턴스"(즉, 자체 등록)와 "클라이언트"(즉, 다른 서비스를 찾기 위해 레지스트리에 쿼리 할 수 ​​있음)로 만듭니다.인스턴스 동작에 의해 구동되는`eureka.instance.*`구성 키,하지만 당신은 응용 프로그램이이 있는지 확인하는 경우 기본값은 잘 될 것입니다`spring.application.name`(이 유레카 서비스 ID, 또는 VIP에 대한 기본값입니다).





참조[EurekaInstanceConfigBean](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-eureka-client/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java)및[EurekaClientConfigBean를](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-eureka-client/src/main/java/org/springframework/cloud/netflix/eureka/EurekaClientConfigBean.java)구성 가능한 옵션의 자세한 내용은.







### 유레카 서버 인증



의 하나가 HTTP 기본 인증이 자동으로 유레카 클라이언트에 추가됩니다`eureka.client.serviceUrl.defaultZone`URL을 (같은 컬 스타일 그 안에 포함 된 자격 증명이`[http://user:password@localhost:8761/eureka](http://user:password@localhost:8761/eureka)`).더 복잡한 요구를 들어, 당신은 만들 수 있습니다`@Bean`유형의를`DiscoveryClientOptionalArgs`하고 주입`ClientFilter`모두는 클라이언트에서 서버로 호출에 적용됩니다, 그것으로 인스턴스.













노트



<td class="content">유레카의 한계로 인해 서버 당 기본 인증 자격 증명을 지원할 수 없으므로 발견 된 첫 번째 세트 만 사용됩니다.













### 상태 페이지 및 상태 표시기



Eureka 인스턴스의 상태 페이지 및 상태 표시기는 각각 Spring Boot Actuator 응용 프로그램의 유용한 끝점의 기본 위치 인 "/ info"및 "/ health"로 기본 설정됩니다.당신은 당신이 기본이 아닌 컨텍스트 경로 나 서블릿 경로 (예를 들어 사용하는 경우에도 액추에이터 응용 프로그램이 변경해야합니다`server.servletPath=/foo`) 또는 관리 엔드 포인트 경로 (예 :`management.contextPath=/admin`).예:





application.yml



<pre>유레카:예:statusPageUrlPath : $ {management.context-path} / infohealthCheckUrlPath : $ {management.context-path} / 건강</pre>







이러한 링크는 클라이언트가 사용하는 메타 데이터에 표시되며 일부 시나리오에서는 응용 프로그램에 요청을 보낼지 여부를 결정하는 데 사용되므로 정확하면 유용합니다.







### 보안 응용 프로그램 등록



앱이 HTTPS를 통해 연락을 원하는 경우에 당신은 두 개의 플래그를 설정할 수 있습니다`EurekaInstanceConfig`,_즉_ `eureka.instance.[nonSecurePortEnabled,securePortEnabled]=[false,true]`각각.이렇게하면 Eureka가 보안 통신에 대한 명시적인 선호를 보여주는 인스턴스 정보를 게시하게됩니다.봄 구름은`DiscoveryClient`항상 반환`[https://…​](https://%E2%80%A6%E2%80%8B/);`이 방식으로 구성 서비스에 대한 URI를하고, 유레카 (기본) 인스턴스 정보는 안전한 상태 점검 URL이있을 것이다.





유레카가 내부적으로 작동하는 방식 때문에 명시 적으로 명시 적으로 무시하지 않는 한 상태 및 홈 페이지에 대해 보안되지 않은 URL을 게시합니다.자리 표시자를 사용하여 eureka 인스턴스 URL을 구성 할 수 있습니다 (예 :





application.yml



<pre>유레카:예:statusPageUrl : https : // $ {eureka.hostname} / infohealthCheckUrl : https : // $ {eureka.hostname} / 건강homePageUrl : https : // $ {eureka.hostname} /</pre>







(즉, 주`${eureka.hostname}`유레카의 이후 버전에서만 사용할 기본 자리 표시 자입니다. 당신은뿐만 아니라, 예를 들어 사용을 봄 자리와 같은 일을 달성 할 수있다`${eureka.instance.hostName}`.)













노트



<td class="content">앱이 프록시 뒤에 있고 SSL 종료가 프록시에있는 경우 (예 : Cloud Foundry 또는 다른 플랫폼에서 서비스로 실행하는 경우) 프록시 "전달 된"헤더를 가로 채고 처리해야합니다. 응용 프로그램.'X-Forwarded - \ *'헤더를 명시 적으로 설정하면 Spring Boot 애플리케이션의 임베디드 Tomcat 컨테이너가 자동으로이 기능을 수행한다.틀린 표시는 앱이 자체적으로 렌더링 한 링크가 잘못된 것입니다 (잘못된 호스트, 포트 또는 프로토콜).













### 유레카 건강 검사



기본적으로 Eureka는 클라이언트 하트 비트를 사용하여 클라이언트가 작동 중인지 확인합니다.별도로 명시하지 않는 한 Discovery Client는 Spring Boot Actuator 당 응용 프로그램의 현재 상태 확인 상태를 전파하지 않습니다.성공적으로 등록한 후 유레카는 응용 프로그램이 항상 UP 상태임을 발표합니다.이 동작은 유레카 상태 검사를 사용하도록 설정하여 응용 프로그램 상태를 유레카로 전파함으로써 변경 될 수 있습니다.결과적으로 다른 모든 응용 프로그램은 'UP'이외의 상태에서 응용 프로그램으로 트래픽을 전송하지 않습니다.





application.yml



<pre>유레카:고객:건강 체크:enabled : true</pre>















경고



<td class="content">`eureka.client.healthcheck.enabled=true`에만 설정되어야한다`application.yml`.값에 설정`bootstrap.yml`와 유레카에 등록하는 등 바람직하지 않은 부작용이 발생할 수`UNKNOWN`상태.











당신이 건강 검진을 통해 더 많은 제어를 필요로하는 경우, 당신은 당신의 자신의 구현을 고려할 수 있습니다`com.netflix.appinfo.HealthCheckHandler`.







### 인스턴스 및 클라이언트에 대한 유레카 메타 데이터



Eureka 메타 데이터가 어떻게 작동하는지 이해하는 데 약간의 시간을 할애 할 가치가 있으므로 플랫폼에서 의미있는 방식으로 사용할 수 있습니다.호스트 이름, IP 주소, 포트 번호, 상태 페이지 및 상태 확인과 같은 것들에 대한 표준 메타 데이터가 있습니다.이들은 서비스 레지스트리에 게시되고 클라이언트가 직접적으로 서비스에 연락하는 데 사용됩니다.추가 메타 데이터의 인스턴스 등록에 추가 될 수`eureka.instance.metadataMap`있으며, 이는 원격 클라이언트에 액세스 할 수 있지만,이 메타 데이터의 의미를 인식하지 않는 한, 일반적으로, 클라이언트의 동작을 변경하지 않을 것이다.Spring Cloud가 이미 메타 데이터 맵에 의미를 할당 한 몇 가지 특별한 경우가 있습니다.





#### Cloudfoundry에서 유레카 사용하기



Cloudfoundry는 글로벌 라우터를 갖추고있어 동일한 앱의 모든 인스턴스가 동일한 호스트 이름을 갖습니다 (비슷한 아키텍처를 가진 다른 PaaS 솔루션에서도 동일 함).이것은 반드시 Eureka를 사용하는 데 장애가되는 것은 아니지만 라우터를 사용하는 경우 (플랫폼을 설정하는 방법에 따라 권장 또는 필수) 호스트 이름과 포트 번호를 명시 적으로 설정해야합니다 (보안 또는 비보안 ) 라우터를 사용합니다.인스턴스 메타 데이터를 사용하여 클라이언트의 인스턴스 (예 : 사용자 정의 부하 분산 장치)를 구별 할 수도 있습니다.기본적으로는`eureka.instance.instanceId`입니다`vcap.application.instance_id`.예 :





application.yml



<pre>유레카:예:호스트 이름 : $ {vcap.application.uris [0]}nonSecurePort : 80</pre>







Cloudfoundry 인스턴스에서 보안 규칙을 설정하는 방법에 따라 직접 서비스 간 호출에 호스트 VM의 IP 주소를 등록하고 사용할 수 있습니다.이 기능은 중추 웹 서비스 (에 (아직) 사용할 수 없습니다[PWS](https://run.pivotal.io/)).







#### AWS에서 Eureka 사용



애플리케이션가 AWS 클라우드에 배치 될 예정이면 유레카 인스턴스 아마존 인식하도록 구성 할 것이며, 이는 사용자 지정하여 수행 할 수[EurekaInstanceConfigBean를](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-eureka-client/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java)다음 방법 :







    @Bean
    @Profile("!default")
    public EurekaInstanceConfigBean eurekaInstanceConfig() {
      EurekaInstanceConfigBean b = new EurekaInstanceConfigBean();
      AmazonInfo info = AmazonInfo.Builder.newBuilder().autoBuild("eureka");
      b.setDataCenterInfo(info);
      return b;
    }









#### 유레카 인스턴스 ID 변경



바닐라 넷플 릭스 유레카 인스턴스는 호스트 이름과 동일한 ID로 등록됩니다 (예 : 호스트 당 하나의 서비스 만).봄 클라우드 유레카는 다음과 같다 재치있는 기본을 제공합니다`${spring.cloud.client.hostname}:${spring.application.name}:${spring.application.instance_id:${server.port}}}`.예를 들어`myhost:myappname:8080`.





봄 클라우드를 사용하여 당신의 고유 식별자를 제공하여이를 대체 할 수 있습니다`eureka.instance.instanceId`.예 :





application.yml



<pre>유레카:예:instanceId : $ {spring.application.name} : $ {vcap.application.instance_id : $ {spring.application.instance_id : $ {random.value}}}</pre>







이 메타 데이터와 localhost에 배포 된 여러 서비스 인스턴스를 사용하면 무작위 값이 인스턴스를 고유하게 만듭니다.Cloudfoundry에서이`vcap.application.instance_id`랜덤 값이 필요하지 않도록, 봄 부팅 응용 프로그램에서 자동으로 채워집니다.









### EurekaClient 사용



당신이 응용 프로그램을 일단`@EnableDiscoveryClient`(또는`@EnableEurekaClient`) 당신은에서 서비스 인스턴스를 검색하는 데 사용할 수 있습니다[유레카 서버](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-eureka-server).이를위한 한 가지 방법은 기본을 사용하는 것이다`com.netflix.discovery.EurekaClient`(봄 구름 반대로`DiscoveryClient`), 예를 들면







<pre>@Autowired개인 EurekaClient discoveryClient;
public String serviceUrl () {InstanceInfo 인스턴스 = discoveryClient.getNextServerFromEureka ( "저장", 거짓);return instance.getHomePageUrl ();}</pre>















팁







사용하지 마십시오`EurekaClient`의`@PostConstruct`방법 또는에서`@Scheduled`합니다 (이 경우 아무 곳이나 방법은`ApplicationContext`아직 시작되지 않을 수 있습니다).그것은 초기화됩니다`SmartLifecycle`(과`phase=0`) 그래서 당신이 사용할 수있는 신뢰할 수있는 최초의 또 다른에`SmartLifecycle`더 높은 단계로.

















### 기본 Netflix EurekaClient의 대안



넌 넷플릭스 원재료를 사용하지 않은`EurekaClient`보통 일종의 래퍼 뒤에 사용하는 것이 더 편리하다.봄 클라우드에 대한 지원이[척하기](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-feign)(A REST 클라이언트 빌더)도[스프링`RestTemplate`](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-ribbon)대신 실제 URL의 논리적 인 유레카 서비스 식별자 (VIP를) 사용합니다.당신은 간단하게 설정할 수있는 물리적 서버의 고정 목록 리본을 구성하려면`<client>.ribbon.listOfServers`물리적 주소 (또는 호스트 이름)의 쉼표로 구분 된 목록에`<client>`클라이언트의 ID입니다.





당신은 또한 사용할 수 있습니다`org.springframework.cloud.client.discovery.DiscoveryClient`넷플릭스, 예를 들어, 특정 아닙니다 발견 클라이언트에 대한 간단한 API를 제공하는을







<pre>@Autowired개인용 DiscoveryClient discoveryClient;
public String serviceUrl () {List <ServiceInstance> list = discoveryClient.getInstances ( "STORES");if (list! = null && list.size ()> 0) {return list.get (0) .getUri ();}null를 돌려 준다.}</pre>









### 서비스 등록이 너무 느린 이유는 무엇입니까?



인스턴스가된다는 것은 또한 (클라이언트를 통해 레지스트리에 주기적 하트 비트 포함`serviceUrl`기본 기간 30초과를).인스턴스, 서버 및 클라이언트가 모두 로컬 캐시에 동일한 메타 데이터를 가지고 있기 때문에 (3 개의 하트 비트가 필요할 수 있음) 클라이언트가 서비스를 검색 할 수 없습니다.사용자는 사용 기간이 변경`eureka.instance.leaseRenewalIntervalInSeconds`이 다른 서비스에 접속 된 클라이언트를 얻는 과정을 빠르게한다.프로덕션 환경에서는 임대 갱신 기간에 대한 가정을 서버에서 내부적으로 계산하기 때문에 기본값을 사용하는 것이 좋습니다.







### 구역



Eureka 클라이언트를 여러 영역에 배치 한 경우 다른 영역에서 서비스를 시도하기 전에 동일한 영역 내의 서비스를 활용하는 것이 더 좋습니다.이렇게하려면 유레카 클라이언트를 올바르게 구성해야합니다.





먼저, 유레카 서버를 각 영역에 배치하고 서로의 동료인지 확인해야합니다.섹션 참조[영역 및 영역을](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-eureka-server-zones-and-regions)자세한 내용은.





다음 당신은 당신의 서비스에있는 영역 유레카 말할 필요가있다. 당신은 사용하여이 작업을 수행 할 수 있습니다`metadataMap`속성을.예를 들어 경우`service 1`모두에 배포`zone 1`하고`zone 2`당신의 다음 유레카 속성을 설정해야합니다`service 1`





**Zone 1의 서비스 1**







    eureka.instance.metadataMap.zone = zone1
    eureka.client.preferSameZoneEureka = true







**Zone 2의 서비스 1**







    eureka.instance.metadataMap.zone = zone2
    eureka.client.preferSameZoneEureka = true













## 서비스 발견 : 유레카 서버





### 유레카 서버 포함 방법



프로젝트에서 유레카 서버를 포함하는 그룹과 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-eureka-server`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.







### 유레카 서버를 실행하는 방법



예시 유레카 서버;







    @SpringBootApplication
    @EnableEurekaServer
    public class Application {

        public static void main(String[] args) {
            new SpringApplicationBuilder(Application.class).web(true).run(args);
        }

    }







서버는 UI와 홈페이지를 갖고, 아래 일반 유레카 기능마다 HTTP API의 종단점`/eureka/*`.





유레카 배경 읽기 : 참조[플럭스 커패시터](https://github.com/cfregly/fluxcapacitor/wiki/NetflixOSS-FAQ#eureka-service-discovery-load-balancer)와[구글의 그룹 토론을](https://groups.google.com/forum/?fromgroups#!topic/eureka_netflix/g3p2r7gHnN0).













팁







Gradle의 의존성 해결 규칙과 부모 bom 기능의 부족으로 인해 spring-cloud-starter-eureka-server에 의존하기 만하면 응용 프로그램 시작시 오류가 발생할 수 있습니다.이 문제를 해결하려면 Spring Boot Gradle 플러그인을 추가해야하며 Spring 클라우드 스타터 상위 BOM을 다음과 같이 가져와야합니다.





build.gradle



    buildscript {
      dependencies {
        classpath("org.springframework.boot:spring-boot-gradle-plugin:1.3.5.RELEASE")
      }
    }

    apply plugin: "spring-boot"

    dependencyManagement {
      imports {
        mavenBom "org.springframework.cloud:spring-cloud-dependencies:Brixton.RELEASE"
      }
    }



















### 고 가용성, 영역 및 영역



Eureka 서버에는 백엔드 저장소가 없지만 레지스트리의 서비스 인스턴스는 등록을 최신 상태로 유지하기 위해 하트 비트를 보내야합니다 (메모리에서이 작업을 수행 할 수 있습니다).또한 클라이언트는 메모리에 유레카 등록 캐시를 가지고 있기 때문에 (서비스에 대한 모든 단일 요청에 대해 레지스트리에 갈 필요가 없습니다).





기본적으로 모든 유레카 서버는 유레카 클라이언트이기도하며 피어를 찾기 위해 적어도 하나의 서비스 URL이 필요합니다.제공하지 않으면 서비스가 실행되고 작동하지만 피어와 함께 등록 할 수 없다는 것에 대한 많은 소음이 로그에 기록됩니다.





참고[리본 지원 자세한 내용은 아래](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-ribbon)영역 및 지역에 대한 클라이언트 측에.







### 독립 실행 형 모드



두 개의 캐시 (클라이언트 및 서버)와 하트 비트의 결합으로 독립 실행 형 유레카 서버는 모니터 또는 탄력적 인 런타임 (예 : Cloud Foundry)을 유지하는 한 실패에 상당히 탄력적입니다.독립 실행 형 모드에서는 클라이언트 측 동작을 계속 끌 수 있으므로 계속 시도하지 않고 피어에 도달하지 못할 수도 있습니다.예:





application.yml (독립 실행 형 유레카 서버)



<pre>섬기는 사람:포트 : 8761
유레카:예:호스트 이름 : localhost고객:registerWithEureka : falsefetchRegistry : 거짓serviceUrl :defaultZone : http : // $ {eureka.instance.hostname} : $ {server.port} / eureka /</pre>







(가) 알`serviceUrl`로컬 인스턴스와 동일한 호스트를 가리키고 있습니다.







### 또래 인식



유레카는 여러 인스턴스를 실행하고 서로 등록하도록 요청함으로써 훨씬 더 탄력적으로 사용할 수 있습니다.사실,이 때문에 당신이 그것을 작동하도록 할 필요가 유효한를 추가하고, 기본 동작입니다`serviceUrl`피어, 예를





application.yml (두 개의 피어 인식 유레카 서버)



<pre>---봄:프로필 : peer1유레카:예:호스트 이름 : peer1고객:serviceUrl :defaultZone : http : // peer2 / eureka /
---봄:프로필 : peer2유레카:예:호스트 이름 : peer2고객:serviceUrl :defaultZone : http : // peer1 / eureka /</pre>







이 예제에서는 두 개의 호스트 (peer1 및 peer2)에서 동일한 서버를 실행하고 다른 Spring 프로파일에서 실행하여 사용할 수있는 YAML 파일을 가지고 있습니다.당신은 조작하여 (생산에 그 일을 훨씬 값이 아니다) 단일 호스트에서 피어 인식을 테스트하기 위해이 구성을 사용할 수있는`/etc/hosts`호스트 이름을 해결하기 위해이.사실,이`eureka.instance.hostname`당신이 자신의 호스트 이름을 알고있는 컴퓨터에서 실행중인 경우 필요하지 않습니다 (그것은 사용하여 조회됩니다`java.net.InetAddress`기본적으로).





시스템에 여러 피어를 추가 할 수 있으며, 둘 이상의 피어가 모두 하나의 가장자리로 서로 연결되어 있으면 서로간에 등록을 동기화합니다.피어가 물리적으로 분리 된 경우 (데이터 센터 내부 또는 여러 데이터 센터간에) 시스템은 원칙적으로 스플릿 브레인 유형 장애를 극복 할 수 있습니다.







### IP 주소 선호



어떤 경우에는 유레카가 호스트 이름이 아닌 서비스의 IP 주소를 광고하는 것이 바람직합니다.집합`eureka.instance.preferIpAddress`을`true`응용 프로그램 유레카에 등록 할 때, 호스트 이름 대신 IP 주소를 사용한다.











## 회로 차단기 : Hystrix 클라이언트





넷플릭스라는 라이브러리를 만들었습니다[Hystrix](https://github.com/Netflix/Hystrix)구현하는[회로 차단기 패턴을](http://martinfowler.com/bliki/CircuitBreaker.html).마이크로 서비스 아키텍처에서는 서비스 호출의 다중 레이어를 갖는 것이 일반적입니다.





![HystrixGraph](./spring-cloud-netflix-doc-images/HystrixGraph.png)

그림 1\. 마이크로 서비스 그래프





서비스 수준이 낮 으면 서비스가 실패하여 연쇄 적으로 장애가 발생할 수 있습니다.특정 서비스에 대한 통화가 특정 임계 값에 도달하면 (Hystrix에서는 5 초 동안 20 개의 실패가 기본값 임) 회선이 열리고 통화가 이루어지지 않습니다.오류 및 개방 회로의 경우 폴백은 개발자가 제공 할 수 있습니다.





![HystrixFallback](./spring-cloud-netflix-doc-images/HystrixFallback.png)

그림 2\. Hystrix 폴백으로 계단식 오류 방지





개방 회로가 있으면 계단식 오류가 발생하지 않으므로 압도되거나 실패한 서비스를 치료할 수 있습니다.폴백은 또 다른 Hystrix 보호 호출, 정적 데이터 또는 정상적인 빈 값일 수 있습니다.폴백은 체인으로 연결되어 첫 번째 폴백이 다른 비즈니스 호출을 만들어 정적 데이터로 다시 폴백 할 수 있습니다.





### Hystrix 포함하는 방법



프로젝트에 Hystrix을 포함하려면 그룹 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-hystrix`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.





부팅 앱의 예 :







<pre>@SpringBootApplication@EnableCircuitBreakerpublic class Application {
공공 정적 무효 메인 (문자열 [] args) {새로운 SpringApplicationBuilder (Application.class) .web (true) .run (args);}
}
@구성 요소공용 클래스 StoreIntegration {
@HystrixCommand (fallbackMethod = "defaultStores")공용 객체 getStores (Map <String, Object> 매개 변수) {// 실패 할 수있는 일을하십시오.}
공용 객체 defaultStores (Map <String, Object> 매개 변수) {return / * 유용한 정보 * /;}}</pre>







이`@HystrixCommand`라는 넷플 릭스있는 contrib 라이브러리에서 제공하는["javanica"](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica).스프링 클라우드는 Hystrix 회로 차단기에 연결된 프록시에서 주석을 사용하여 스프링 빈을 자동으로 래핑합니다.회로 차단기는 회로를 열고 닫는시기와 고장이 발생할 경우 수행 할 작업을 계산합니다.





를 구성하려면`@HystrixCommand`당신은 사용할 수`commandProperties`의 목록 속성을`@HystrixProperty`주석.참조하십시오[여기에](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica#configuration)자세한 내용은.참고 항목[Hystrix 위키](https://github.com/Netflix/Hystrix/wiki/Configuration)사용할 수있는 속성에 대한 자세한 내용을.







### 보안 컨텍스트 전파 또는 스프링 스코프 사용



당신은 어떤 스레드 로컬 컨텍스트가에 전파하려는 경우`@HystrixCommand`는 (시간 초과의 경우) 스레드 풀에서 명령을 실행하기 때문에 작동하지 않습니다 디폴트 선언.일부 구성을 사용하여 발신자와 동일한 스레드를 사용하거나 주석에서 다른 "격리 전략"을 사용하도록 요청하여 Hystrix를 전환 할 수 있습니다.예 :







    @HystrixCommand(fallbackMethod = "stubMyService",
        commandProperties = {
          @HystrixProperty(name="execution.isolation.strategy", value="SEMAPHORE")
        }
    )
    ...







당신이 사용하는 경우 같은 일이 적용`@SessionScope`나`@RequestScope`.범위가 지정된 컨텍스트를 찾을 수 없다는 런타임 예외 때문에이 작업을 수행해야하는시기를 알 수 있습니다.





또한 설정할 수있는 옵션이`hystrix.shareSecurityContext`에 속성을`true`.이렇게하면 자동차가 전송 것 Hystrix 동시성 전략 플러그인 후크 구성합니다`SecurityContext`Hystrix 명령에 의해 사용되는에 주 스레드에서합니다.Hystrix는 확장 메커니즘이 자신을 선언하여 사용할 수 있도록 여러 hystrix 동시성 전략은 등록 할 수 없습니다`HystrixConcurrencyStrategy`스프링 빈으로.Spring Cloud는 Spring 컨텍스트 내에서 구현을 검색하여 자체 플러그인 내부에 랩핑합니다.







### 건강 지표



접속 회로 차단기의 상태도에 노출되어`/health`호출 애플리케이션의 엔드 포인트.







    {
        "hystrix": {
            "openCircuitBreakers": [
                "StoreIntegration::getStoresByLocationLink"
            ],
            "status": "CIRCUIT_OPEN"
        },
        "status": "UP"
    }









### Hystrix 메트릭스 스트림



Hystrix 메트릭 스트림을 사용하려면에 대한 종속성을 포함한다`spring-boot-starter-actuator`.이 노출됩니다`/hystrix.stream`관리 엔드 포인트로.







        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-actuator</artifactId>
        </dependency>













## 회로 차단기 : Hystrix 대시 보드





Hystrix의 주요 이점 중 하나는 각 HystrixCommand에 대해 수집하는 일련의 메트릭입니다.Hystrix Dashboard는 각 회로 차단기의 상태를 효율적으로 표시합니다.





![Hystrix](./spring-cloud-netflix-doc-images/Hystrix.png)

그림 3\. Hystrix 대시 보드





### Hystrix 대시 보드 포함 방법



프로젝트에서 Hystrix 대시 보드를 포함하는 그룹과 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-hystrix-dashboard`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.





Hystrix 대시 보드와 봄 부트 메인 클래스에 주석을 실행합니다`@EnableHystrixDashboard`.그런 다음 방문`/hystrix`및 개별 인스턴스에 대시 보드를 가리`/hystrix.stream`Hystrix 클라이언트 응용 프로그램에서 엔드 포인트.







### 터빈



개별 인스턴스를 보면 Hystrix 데이터는 시스템의 전반적인 상태와 관련하여별로 유용하지 않습니다.[터빈](https://github.com/Netflix/Turbine)관련 모든 집계하는 응용 프로그램입니다`/hystrix.stream`결합으로 엔드 포인트를`/turbine.stream`Hystrix 대시 보드에 사용.개별 인스턴스는 Eureka를 통해 위치합니다.터빈을 실행하면 사용하여 메인 클래스에 주석을만큼 간단하다`@EnableTurbine`(예를 들어, 클래스 경로를 설정하는 스프링 클라우드 스타터 터빈을 사용하여) 주석.에서 문서화 된 구성 등록 정보의 모든[터빈 1 위키](https://github.com/Netflix/Turbine/wiki/Configuration-(1.x))적용됩니다.유일한 차이점은이 있다는 것입니다`turbine.instanceUrlSuffix`이 자동으로하지 않는 한 처리로 앞에 추가 포트를 필요로하지 않는다`turbine.instanceInsertPort=false`.













노트



<td class="content">기본적으로 터빈이 찾는`/hystrix.stream`그 조회하여 등록 된 인스턴스 엔드 포인트`homePageUrl`추가 한 다음, 유레카의 항목을`/hystrix.stream`그것.이 경우 의미합니다`spring-boot-actuator`(기본값) 자신의 포트에서 실행되고, 호출에`/hystrix.stream`실패합니다.터빈이 올바른 포트에 Hystrix 스트림을 찾을 수 있도록하려면 추가 할 필요가`management.port`인스턴스의 메타 데이터에 :













<pre>유레카:예:메타 데이터 -지도 :관리. 포트 : $ {management.port : 8081}</pre>







구성 키는`turbine.appConfig`터빈 인스턴스를 조회하는 데 사용할 유레카 serviceIds의 목록입니다.: 터빈 스트림은 다음과 같은 URL을 사용 Hystrix 대시 보드에 사용된다`[http://my.turbine.sever:8080/turbine.stream?cluster=<CLUSTERNAME>](http://my.turbine.sever:8080/turbine.stream?cluster=%3CCLUSTERNAME%3E);`(클러스터 파라미터 이름이 "기본"인 경우 생략 될 수있다)를.`cluster`매개 변수의 항목과 일치해야합니다`turbine.aggregator.clusterConfig`.eureka에서 반환 된 값은 대문자이므로 Eureka에 등록 된 앱이 '고객'인 경우이 예제가 작동 할 것으로 기대합니다.







<pre>터빈:어 그리 게이터 :clusterConfig : 고객appConfig : 고객</pre>







은`clusterName`에 SPEL 표현하여 사용자 정의 할 수 있습니다`turbine.clusterNameExpression`루트의 인스턴스`InstanceInfo`.기본값은`appName`유레카 서비스 id합니다 (즉, 클러스터 키로 끝 즉,`InstanceInfo`고객이있다`appName`"고객"의 참조).각기 다른 예로들 수`turbine.clusterNameExpression=aSGName`AWS ASG 이름에서 클러스터 이름을 얻을 것이다.다른 예 :







<pre>터빈:어 그리 게이터 :clusterConfig : SYSTEM, USERappConfig : 고객, 상점, UI, 관리자clusterName 표현식 : metadata [ 'cluster']</pre>







이 경우 4 개 서비스의 클러스터 이름은 메타 데이터 맵에서 가져오고 "SYSTEM"및 "USER"가 포함 된 값이 있어야합니다.





모든 응용 프로그램에 "기본"클러스터를 사용하려면 문자열 리터럴 표현식 (작은 따옴표로 묶고 YAML에있는 경우 큰 따옴표로 이스케이프 처리해야 함)이 필요합니다.







<pre>터빈:appConfig : 고객, 상점clusterNameExpression : " ''기본값 '"</pre>







봄 클라우드가 제공하는`spring-cloud-starter-turbine`당신은 터빈 서버를 실행 얻기 위해 필요한 모든 종속성을 갖는다.그냥 봄 부팅 응용 프로그램을 작성하고 그것을 주석`@EnableTurbine`.













노트



<td class="content">기본적으로 Spring Cloud는 Turbine이 호스트와 포트를 사용하여 클러스터 당 호스트 당 여러 프로세스를 허용합니다.당신은 않습니다 터빈에 내장 된 기본 넷플릭스 동작하려면_하지_클러스터 당 (인스턴스 ID의 핵심 호스트 이름이다), 호스트 당 여러 프로세스를 허용을 누른 다음 속성을 설정합니다`turbine.combineHostPort=false`.













### 터빈 스트림



일부 환경 (예 : PaaS 설정)에서는 모든 분산 Hystrix 명령에서 메트릭을 가져 오는 클래식 터빈 모델이 작동하지 않습니다.이 경우 Hystrix가 Turbine에 메트릭을 푸시하도록 할 수 있으며 Spring Cloud는 메시징으로이를 지원합니다.클라이언트에서 수행 할 필요가에 종속성을 추가입니다`spring-cloud-netflix-hystrix-stream`및`spring-cloud-starter-stream-*`당신의 선택의 (브로커에 대한 자세한 내용은 봄 클라우드 스트림 설명서를 참조하는 방법과 클라이언트 자격 증명을 구성하는,하지만 로컬 브로커 상자 밖으로 작동합니다 ).





서버 측에서 그냥 봄 부팅 응용 프로그램을 작성하고 그것을 주석`@EnableTurbineStream`과 기본적으로 포트 8989에 올 것이다 (모든 경로, 해당 포트에 Hystrix 대시 보드를 가리 킵니다).당신이 중 하나를 사용하여 포트를 사용자 정의 할 수 있습니다`server.port`또는`turbine.stream.port`.당신이있는 경우`spring-boot-starter-web`및`spring-boot-starter-actuator`뿐만 아니라 클래스 패스에, 당신은 제공 (기본적으로 톰캣)와 별도의 포트에 액추에이터 엔드 포인트를 열 수있는`management.port`다른 어떤을.





그런 다음 Hystrix 대시 보드를 개별 Hystrix 스트림 대신 Turbine Stream Server로 지정할 수 있습니다.터빈 스트림이 myhost의 포트 8989에서 실행중인 경우, 다음 넣어`[http://myhost:8989](http://myhost:8989/)`Hystrix 대시 보드에서 스트림 입력 필드에.회선은 각각의 serviceId가 접두어로 붙고 그 뒤에 점과 회로 이름이옵니다.





봄 클라우드가 제공하는`spring-cloud-starter-turbine-stream`단지 예를 들어, 당신의 선택의 스트림 바인더를 추가 - 당신은 터빈 스트림 서버를 실행 얻기 위해 필요한 모든 종속성을 갖는다`spring-cloud-starter-stream-rabbit`.Netty 기반이기 때문에 Java 8이 필요합니다.











## 클라이언트 측로드 밸런서 : 리본





리본은 HTTP 및 TCP 클라이언트의 동작을 제어 할 수있는 클라이언트 측로드 밸런서입니다.당신이 사용하는, 그래서 만약 이미 리본을 사용 꾀병`@FeignClient`다음이 섹션에도 적용됩니다.





리본의 중심 개념은 명명 된 클라이언트의 개념입니다.(예를 사용하여 각 부하 분산 장치는 필요에 따라 원격 서버에 접속하기 위해 함께 작동 구성 요소의 앙상블의 일부, 그리고 앙상블은 응용 프로그램 개발자로주는 이름을 가진`@FeignClient`주석).봄 구름은 같은 새로운 앙상블 작성`ApplicationContext`하여 명명 된 각 클라이언트에 대한 수요를`RibbonClientConfiguration`.이것은 (다른 것들 중에서)를 포함`ILoadBalancer`하는`RestClient`, 및`ServerListFilter`.





### 리본 포함 방법



프로젝트에 리본을 포함하려면 그룹 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-ribbon`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.







### 리본 클라이언트 사용자 정의



당신은 외부 속성을 사용하여 리본 클라이언트의 일부 비트를 구성 할 수 있습니다`<client>.ribbon.*`당신은 봄 부팅 구성 파일을 사용할 수있는 것을 제외하고는 기본적으로 넷플 릭스 API를 사용하는 것보다 더 차이가없는.기본 옵션은 정적 필드로 검사 할 수있다`CommonClientConfigKey`(리본 코어의 일부).





봄 구름은 또한 당신 (의 위에 추가 구성을 선언하여 클라이언트의 모든 권한 걸릴 수 있습니다`RibbonClientConfiguration`사용)`@RibbonClient`.예:







    @Configuration
    @RibbonClient(name = "foo", configuration = FooConfiguration.class)
    public class TestConfiguration {
    }







이 경우 클라이언트가 이미 구성 요소로 구성되어`RibbonClientConfiguration`어느와 함께`FooConfiguration`(후자는 일반적으로 이전보다 우선합니다 경우).













경고



이`FooConfiguration`있어야한다`@Configuration`하지만이 아닌 관리 걸릴`@ComponentScan`그렇지 않으면 모두에 의해 공유됩니다, 기본 응용 프로그램 컨텍스트를`@RibbonClients`.당신이 사용하는 경우`@ComponentScan`(또는`@SpringBootApplication`당신이 포함되지 않도록하기위한 조치를 취할 필요) (예를 들어 별도의 겹치지 않는 패키지에 넣어, 또는 명시 적으로 검사 할 패키지를 지정`@ComponentScan`).











봄 클라우드 넷플릭스는 리본 기본적으로 (다음 콩을 제공`BeanType`beanName에을 :`ClassName`)





*   `IClientConfig`ribbonClientConfig :`DefaultClientConfigImpl`

*   `IRule`ribbonRule :`ZoneAvoidanceRule`

*   `IPing`ribbonPing :`NoOpPing`

*   `ServerList<Server>`ribbonServerList :`ConfigurationBasedServerList`

*   `ServerListFilter<Server>`ribbonServerListFilter :`ZonePreferenceServerListFilter`

*   `ILoadBalancer`ribbonLoadBalancer :`ZoneAwareLoadBalancer`





그 유형 중 하나의 콩 만들기 및에 배치`@RibbonClient`구성하면 (예 :`FooConfiguration`위)가 설명 된 콩의 각각을 대체 할 수 있습니다.예:







    @Configuration
    public class FooConfiguration {
        @Bean
        public IPing ribbonPing(IClientConfig config) {
            return new PingUrl();
        }
    }







이것은 대체`NoOpPing`와 함께`PingUrl`.







### 속성을 사용하여 리본 클라이언트 사용자 정의하기



버전 1.2.0부터 봄 구름 넷플릭스는 현재와 호환되도록 속성을 사용하여 사용자 정의 리본 고객 지원[리본 설명서를](https://github.com/Netflix/ribbon/wiki/Working-with-load-balancers#components-of-load-balancer).





이렇게하면 다른 환경에서 시작시 동작을 변경할 수 있습니다.





지원되는 특성은 다음과 같습니다과 접두어해야합니다`<clientName>.ribbon.`:





*   `NFLoadBalancerClassName`: 구현해야합니다.`ILoadBalancer`

*   `NFLoadBalancerRuleClassName`: 구현해야합니다.`IRule`

*   `NFLoadBalancerPingClassName`: 구현해야합니다.`IPing`

*   `NIWSServerListClassName`: 구현해야합니다.`ServerList`

*   `NIWSServerListFilterClassName`구현해야한다`ServerListFilter`













노트



<td class="content">이러한 속성에 정의 된 클래스를 사용하여 정의 콩보다 우선 순위가`@RibbonClient(configuration=MyRibbonConfig.class)`봄 구름 넷플릭스가 제공하는 기본값을.











을 설정하려면`IRule`서비스 이름에 대해`users`다음을 설정할 수 있습니다 :





application.yml



<pre>사용자 :리본:NFLoadBalancerRuleClassName : com.netflix.loadbalancer.WeightedResponseTimeRule</pre>







참고 항목[리본 문서](https://github.com/Netflix/ribbon/wiki/Working-with-load-balancers)리본에 의해 제공되는 구현을.







### 유레카와 함께 리본 사용하기



유레카는 리본과 함께 사용되면 (즉, 둘 다 클래스 패스에있는)`ribbonServerList`의 확장으로 오버라이드 (override)`DiscoveryEnabledNIWSServerList`유레카에서 서버 목록을 채 웁니다있다.또한 대체`IPing`와 인터페이스`NIWSDiscoveryPing`서버가있는 경우 유레카 명 규모가 결정되는합니다.`ServerList`기본적으로 설치되는이 인`DomainExtractingServerList`이의 목적은 (넷플 릭스에 의존하는 것입니다) AWS AMI 메타 데이터를 사용하지 않고 부하 분산 장치에 대한 물리적 메타 데이터를 사용할 수 있도록하는 것입니다.인스턴스 메타 데이터 (그래서 원격 클라이언트 설정에 규정 된 기본적으로 서버 목록은 "영역"정보로 구성됩니다`eureka.instance.metadataMap.zone`), 그리고이없는 경우는 경우 (영역에 대한 프록시 서버 호스트 이름에서 도메인 이름을 사용할 수 있습니다 플래그는`approximateZoneFromHostname`) 설정됩니다.영역 정보가 제공되면 그것이 사용될 수있다`ServerListFilter`.기본적으로는 기본이 때문에 클라이언트와 동일한 영역에 서버를 찾는 데 사용됩니다`ZonePreferenceServerListFilter`.클라이언트의 영역은, 예를 통해 기본적으로 원격 인스턴스와 동일한 방식으로 결정된다`eureka.instance.metadataMap.zone`.













노트



<td class="content">클라이언트 영역을 설정하는 "archaius"방식은 "@zone"이라는 구성 속성을 통해 이루어지며 Spring Cloud는 사용 가능한 경우 다른 모든 설정보다 우선적으로 사용합니다 (키는 YAML에서 인용해야합니다 구성).



















노트



<td class="content">영역 데이터의 다른 소스가없는 경우 클라이언트 구성 (인스턴스 구성과 반대 됨)을 기반으로 추측이 이루어집니다.우리는 걸릴`eureka.client.availabilityZones`영역 목록에 지역 이름에서지도를하다, 그리고 인스턴스의 자신의 지역의 제 1 영역을 당겨 (즉`eureka.client.region`, 이는 기본적으로 "우리 동쪽-1"기본 넷플릭스와 comatibility)입니다.













### 예 : 유레카가없는 리본 사용법



Eureka는 원격 서버의 발견을 추상화하는 편리한 방법이므로 클라이언트에 URL을 하드 코딩 할 필요는 없지만 사용하지 않으려는 경우에도 Ribbon 및 Feign은 여전히 ​​사용하기 쉽습니다.당신이 선언 한 가정`@RibbonClient`"매장"에 대한, 그리고 유레카는 (심지어 클래스 패스가 아닌)를 사용하지 않을 것입니다.리본 클라이언트는 기본적으로 구성된 서버 목록으로 구성되며 다음과 같은 구성을 제공 할 수 있습니다





application.yml



<pre>백화점:리본:listOfServers : example.com, google.com</pre>









### 예 : 리본에서 유레카 사용을 비활성화합니다.



속성을 설정하면`ribbon.eureka.enabled = false`명시 적으로 리본에서 유레카의 사용을 중지됩니다.





application.yml



<pre>리본:유레카:enabled : false</pre>









### 리본 API를 직접 사용



당신은 또한 사용할 수 있습니다`LoadBalancerClient`직접.예:







    public class MyClass {
        @Autowired
        private LoadBalancerClient loadBalancer;

        public void doStuff() {
            ServiceInstance instance = loadBalancer.choose("stores");
            URI storesUri = URI.create(String.format("http://%s:%s", instance.getHost(), instance.getPort()));
            // ... do something with the URI
        }
    }













## 선언적 REST 클라이언트 : Feign





[꾀병은](https://github.com/Netflix/feign)선언적 웹 서비스 클라이언트이다.따라서 웹 서비스 클라이언트를 쉽게 작성할 수 있습니다.Feign을 사용하려면 인터페이스를 만들고 주석을 달아 라.Feign 주석과 JAX-RS 주석을 포함하는 플러그 가능한 주석 지원 기능을 제공합니다.Feign은 또한 플러그 형 인코더와 디코더를 지원합니다.봄 구름 스프링 MVC 주석과 같은 사용에 대한 지원을 추가`HttpMessageConverters`봄 웹에서 기본적으로 사용합니다.Spring Cloud는 Ribbon과 Eureka를 통합하여 Feign을 사용할 때로드 밸런싱 된 HTTP 클라이언트를 제공합니다.





### 기소 포함하는 법



프로젝트에 척하기를 포함하는 그룹과 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-feign`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.





봄철 부팅 앱의 예







    @Configuration
    @ComponentScan
    @EnableAutoConfiguration
    @EnableEurekaClient
    @EnableFeignClients
    public class Application {

        public static void main(String[] args) {
            SpringApplication.run(Application.class, args);
        }

    }







StoreClient.java



    @FeignClient("stores")
    public interface StoreClient {
        @RequestMapping(method = RequestMethod.GET, value = "/stores")
        List<Store> getStores();

        @RequestMapping(method = RequestMethod.POST, value = "/stores/{storeId}", consumes = "application/json")
        Store update(@PathVariable("storeId") Long storeId, Store store);
    }







에서`@FeignClient`주석 문자열 값 ( "저장"위)는 리본로드 밸런서 (참조 만드는 데 사용되는 임의의 클라이언트 이름입니다[리본 지원 자세한 내용은 아래를](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-ribbon)).또한 사용하여 URL을 지정할 수 있습니다`url`속성 (절대 값 또는 그냥 호스트 이름).응용 프로그램 컨텍스트에서 Bean의 이름은 인터페이스의 완전한 이름입니다.'name'속성과 'FeignClient'가 추가 된 별칭도 생성됩니다.위의 예를 들어,`@Qualifier("storesFeignClient")`빈을 참조하기 위해 사용될 수있다.기본 변경하려면`@Qualifier`값을이가 함께 할 수있는`qualifier`가치`@FeignClient`.





위의 리본 클라이언트는 "상점"서비스의 실제 주소를 검색하려고합니다.응용 프로그램이 유레카 클라이언트 인 경우 유레카 서비스 레지스트리의 서비스가 해결됩니다.당신은 유레카를 사용하지 않으려면, 당신은 단순히 외부 구성 (참조에서 서버 목록을 구성 할 수 있습니다[예를 들어 위](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-ribbon-without-eureka)).







### 기본 값 재정의



Spring Cloud의 Feign 지원의 핵심 개념은 명명 된 클라이언트의 개념입니다.각 꾀병 클라이언트는 필요에 따라 원격 서버에 접속하기 위해 함께 작동 구성 요소의 앙상블의 일부이며, 앙상블 당신이 사용하는 응용 프로그램 개발자로 제공 이름이`@FeignClient`주석을.봄 구름은 같은 새로운 앙상블 작성`ApplicationContext`하여 명명 된 각 클라이언트에 대한 수요를`FeignClientsConfiguration`.이것은 (다른 것들 중에서)를 포함`feign.Decoder`하는`feign.Encoder`, 및`feign.Contract`.





봄 클라우드는 (의 위에 추가 구성 선언함으로써 꾀병 클라이언트의 전체 제어 할 수 있습니다`FeignClientsConfiguration`) 사용하여`@FeignClient`.예:







    @FeignClient(name = "stores", configuration = FooConfiguration.class)
    public interface StoreClient {
        //..
    }







이 경우 클라이언트가 이미 구성 요소로 구성되어`FeignClientsConfiguration`어떤과 함께`FooConfiguration`(후자가 전자보다 우선합니다 경우).













경고



<td class="content">이`FooConfiguration`있어야한다`@Configuration`하지만이 아닌 관리 걸릴`@ComponentScan`그렇지 않으면 모든 사용됩니다, 기본 응용 프로그램 컨텍스트를`@FeignClient`.당신이 사용하는 경우`@ComponentScan`(또는`@SpringBootApplication`당신이 포함되지 않도록하기위한 조치를 취할 필요) (예를 들어 별도의 겹치지 않는 패키지에 넣어, 또는 명시 적으로 검사 할 패키지를 지정`@ComponentScan`).



















노트



<td class="content">`serviceId`속성은 이제 찬성되지 않습니다`name`속성.



















경고



<td class="content">이전에는 사용`url`속성은 필요하지 않은`name`속성을.사용하는 것이`name`지금 필요합니다.











자리가 지원됩니다`name`및`url`속성.







    @FeignClient(name = "${feign.name}", url = "${feign.url}")
    public interface StoreClient {
        //..
    }







봄 클라우드 넷플릭스는 꾀병을 위해 기본적으로 다음 콩 제공 (`BeanType`beanName에을 :`ClassName`)





*   `Decoder`feignDecoder :`ResponseEntityDecoder`(래핑`SpringDecoder`)

*   `Encoder`feignEncoder :`SpringEncoder`

*   `Logger`feignLogger :`Slf4jLogger`

*   `Contract`feignContract :`SpringMvcContract`

*   `Feign.Builder`feignBuilder :`HystrixFeign.Builder`

*   `Client`feignClient : 리본을 사용하는 경우 그것은이다`LoadBalancerFeignClient`그렇지 않으면 기본 꾀병 클라이언트가 사용됩니다.





OkHttpClient 및 ApacheHttpClient는 고객이 설정하여 사용할 수있는 가장하다`feign.okhttp.enabled`또는`feign.httpclient.enabled`에`true`각각, 및 클래스 패스에 그들을 가지고.





봄 클라우드 넷플릭스는_하지 않습니다_꾀병 기본적으로 다음 콩을 제공하지만 여전히 꾀병 클라이언트를 만들 수있는 응용 프로그램 컨텍스트에서 이러한 종류의 콩을 검색 :





*   `Logger.Level`

*   `Retryer`

*   `ErrorDecoder`

*   `Request.Options`

*   `Collection<RequestInterceptor>`





그 유형 중 하나의 콩 만들기 및에 배치`@FeignClient`구성하면 (예 :`FooConfiguration`위)가 설명 된 콩의 각각을 대체 할 수 있습니다.예:







    @Configuration
    public class FooConfiguration {
        @Bean
        public Contract feignContract() {
            return new feign.Contract.Default();
        }

        @Bean
        public BasicAuthRequestInterceptor basicAuthRequestInterceptor() {
            return new BasicAuthRequestInterceptor("user", "password");
        }
    }







이 대체`SpringMvcContract`로`feign.Contract.Default`하고, 추가`RequestInterceptor`의 컬렉션`RequestInterceptor`.





기본 구성이 지정 될 수있는`@EnableFeignClients`특성을`defaultConfiguration`상술 한 바와 같이 유사한 방식.차이점은이 구성에 적용 할 것입니다_모든_꾀병 클라이언트.













노트



<td class="content">당신은 사용해야 할 경우`ThreadLocal`당신의 바운드 변수`RequestInterceptor`s you will need to either set the thread isolation strategy for Hystrix to `SEMAPHORE`또는 척하기에 Hystrix을 사용하지 않도록 설정합니다.











application.yml







    # To disable Hystrix in Feign
    feign:
      hystrix:
        enabled: false

    # To set thread isolation to SEMAPHORE
    hystrix:
      command:
        default:
          execution:
            isolation:
              strategy: SEMAPHORE









### 수동으로 고객 보호 생성



경우에 따라 위의 방법을 사용하여 불가능한 방식으로 고객을 맞춤화해야 할 수도 있습니다.이 경우에는 사용하는 클라이언트 만들 수 있습니다[척하기 빌더 API를](https://github.com/OpenFeign/feign/#basics).다음은 같은 인터페이스를 가진 두 개의 Feign 클라이언트를 생성하지만 별도의 요청 인터셉터를 사용하여 각각을 구성하는 예제입니다.







    @Import(FeignClientsConfiguration.class)
    class FooController {

    	private FooClient fooClient;

    	private FooClient adminClient;

        @Autowired
    	public FooController(
    			Decoder decoder, Encoder encoder, Client client) {
    		this.fooClient = Feign.builder().client(client)
    				.encoder(encoder)
    				.decoder(decoder)
    				.requestInterceptor(new BasicAuthRequestInterceptor("user", "user"))
    				.target(FooClient.class, "http://PROD-SVC");
    		this.adminClient = Feign.builder().client(client)
    				.encoder(encoder)
    				.decoder(decoder)
    				.requestInterceptor(new BasicAuthRequestInterceptor("admin", "admin"))
    				.target(FooClient.class, "http://PROD-SVC");
        }
    }















노트



<td class="content">위의 예에서`FeignClientsConfiguration.class`봄 클라우드 넷플릭스가 제공하는 기본 구성입니다.



















노트



<td class="content">`PROD-SVC`고객이 요청할 서비스의 이름입니다.













### Hystrix 지원 지원



Hystrix가 classpath에 있다면, 기본적으로 Feign은 모든 메소드를 회로 차단기로 감쌀 것이다.을 반환하는`com.netflix.hystrix.HystrixCommand`도 사용할 수 있습니다.이렇게하면에 호출 (반응 패턴을 사용할 수 있습니다`.toObservable()`하거나`.observe()`또는 호출과 비동기 사용 (`.queue()`).





척하기위한 Hystrix 지원을 사용하지 않으려면 설정`feign.hystrix.enabled=false`.





클라이언트 당 기준으로 Hystrix 지원을 비활성화하려면 바닐라 작성`Feign.Builder`은 "프로토 타입"범위, 예를 들면와를 :







    @Configuration
    public class FooConfiguration {
        @Bean
    	@Scope("prototype")
    	public Feign.Builder feignBuilder() {
    		return Feign.builder();
    	}
    }









### Hystrix Fallbacks를 기쁘게합니다.



Hystrix는 회로가 열려 있거나 오류가있을 때 실행되는 기본 코드 경로 인 폴백의 개념을 지원합니다.A는 주어진에 대한 폴백을 사용하려면`@FeignClient`설정된`fallback`대체를 구현하는 클래스의 이름 속성을.







    @FeignClient(name = "hello", fallback = HystrixClientFallback.class)
    protected interface HystrixClient {
        @RequestMapping(method = RequestMethod.GET, value = "/hello")
        Hello iFailSometimes();
    }

    static class HystrixClientFallback implements HystrixClient {
        @Override
        public Hello iFailSometimes() {
            return new Hello("fallback");
        }
    }







하나는 대체 트리거를 만든 원인에 대한 액세스를 필요로하는 경우, 하나는 사용할 수있는`fallbackFactory`내부 속성을`@FeignClient`.







    @FeignClient(name = "hello", fallbackFactory = HystrixClientFallbackFactory.class)
    protected interface HystrixClient {
    	@RequestMapping(method = RequestMethod.GET, value = "/hello")
    	Hello iFailSometimes();
    }

    @Component
    static class HystrixClientFallbackFactory implements FallbackFactory<HystrixClient> {
    	@Override
    	public HystrixClient create(Throwable cause) {
    		return new HystrixClientWithFallBackFactory() {
    			@Override
    			public Hello iFailSometimes() {
    				return new Hello("fallback; reason was: " + cause.getMessage());
    			}
    		};
    	}
    }















경고



<td class="content">Feign의 대체 기능 구현과 Hystrix 대체 버전의 작동 방식에는 제한이 있습니다.폴백은 현재 반환 방법에 대해 지원되지 않습니다`com.netflix.hystrix.HystrixCommand`및`rx.Observable`.













### 기꺼이 상속 지원



Feign은 단일 상속 인터페이스를 통해 상용구 API를 지원합니다.이를 통해 공통 작업을 편리한 기본 인터페이스로 그룹화 할 수 있습니다.





UserService.java



    public interface UserService {

        @RequestMapping(method = RequestMethod.GET, value ="/users/{id}")
        User getUser(@PathVariable("id") long id);
    }







UserResource.java



    @RestController
    public class UserResource implements UserService {

    }







UserClient.java



    package project.user;

    @FeignClient("users")
    public interface UserClient extends UserService {

    }















노트



<td class="content">일반적으로 서버와 클라이언트간에 인터페이스를 공유하는 것은 바람직하지 않습니다.이것은 tight coupling을 소개하고 실제로는 현재의 형태로 Spring MVC에서 작동하지 않습니다 (메소드 매개 변수 매핑은 상속되지 않습니다).













### 희망 요청 / 응답 압축



귀하는 귀하의 Feign 요청에 대해 요청 또는 응답 GZIP 압축을 활성화하는 것을 고려할 수 있습니다.다음 중 하나의 특성을 사용하여이를 수행 할 수 있습니다.







    feign.compression.request.enabled=true
    feign.compression.response.enabled=true







긴급 요청 압축을 사용하면 웹 서버에 설정할 수있는 것과 비슷한 설정을 사용할 수 있습니다.







    feign.compression.request.enabled=true
    feign.compression.request.mime-types=text/xml,application/xml,application/json
    feign.compression.request.min-request-size=2048







이러한 등록 정보를 사용하면 압축 미디어 유형 및 최소 요청 임계 값 길이에 대한 선택을 할 수 있습니다.







### 벌채 로깅



작성된 각 Feign 클라이언트에 대해 로거가 작성됩니다.기본적으로 로거 이름은 Feign 클라이언트를 만드는 데 사용 된 인터페이스의 전체 클래스 이름입니다.척하기 로깅 만에 응답`DEBUG`수준.





application.yml



    logging.level.project.user.UserClient: DEBUG







`Logger.Level`는 클라이언트에 따라 구성 할 수 있습니다 목적은, 얼마를 기록하는 척하기 알려줍니다.선택 사항은 다음과 같습니다.





*   `NONE`아니, 로깅 (**DEFAULT**).

*   `BASIC`, 요청 메소드와 URL 및 응답 상태 코드와 실행 시간 만 로깅하십시오.

*   `HEADERS`, 요청 및 응답 헤더와 함께 기본 정보를 기록하십시오.

*   `FULL`, 요청과 응답에 대한 헤더, 본문 및 메타 데이터를 기록합니다.





예를 들어, 다음을 설정할 것이다`Logger.Level`하기`FULL`:







    @Configuration
    public class FooConfiguration {
        @Bean
        Logger.Level feignLoggerLevel() {
            return Logger.Level.FULL;
        }
    }













## 외부 구성 : Archaius





[Archaius는](https://github.com/Netflix/archaius)넷플 릭스 클라이언트 측 구성 라이브러리입니다.모든 Netflix OSS 구성 요소가 구성에 사용하는 라이브러리입니다.Archaius는의 확장[아파치 코 몬즈 구성](https://commons.apache.org/proper/commons-configuration)프로젝트.소스를 폴링하여 변경 사항을 보거나 소스가 변경 사항을 클라이언트에 푸시하여 구성을 갱신 할 수 있습니다.Archaius는 동적 <Type> 속성 클래스를 속성의 핸들로 사용합니다.





아키라 우스의 예



    class ArchaiusTest {
        DynamicStringProperty myprop = DynamicPropertyFactory
                .getInstance()
                .getStringProperty("my.prop");

        void doSomething() {
            OtherClass.someMethod(myprop.get());
        }
    }







Archaius는 고유 한 구성 파일 세트 및로드 우선 순위를 가지고 있습니다.Spring 애플리케이션은 일반적으로 Archaius를 직접 사용하지 않아야하지만 Netflix 툴을 기본적으로 구성해야 할 필요성은 여전히 ​​남아 있습니다.Spring Cloud에는 Spring Environment Bridge가있어서 Archaius는 Spring Environment로부터 속성을 읽을 수 있습니다.이를 통해 스프링 부트 프로젝트는 일반 구성 툴체인을 사용하면서 문서화 된대로 Netflix 툴을 구성 할 수 있습니다.









## 라우터 및 필터 : Zuul





마이크로 서비스 아키텍처의 필수 부분에서 라우팅.예를 들어,`/`웹 어플리케이션에 매핑 될 수 있고,`/api/users`사용자의 서비스에 대응하고,`/api/shop`점포 서비스 매핑된다.[Zuul는](https://github.com/Netflix/zuul)넷플릭스에 의해 JVM 기반의 라우터와 서버 측 부하 분산 장치입니다.





[넷플릭스는 Zuul을 사용하여](http://www.slideshare.net/MikeyCohen1/edge-architecture-ieee-international-conference-on-cloud-engineering-32240146/27)다음과 같은 사항에 대해 :





*   입증

*   통찰력

*   스트레스 테스트

*   카나리아 테스트

*   동적 라우팅

*   서비스 마이그레이션

*   로드 흘리기

*   보안

*   정적 응답 처리

*   액티브 / 액티브 트래픽 관리





Zuul의 규칙 엔진을 사용하면 규칙과 필터를 Java 및 Groovy에 대한 지원 기능이 내장 된 본질적으로 모든 JVM 언어로 작성할 수 있습니다.













노트



<td class="content">구성 속성은`zuul.max.host.connections`두 가지 새로운 속성으로 대체되었습니다`zuul.host.maxTotalConnections`및`zuul.host.maxPerRouteConnections`각각 200과 20에있는 기본.



















노트



<td class="content">모든 경로의 기본 Hystrix 격리 패턴 (ExecutionIsolationStrategy)은 SEMAPHORE입니다.`zuul.ribbonIsolationStrategy`이 격리 패턴을 선호하는 경우 THREAD로 변경할 수 있습니다.











### Zuul을 포함시키는 방법



프로젝트에 Zuul을 포함하려면 그룹 스타터 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-starter-zuul`.참고 항목[봄 클라우드 프로젝트 페이지](http://projects.spring.io/spring-cloud/)현재 봄 클라우드 출시 기차와 빌드 시스템 설정에 대한 자세한 내용을.







### 임베디드 Zuul 역방향 프록시



Spring Cloud는 UI 애플리케이션이 하나 이상의 백엔드 서비스에 대한 호출을 프록시하기를 원하는 매우 일반적인 사용 사례의 개발을 용이하게하기 위해 임베디드 Zuul 프록시를 만들었습니다.이 기능은 필요한 모든 백엔드에 대해 독립적으로 CORS 및 인증 문제를 관리 할 필요가 없도록 사용자 인터페이스가 필요한 백엔드 서비스로 프록시 할 때 유용합니다.





그것을 사용하려면, 함께 봄 부트 메인 클래스에 주석`@EnableZuulProxy`, 이는 해당 서비스에 시내 전화를 전달합니다.규칙에 따라 ID "사용자"와 서비스에있는 프록시의 요청받을 것`/users`(제거 접두사와 참조).프록시는 검색을 통해에 전달하는 인스턴스를 찾을 리본을 사용하며, 모든 요청은 실행된다[hystrix 명령](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#hystrix-fallbacks-for-routes), 오류가 Hystrix 통계에 표시됩니다 있도록하고, 회로가 개방되면 프록시는 서비스에 문의하려고하지 않습니다.













노트



<td class="content">Zuul 스타터에는 검색 클라이언트가 포함되어 있지 않으므로 서비스 ID를 기반으로하는 경로의 경우 클래스 패스에있는 경로 중 하나를 제공해야합니다 (예 : Eureka는 하나의 선택 사항입니다).











설정 자동으로 추가 서비스 갖는 건너 뛰려면`zuul.ignored-services`서비스 ID 패턴 목록에 있습니다.서비스가 무시되고 명시 적으로 구성된 라우트 맵에 포함 된 패턴과 일치하면 무시되지 않습니다.예:





application.yml



     zuul:
      ignoredServices: '*'
      routes:
        users: /myusers/**







이 예에서, 모든 서비스가 무시되는**것을 제외하고**'사용자'.





프록시 경로를 보강하거나 변경하려면 다음과 같은 외부 구성을 추가 할 수 있습니다.





application.yml



     zuul:
      routes:
        users: /myusers/**







즉, "/ myusers"에 대한 http 호출은 "사용자"서비스로 전달됩니다 (예 : "/ myusers / 101"은 "/ 101"로 전달됨).





경로를 세밀하게 제어하려면 경로와 serviceId를 독립적으로 지정할 수 있습니다.





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          serviceId: users_service







이것은 "/ myusers"에 대한 http 호출이 "users_service"서비스로 전달됨을 의미합니다.경로는 개미 스타일 패턴으로 지정할 수있는 "경로"를 가져야하므로 "/ myusers / *"는 한 레벨에만 일치하지만 "/ myusers / **"는 계층 적으로 일치합니다.





백엔드의 위치는 "serviceId"(발견 된 서비스의 경우) 또는 "url"(물리적 위치의 경우)으로 지정할 수 있습니다.





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          url: http://example.com/users_service







이러한 단순 URL-노선은으로 실행되지 않는`HystrixCommand`없으며 리본 여러 URL을로드 균형 조정 할 수 있습니다.이를 달성하기 위해, 서비스 경로를 지정하고 (이 현재 리본에 유레카 지원을 사용하지 않도록 설정이 필요합니다 볼 수있는 서비스 id를위한 리본 클라이언트를 구성[자세한 정보는 위](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-ribbon-without-eureka)), 예를 들어,





application.yml



    zuul:
      routes:
        users:
          path: /myusers/**
          serviceId: users

    ribbon:
      eureka:
        enabled: false

    users:
      ribbon:
        listOfServers: example.com,google.com







regexmapper를 사용하여 serviceId와 route 사이에 규칙을 제공 할 수 있습니다.그룹이라는 정규 표현식을 사용하여 serviceId에서 변수를 추출하여 경로 패턴에 주입합니다.





ApplicationConfiguration.java



    @Bean
    public PatternServiceRouteMapper serviceRouteMapper() {
        return new PatternServiceRouteMapper(
            "(?<name>^.+)-(?<version>v.+$)",
            "${version}/${name}");
    }







즉, serviceId "myusers-v1"은 "/ v1 / myusers / **"경로에 매핑됩니다.모든 정규식이 허용되지만 모든 명명 된 그룹은 servicePattern과 routePattern에 모두 있어야합니다.servicePattern이 serviceId와 일치하지 않으면 기본 비헤이비어가 사용됩니다.위의 예에서 serviceId "myusers"는 "/ myusers / **"경로에 매핑됩니다 (버전이 없음).이 기능은 기본적으로 비활성화되어 있으며 발견 된 서비스에만 적용됩니다.





설정된 모든 매핑에 접두사를 추가하려면`zuul.prefix`다음과 같은 값으로,`/api`.요청이 기본적으로 전달되기 전에 프록시 접두사 (와 떨어져이 동작을 전환 요청에서 제거된다`zuul.stripPrefix=false`).개별 경로에서 서비스 별 접두어를 제거 할 수도 있습니다 (예 :





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          stripPrefix: false















노트



<td class="content">`zuul.stripPrefix`만에 접두사 집합에 적용됩니다`zuul.prefix`.이는 주어진 행의 내에 정의 된 접두어에 아무런 영향을 미치지 않는다`path`.











이 예에서 "/ myusers / 101"에 대한 요청은 "users"서비스의 "/ myusers / 101"로 전달됩니다.





`zuul.routes`항목은 실제로 유형의 개체에 바인딩`ZuulProperties`.해당 객체의 속성을 보면 "재시도"플래그도 있음을 알 수 있습니다.해당 플래그를 "true"로 설정하면 리본 클라이언트가 실패한 요청을 자동으로 다시 시도합니다 (필요하면 리본 클라이언트 구성을 사용하여 재시도 작업의 매개 변수를 수정할 수 있음).





`X-Forwarded-Host`헤더는 기본적으로 전달 요청에 추가됩니다.집합을 해제합니다`zuul.addProxyHeaders = false`.접두어 경로는 기본적으로 제거되고 백엔드에 대한 요청은 헤더 "X-Forwarded-Prefix"(위의 예에서 "/ myusers")를 선택합니다.





와 응용 프로그램은`@EnableZuulProxy`당신이 기본 경로 ( "/")를 설정하면 예를 들어, 독립 서버로 동작 할 수`zuul.route.home: /`경로의 모든 트래픽을 것 (즉, "/ **") "홈"서비스.





보다 세분화 된 무시가 필요할 경우 무시할 특정 패턴을 지정할 수 있습니다.이 패턴은 라우트 위치 지정 프로세스의 시작 부분에서 평가됩니다. 즉, 일치를 보장하기 위해 접두사를 패턴에 포함시켜야합니다.무시 된 패턴은 모든 서비스에 적용되며 다른 경로 사양보다 우선합니다.





application.yml



     zuul:
      ignoredPatterns: /**/admin/**
      routes:
        users: /myusers/**







즉, "/ myusers / 101"과 같은 모든 호출은 "users"서비스의 "/ 101"로 전달됩니다.그러나 "/ admin /"을 포함한 전화는 해결되지 않습니다.













경고



<td class="content">주문을 보존하기 위해 경로가 필요하다면 속성 파일을 사용하여 주문이 손실되므로 YAML 파일을 사용해야합니다.예 :











application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
        legacy:
          path: /**







당신은 속성의 파일을 사용했다 경우,`legacy`경로는 앞에 끝낼 수 있습니다`users`렌더링 경로`users`도달 할 수없는 경로입니다.







### 주루 HTTP 클라이언트



zuul 사용하는 기본 HTTP 클라이언트는 이제 아파치 HTTP 클라이언트 대신 사용되지 않는 리본에 의해 백업됩니다`RestClient`.사용`RestClient`또는 사용하도록`okhttp3.OkHttpClient`설정`ribbon.restclient.enabled=true`하거나`ribbon.okhttp.enabled=true`각각을.







### 쿠키 및 민감한 헤더



동일한 시스템에서 서비스간에 헤더를 공유해도 괜찮지 만, 민감한 헤더가 외부 서버로 다운 스트림으로 유출되는 것을 원하지 않을 것입니다.무시 된 헤더 목록을 라우트 구성의 일부로 지정할 수 있습니다.쿠키는 브라우저에서 잘 정의 된 의미 체계를 가지고 있기 때문에 특별한 역할을하며 항상 민감한 것으로 취급됩니다.프록시 사용자가 브라우저 인 경우 다운 스트림 서비스에 대한 쿠키도 모두 혼란 스럽기 때문에 문제가됩니다 (다운 스트림 서비스는 모두 같은 장소에서 온 것처럼 보입니다).





예를 들어 다운 스트림 서비스 중 하나에서만 쿠키를 설정하는 경우와 같이 서비스 설계에주의를 기울이면 백엔드에서 발신자까지 모든 흐름을 전달할 수 있습니다.또한 프록시가 쿠키를 설정하고 모든 백엔드 서비스가 동일한 시스템의 일부인 경우 간단하게 공유하는 것이 자연 스럽습니다 (예를 들어 Spring 세션을 사용하여 일부 공유 상태로 연결).그 이외에는 다운 스트림 서비스에 의해 설정된 쿠키는 호출자에게별로 유용하지 않을 수 있으므로 "Set-Cookie"및 "Cookie"를 중요한 헤더에 사용하는 것이 좋습니다 도메인의 일부가 아닙니다.심지어 경로에 대한**있습니다**도메인의 일부가 쿠키를 그들과 프록시 사이의 흐름을 허용하기 전에 무엇을 의미하는지에 대해 신중하게 생각하려고합니다.





민감한 헤더는 경로별로 쉼표로 구분 된 목록으로 구성 할 수 있습니다 (예 :





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          sensitiveHeaders: Cookie,Set-Cookie,Authorization
          url: https://downstream















노트



<td class="content">이 디폴트 값입니다`sensitiveHeaders`, 그래서 당신이 다른되고 싶어하지 않는 한 당신은 그것을 설정할 필요가 없습니다.NB 이것은 Spring Cloud Netflix 1.1에서 새로 추가되었습니다 (1.0에서는 사용자가 헤더를 제어 할 수없고 모든 쿠키가 양방향으로 흐른다).











는`sensitiveHeaders`그렇게 Zuul가 명시 적으로 빈리스트로 설정해야합니다 ( "무시"을 제외한) 모든 헤더를 보낼 수 있도록, 블랙리스트이며, 기본값은 비어 있지 않습니다.백엔드에 쿠키 또는 승인 헤더를 전달하려는 경우 필요합니다.예:





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          sensitiveHeaders:
          url: https://downstream







민감한 헤더도 설정하여 전 세계적으로 설정할 수 있습니다`zuul.sensitiveHeaders`.경우`sensitiveHeaders`경로에 설정이 글로벌 우선합니다`sensitiveHeaders`설정.







### 무시 된 헤더



당 노선에 민감한 헤더 이외에, 당신은에 대한 글로벌 값을 설정할 수 있습니다`zuul.ignoredHeaders`다운 스트림 서비스와 상호 작용하는 동안 폐기해야 값 (요청 및 응답 모두 포함)을.Spring Security가 classpath에 없다면, 디폴트로 비어있다. 그렇지 않으면 Spring Security가 지정한대로 잘 알려진 "보안"헤더 세트 (예 : 캐싱 포함)로 초기화된다.이 경우의 가정은 다운 스트림 서비스가이 헤더를 추가 할 수 있으며 프록시의 값을 원한다는 것입니다.경우 봄 보안에서 이러한 잘 알려진 보안 헤더를 버리지하려면 사용자가 설정할 수있는 클래스 패스에`zuul.ignoreSecurityHeaders`에`false`.이것은 Spring 보안에서 HTTP 보안 응답 헤더를 비활성화하고 다운 스트림 서비스에서 제공 한 값을 원할 때 유용 할 수 있습니다







### 경로 종점



당신이 사용하는 경우`@EnableZuulProxy`와 같은 HTTP를 통해 사용할 수 있습니다 (기본적으로) 가능하게 할 것이다 그쪽으로 봄 부팅 액추에이터 추가 엔드 포인트와 함께`/routes`.이 엔드 포인트에 대한 GET은 맵핑 된 라우트 목록을 리턴합니다.POST는 기존 경로를 강제로 새로 고칩니다 (예 : 서비스 카탈로그가 변경된 경우).













노트



<td class="content">경로는 서비스 카탈로그의 변경 사항에 자동으로 응답해야하지만 / routes에 대한 POST는 변경 사항을 즉시 적용하는 방법입니다.













### 교살 패턴과 로컬 전달



기존 애플리케이션이나 API를 마이그레이션 할 때 일반적인 패턴은 이전 엔드 포인트를 "교살하여 다른 구현으로 천천히 대체하는 것"입니다.Zuul 프록시는 이전 엔드 포인트 클라이언트의 모든 트래픽을 처리하는 데 사용할 수 있기 때문에이 도구를 사용하면 유용하지만 일부 요청은 새 엔드 포인트로 리디렉션합니다.





구성 예 :





application.yml



     zuul:
      routes:
        first:
          path: /first/**
          url: http://first.example.com
        second:
          path: /second/**
          url: forward:/second
        third:
          path: /third/**
          url: forward:/3rd
        legacy:
          path: /**
          url: http://legacy.example.com







이 예에서는 다른 패턴 중 하나와 일치하지 않는 모든 요청에 ​​매핑되는 '기존'앱을 차단하고 있습니다.의 경로는`/first/**`외부 URL로 새로운 서비스로 추출되었다.그리고에서 경로`/second/**`전달은 그래서 그들은 정상적인 봄으로, 로컬 등을 처리 할 수 있습니다`@RequestMapping`.의 경로`/third/**`도 전달되지만, 다른 접두사로 (즉,이`/third/foo`전달됩니다`/3rd/foo`).













노트



<td class="content">무시 된 패턴은 완전히 무시되지 않고 프록시에 의해 처리되지 않습니다 (따라서 효과적으로 로컬로 전달됩니다).













### Zuul을 통한 파일 업로드



당신이 경우`@EnableZuulProxy`당신은 파일을 업로드 할 프록시 경로를 사용할 수 있습니다 그리고 그것은 단지 한 파일이 작으로 작동합니다.큰 파일의 경우 봄 우회 대안 경로가`DispatcherServlet`"/ zuul / *"에 (다중 처리를 방지하기 위해).즉, 만약`zuul.routes.customers=/customers/**`당신이 "/ zuul / 고객 / *"큰 파일을 게시 할 수 있습니다.서블릿 경로를 통해 구체화된다`zuul.servletPath`.대용량 파일은 프록시 경로가 리본로드 밸런서를 통해 이동하는 경우 시간 초과 설정을 높여야합니다 (예 :





application.yml



    hystrix.command.default.execution.isolation.thread.timeoutInMilliseconds: 60000
    ribbon:
      ConnectTimeout: 3000
      ReadTimeout: 60000







스트리밍을 대용량 파일로 작업하려면 요청에서 청크 분할 인코딩을 사용해야합니다 (일부 브라우저에서는 기본적으로 수행하지 않음).예 : 명령 줄에서 :







<pre>$ curl -v -H "전송 인코딩 : 청크 분할"\-F "file=@mylarge.iso"로컬 호스트 : 9999 / zuul / 간단한 / 파일</pre>









### 쿼리 문자열 인코딩



들어오는 요청을 처리 할 때 쿼리 매개 변수가 디코딩되어 Zuul 필터에서 가능한 수정을 위해 사용할 수 있습니다.그런 다음 경로 필터에 백엔드 요청을 작성할 때 다시 인코딩됩니다.이 자바 스크립트의 사용하여 인코딩 된 경우, 결과는 원래의 입력보다 상이 할 수있다`encodeURIComponent()`, 예를 들어 방법.대부분의 경우이 문제가 발생하지는 않지만 일부 웹 서버는 복잡한 쿼리 문자열의 인코딩으로 인해 까다로울 수 있습니다.





쿼리 문자열의 원래 인코딩을 강제로,에 특별한 플래그를 통과 할 수있다`ZuulProperties`쿼리 문자열이와 같이 찍은되도록`HttpServletRequest::getQueryString`방법 :





application.yml



     zuul:
      forceOriginalQueryStringEncoding: true







**참고 :**이 특수 플래그 만 작동`SimpleHostRoutingFilter`하고 쉽게와 쿼리 매개 변수를 오버라이드 (override) 할 수있는 기능 느슨한`RequestContext.getCurrentContext().setRequestQueryParams(someOverriddenParameters)`쿼리 문자열은 이제 원래의 직접 인출되기 때문에를`HttpServletRequest`.







### Plain Embedded Zuul



당신이 사용하는 경우, 또한 프록시없이 Zuul 서버를 실행하거나, 선택적으로 프록시 플랫폼의 일부에 전환 할 수 있습니다`@EnableZuulServer`(대신`@EnableZuulProxy`).만약 유형의 애플리케이션에 추가하는 콩`ZuulFilter`들이 함께 한, 자동적으로 설치된다`@EnableZuulProxy`하지만 않고 프록시 필터 중 하나가 자동으로 추가된다.





이 경우 Zuul 서버에 대한 경로는 "zuul.routes. *"를 구성하여 계속 지정되지만 서비스 발견 및 프록시가 없으므로 "serviceId"및 "url"설정은 무시됩니다.예 :





application.yml



     zuul:
      routes:
        api: /api/**







"/ api / **"의 모든 경로를 Zuul 필터 체인에 매핑합니다.







### 주울 필터 사용 안 함



봄 클라우드에 대한 Zuul이 다수 포함되어`ZuulFilter`모두 프록시 서버 모드에서 기본적으로 활성화 콩.참조[zuul 필터 패키지를](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/zuul/filters)사용할 수 있습니다 가능한 필터에 대해.당신이 하나를 사용하지 않으려면, 간단하게 설정`zuul.<SimpleClassName>.<filterType>.disable=true`.관례 적으로, 패키지는 후`filters`Zuul 필터 유형입니다.예를 들어 사용하지 않도록 설정하는`org.springframework.cloud.netflix.zuul.filters.post.SendResponseFilter`설정`zuul.SendResponseFilter.post.disable=true`.







### 경로에 대한 Hystrix 폴백 제공



Zuul에 주어진 경로에 대한 회로가 트립되면 당신은 타입의 빈을 생성하여 대체 응답을 제공 할 수 있습니다`ZuulFallbackProvider`.이 빈 내에서 당신은 대체가되는 경로 ID를 지정하고를 제공 할 필요가`ClientHttpResponse`대체로 돌아갑니다.다음은 매우 간단합니다`ZuulFallbackProvider`구현.







    class MyFallbackProvider implements ZuulFallbackProvider {
        @Override
        public String getRoute() {
            return "customers";
        }

        @Override
        public ClientHttpResponse fallbackResponse() {
            return new ClientHttpResponse() {
                @Override
                public HttpStatus getStatusCode() throws IOException {
                    return HttpStatus.OK;
                }

                @Override
                public int getRawStatusCode() throws IOException {
                    return 200;
                }

                @Override
                public String getStatusText() throws IOException {
                    return "OK";
                }

                @Override
                public void close() {

                }

                @Override
                public InputStream getBody() throws IOException {
                    return new ByteArrayInputStream("fallback".getBytes());
                }

                @Override
                public HttpHeaders getHeaders() {
                    HttpHeaders headers = new HttpHeaders();
                    headers.setContentType(MediaType.APPLICATION_JSON);
                    return headers;
                }
            };
        }
    }







다음은 라우트 구성이 어떻게 생겼는지입니다.







    zuul:
      routes:
        customers: /customers/**









### 사이드카로 다국어 지원



Eureka, Ribbon 및 Config Server를 활용하고자하는 jvm이 아닌 언어를 사용합니까?봄 클라우드 넷플릭스 사이드카가 영감을받은[넷플릭스 프라나](https://github.com/Netflix/Prana).여기에는 주어진 서비스에 대한 모든 인스턴스 (예 : 호스트 및 포트)를 가져 오는 간단한 http API가 포함되어 있습니다.Eureka에서 경로 항목을 가져온 Zuul 프록시를 통해 서비스 호출을 프록시 할 수도 있습니다.Spring Cloud Config Server는 호스트 조회 또는 Zuul 프록시를 통해 직접 액세스 할 수 있습니다.비 jvm 앱은 헬스 체크를 구현하여 앱이 위 또는 아래로 움직이는 경우 사이드카가 eureka에보고 할 수 있도록해야합니다.





프로젝트에 사이드카를 포함하려면 그룹과 종속성 사용`org.springframework.cloud`및 이슈 ID를`spring-cloud-netflix-sidecar`.





사이드카를 사용하려면, 함께 봄 부팅 응용 프로그램을 만듭니다`@EnableSidecar`.이 주석은 포함`@EnableCircuitBreaker`,`@EnableDiscoveryClient`하고`@EnableZuulProxy`.비 -JVM 응용 프로그램과 같은 호스트에서 결과 응용 프로그램을 실행하십시오.





측면 차 추가 구성하려면 다음`sidecar.port`과`sidecar.health-uri`에를`application.yml`.`sidecar.port`속성은 비 JVM 앱이 수신 대기하는 포트입니다.이것은 사이드카가 앱을 유레카에 제대로 등록 할 수있게 해줍니다.는`sidecar.health-uri`봄 부팅 상태 표시기를 mimicks 비 JVM을 응용 프로그램에 액세스 할 수있는 URI입니다.다음과 같은 json 문서를 반환해야합니다.





건강 - 우호 - 문서



    {
      "status":"UP"
    }







다음은 사이드카 응용 프로그램의 application.yml 예제입니다.





application.yml



    server:
      port: 5678
    spring:
      application:
        name: sidecar

    sidecar:
      port: 8000
      health-uri: http://localhost:8000/health.json







에 대한 API를`DiscoveryClient.getInstances()`하는 방법이다`/hosts/{serviceId}`.여기에 대한 예제 응답입니다`/hosts/customers`즉 다른 호스트에 두 개의 인스턴스를 반환합니다.에서 (사이드카가 포트 5678에있는 경우)이 API는 비 JVM을 응용 프로그램에 액세스 할 수 있습니다`[http://localhost:5678/hosts/{serviceId}](http://localhost:5678/hosts/%7BserviceId%7D)`.





/ hosts / customers



    [
        {
            "host": "myhost",
            "port": 9000,
            "uri": "http://myhost:9000",
            "serviceId": "CUSTOMERS",
            "secure": false
        },
        {
            "host": "myhost2",
            "port": 9000,
            "uri": "http://myhost2:9000",
            "serviceId": "CUSTOMERS",
            "secure": false
        }
    ]







Zuul 프록시 자동으로 유레카에 공지 된 각 서비스에 대한 경로를 추가`/<serviceId>`, 그래서 고객 서비스에서 확인할 수있다`/customers`.비 JVM을 앱을 통해 고객 서비스에 액세스 할 수 있습니다`[http://localhost:5678/customers](http://localhost:5678/customers)`(사이드카가 포트 5678에서 수신 대기 가정).





구성 서버가 Eureka에 등록 된 경우 비 jvm 응용 프로그램은 Zuul 프록시를 통해 액세스 할 수 있습니다.ConfigServer의 서비스 id 인 경우`configserver`와 사이드카가 포트 5678에, 다음이에서 액세스 할 수 있습니다[에 http : // localhost를 : 5678 / configserver](http://localhost:5678/configserver)





비 jvm 앱은 YAML 문서를 반환하는 구성 서버의 기능을 이용할 수 있습니다.예를 들어, 호출[http://sidecar.local.spring.io:5678/configserver/default-master.yml는](http://sidecar.local.spring.io:5678/configserver/default-master.yml)다음과 같은 YAML 문서이 발생할 수 있습니다







    eureka:
      client:
        serviceUrl:
          defaultZone: http://localhost:8761/eureka/
      password: password
    info:
      description: Spring Cloud Samples
      url: https://github.com/spring-cloud-samples













## 스프링 MVC가있는 RxJava





봄 클라우드 넷플릭스는 포함[RxJava을](https://github.com/ReactiveX/RxJava).





> 
> 
> RxJava은의 자바 VM의 구현[반응성 확장](http://reactivex.io/)관찰 시퀀스를 사용하여 비동기 및 이벤트 기반 프로그램을 구성하기위한 라이브러리 :.
> 
> 





봄 클라우드 넷플릭스는 반환에 대한 지원 제공`rx.Single`스프링 MVC 컨트롤러에서 개체를.또한 사용 지원`rx.Observable`을위한 객체[서버 전송 이벤트 (SSE)를](https://en.wikipedia.org/wiki/Server-sent_events).내부 API를 이미 (참조 RxJava를 사용하여 구축하는 경우 이것은 매우 편리 할 수 있습니다[척하기 Hystrix 지원](http://cloud.spring.io/spring-cloud-netflix/spring-cloud-netflix.html#spring-cloud-feign-hystrix)예를 들어).





여기에 사용하는 몇 가지 예입니다`rx.Single`:







    @RequestMapping(method = RequestMethod.GET, value = "/single")
    public Single<String> single() {
    	return Single.just("single value");
    }

    @RequestMapping(method = RequestMethod.GET, value = "/singleWithResponse")
    public ResponseEntity<Single<String>> singleWithResponse() {
    	return new ResponseEntity<>(Single.just("single value"),
    			HttpStatus.NOT_FOUND);
    }

    @RequestMapping(method = RequestMethod.GET, value = "/singleCreatedWithResponse")
    public Single<ResponseEntity<String>> singleOuterWithResponse() {
    	return Single.just(new ResponseEntity<>("single value", HttpStatus.CREATED));
    }

    @RequestMapping(method = RequestMethod.GET, value = "/throw")
    public Single<Object> error() {
    	return Single.error(new RuntimeException("Unexpected"));
    }







당신이있는 경우`Observable`, 오히려 하나보다, 당신이 사용할 수있는`.toSingle()`나`.toList().toSingle()`.다음은 몇 가지 예입니다.







    @RequestMapping(method = RequestMethod.GET, value = "/single")
    public Single<String> single() {
        return Observable.just("single value").toSingle();
    }

    @RequestMapping(method = RequestMethod.GET, value = "/multiple")
    public Single<List<String>> multiple() {
        return Observable.just("multiple", "values").toList().toSingle();
    }

    @RequestMapping(method = RequestMethod.GET, value = "/responseWithObservable")
    public ResponseEntity<Single<String>> responseWithObservable() {

        Observable<String> observable = Observable.just("single value");
        HttpHeaders headers = new HttpHeaders();
        headers.setContentType(APPLICATION_JSON_UTF8);
        return new ResponseEntity<>(observable.toSingle(), headers, HttpStatus.CREATED);
    }

    @RequestMapping(method = RequestMethod.GET, value = "/timeout")
    public Observable<String> timeout() {
        return Observable.timer(1, TimeUnit.MINUTES).map(new Func1<Long, String>() {
            @Override
            public String call(Long aLong) {
                return "single value";
            }
        });
    }







스트리밍 엔드 포인트와 클라이언트가있는 경우 SSE가 옵션 일 수 있습니다.변환하려면`rx.Observable`봄에`SseEmitter`사용`RxResponse.sse()`.다음은 몇 가지 예입니다.







    @RequestMapping(method = RequestMethod.GET, value = "/sse")
    public SseEmitter single() {
    	return RxResponse.sse(Observable.just("single value"));
    }

    @RequestMapping(method = RequestMethod.GET, value = "/messages")
    public SseEmitter messages() {
    	return RxResponse.sse(Observable.just("message 1", "message 2", "message 3"));
    }

    @RequestMapping(method = RequestMethod.GET, value = "/events")
    public SseEmitter event() {
    	return RxResponse.sse(APPLICATION_JSON_UTF8,
    			Observable.just(new EventDto("Spring io", getDate(2016, 5, 19)),
    					new EventDto("SpringOnePlatform", getDate(2016, 8, 1))));
    }











## 통계 : 관중, 서보 및지도





Spectator / Servo와 Atlas를 함께 사용하면 거의 실시간 운영 통찰력을 제공합니다.





Spectator와 Servo는 Netflix의 메트릭 컬렉션 라이브러리입니다.Atlas는 차원 시계열 데이터를 관리하기위한 Netflix 메트릭 백엔드입니다.





Servo는 Netflix를 수년간 사용했으며 여전히 사용할 수 있지만 점차적으로 Java 8에서만 작동하도록 설계된 Spectator를 단계적으로 단계적으로 제거하고 있습니다. Spring Cloud Netflix는 둘 다 지원하지만 Java 8 기반 응용 프로그램은 Spectator .





### 차원 대 계층 적 메트릭 비교



스프링 부트 액츄에이터 메트릭은 계층 적이며 메트릭은 이름으로 만 구분됩니다.이러한 이름은 종종 마침표로 구분 된 이름에 키 / 값 속성 쌍 (차원)을 포함하는 이름 지정 규칙을 따릅니다.root 및 star-star라는 두 개의 끝점에 대해 다음과 같은 측정 항목을 고려하십시오.







    {
        "counter.status.200.root": 20,
        "counter.status.400.root": 3,
        "counter.status.200.star-star": 5,
    }







첫 x 째 메트릭은 단위 시간당 루트 엔드 포인트에 대한 정상적인 요청 성공 횟수를 제공합니다.그러나 시스템에 20 개의 엔드 포인트가 있고 모든 엔드 포인트에 대한 성공적인 요청 수가 필요한 경우에는 어떨까요?일부 계층 통계 백엔드는 당신은 와일드 카드를 지정할 수있는 것</font> **<font>그 모든 20 메트릭을 읽고 결과를 집계한다.</font> ****<font>또는, 당신은 제공 할 수있는</font> ****<font>것을 차단과 같은 메트릭 기록</font> ****<font>에 상관없이 엔드 포인트의 모든 성공적인 요청을하지만, 지금은 20 + 1 가지 통계를 작성해야합니다.</font> ****<font>이 서비스의 모든 엔드 포인트에 대한 성공적인 요청의 총 수를 알고 싶다면 마찬가지로 같은 와일드 카드를 지정할 수 있습니다</font>** <font>.`counter.status.200.`**`HandlerInterceptorAdapter``counter.status.200.all``counter.status.2`**`.*`





계층 적 메트릭 백엔드에서 와일드 카드 지원이 있더라도 명명 일관성은 어려울 수 있습니다.특히 이름 문자열에있는 이러한 태그의 위치는 시간이지나면서 질의를 위반할 수 있습니다.예를 들어 위의 계층 적 메트릭에 HTTP 메서드에 대해 추가 차원을 추가한다고 가정합니다.그런 다음`counter.status.200.root`이된다 없습니다`counter.status.200.method.get.root`등 우리는`counter.status.200.*`갑자기 더 이상 같은 의미 론적 의미를 가지고있다.또한 새로운 차원이 코드베이스 전체에 균일하게 적용되지 않으면 특정 쿼리가 불가능해질 수 있습니다.이것은 빨리 빠져 나갈 수 있습니다.





Netflix 측정 항목에는 태그가 지정됩니다 (일명 차원).각 메트릭에는 이름이 있지만이 단일 메트릭에는 더 많은 쿼리 유연성을 허용하는 여러 통계 및 '태그'키 / 값 쌍이 포함될 수 있습니다.실제로 통계 자체는 특수 태그에 기록됩니다.





Netflix Servo 또는 Spectator로 기록한 위에 설명 된 루트 끝점의 타이머에는 상태 코드 당 4 개의 통계가 포함됩니다. 여기서 카운트 통계는 Spring Boot Actuator의 카운터와 동일합니다.지금까지 HTTP 200과 400이 발생했다면 사용 가능한 데이터 포인트는 8 개가됩니다.







    {
        "root(status=200,stastic=count)": 20,
        "root(status=200,stastic=max)": 0.7265630630000001,
        "root(status=200,stastic=totalOfSquares)": 0.04759702862580789,
        "root(status=200,stastic=totalTime)": 0.2093076914666667,
        "root(status=400,stastic=count)": 1,
        "root(status=400,stastic=max)": 0,
        "root(status=400,stastic=totalOfSquares)": 0,
        "root(status=400,stastic=totalTime)": 0,
    }









### 기본 메트릭 컬렉션



추가 종속성 또는 구성하지 않고, 봄 클라우드 기반 서비스는 서보 자동 구성됩니다`MonitorRegistry`모든 스프링 MVC 요청에 대한 통계 수집을 시작.기본적으로, 이름 서보 타이머`rest`태그 MVC 각 요청에 대해 기록한다 :





1.  HTTP 메소드

2.  HTTP 상태 (예 : 200, 400, 500)

3.  URI (URI가 비어 있으면 "root"), Atlas에 대해 살균 됨

4.  요청 처리기가 예외를 던진 경우 예외 클래스 이름

5.  발신자는 경우 키 일치와 요청 헤더는`netflix.metrics.rest.callerHeader`요청에 설정되어 있습니다.에 대한 기본 키가 없습니다`netflix.metrics.rest.callerHeader`.발신자 정보를 수집하려면 응용 프로그램 속성에 추가해야합니다.





설정`netflix.metrics.rest.metricName`에서 메트릭의 이름을 변경하려면 속성을`rest`사용자가 제공하는 이름.





스프링 AOP가 활성화되어있는 경우`org.aspectj:aspectjweaver`런타임 클래스 경로에 존재하는, 봄 구름도로 만든 모든 클라이언트 호출에 대한 통계를 수집합니다`RestTemplate`.의 이름을 가진 서보 타이머`restclient`태그 각 MVC 요청에 대해 기록 될 것입니다 :





1.  HTTP 메소드

2.  HTTP 상태 (예 : 200, 500, 400)는이 경우 "CLIENT_ERROR"경우 응답이 널 (null), 또는 "IO_ERROR"반환`IOException`의 실행 중에 발생`RestTemplate`방법

3.  Atlas에 대해 살생 된 URI

4.  고객 이름













경고



<td class="content">내 하드 URL 매개 변수를 사용하지 마십시오`RestTemplate`.동적 엔드 포인트를 타겟팅 할 때 URL 변수를 사용합니다.이 문제 가능성 "에 도달 GC 오버 헤드 제한"피할`ServoMonitorCache`고유 키 각 URL을 처리합니다.













    // recommended
    String orderid = "1";
    restTemplate.getForObject("http://testeurekabrixtonclient/orders/{orderid}", String.class, orderid)

    // avoid
    restTemplate.getForObject("http://testeurekabrixtonclient/orders/1", String.class)









### 통계 수집 : 관중



구경꾼 통계를 사용하려면 종속성에 포함`spring-boot-starter-spectator`:







        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-spectator</artifactId>
        </dependency>







Spectator 용어에서 미터는 명명 된, 입력 된 및 태그가있는 구성이고 메트릭은 특정 시점의 주어진 미터의 값을 나타냅니다.관측기 미터는 현재 여러 가지 구현이있는 레지스트리에 의해 생성되고 제어됩니다.Spectator는 4 미터 유형을 제공합니다 : 카운터, 타이머, 게이지 및 분배 요약.





봄 구름 관객 통합은 주사 구성`com.netflix.spectator.api.Registry`당신을 위해 인스턴스를.구체적으로는 구성`ServoRegistry`REST 통계의 수집 및 하나의 서보 API에서 아틀라스 백엔드에 대한 메트릭의 수출을 통합하기 위해 인스턴스를.실제로,이 코드가 서보 모니터와 구경꾼 미터 모두 봄 부팅 액추에이터에 의해 훔쳐됩니다의 혼합물을 사용할 수 있다는 것을 의미`MetricReader`인스턴스와 모두 아틀라스 백엔드로 배송됩니다.





#### 관중 카운터



카운터는 일부 이벤트가 발생하는 비율을 측정하는 데 사용됩니다.







    // create a counter with a name and a set of tags
    Counter counter = registry.counter("counterName", "tagKey1", "tagValue1", ...);
    counter.increment(); // increment when an event occurs
    counter.increment(10); // increment by a discrete amount







카운터는 단일 시간 정규화 통계를 기록합니다.







#### 관중 타이머



타이머는 일부 이벤트가 얼마나 오래 걸리는지 측정하는 데 사용됩니다.봄 클라우드는 자동으로 조건부 스프링 MVC 요청과에 대한 타이머 기록`RestTemplate`후 대기 시간 등의 요청 관련 통계에 대한 대시 보드를 만들 수 있습니다 요청을 :





![RequestLatency](./spring-cloud-netflix-doc-images/RequestLatency.png)

그림 4\. 요청 대기 시간







    // create a timer with a name and a set of tags
    Timer timer = registry.timer("timerName", "tagKey1", "tagValue1", ...);

    // execute an operation and time it at the same time
    T result = timer.record(() -> fooReturnsT());

    // alternatively, if you must manually record the time
    Long start = System.nanoTime();
    T result = fooReturnsT();
    timer.record(System.nanoTime() - start, TimeUnit.NANOSECONDS);







타이머는 count, max, totalOfSquares 및 totalTime의 4 가지 통계를 동시에 기록합니다.카운트 통계는 항상 호출 한 경우 카운터에서 제공하는 하나의 정규화 된 값과 일치합니다`increment()`당신은 타이밍을 기록 할 때마다의 카운터에 한 번을, 그래서 하나의 작업에 대해 개별적으로 계산하고 시간에 거의 필요하지 않습니다.





들어[장기 실행 작업](https://github.com/Netflix/spectator/wiki/Timer-Usage#longtasktimer), 관객은 특별한을 제공합니다`LongTaskTimer`.







#### 스펙 테이터 게이지



게이지는 실행중인 상태의 대기열 또는 스레드 수와 같은 현재 값을 결정하는 데 사용됩니다.게이지는 샘플링되므로 샘플간에 이러한 값이 변동하는 방식에 대한 정보는 제공하지 않습니다.





게이지의 정상적인 사용에는 초기화시 ID, 샘플링 할 객체에 대한 참조, 객체를 기반으로 숫자 값을 가져 오거나 계산하는 함수를 사용하여 게이지를 등록하는 작업이 포함됩니다.객체에 대한 참조는 별도로 전달되며 Spectator 레지스트리는 객체에 대한 약한 참조를 유지합니다.객체가 가비지 수집 된 경우 Spectator는 자동으로 등록을 삭제합니다.참조[노트](https://github.com/Netflix/spectator/wiki/Gauge-Usage#using-lambda)이 API가 잘못 사용되는 경우 잠재적 메모리 누수에 대한 관객의 문서를.







    // the registry will automatically sample this gauge periodically
    registry.gauge("gaugeName", pool, Pool::numberOfRunningThreads);

    // manually sample a value in code at periodic intervals -- last resort!
    registry.gauge("gaugeName", Arrays.asList("tagKey1", "tagValue1", ...), 1000);









#### 관람객 분포 요약



분배 요약은 이벤트 분배를 추적하는 데 사용됩니다.이것은 타이머와 비슷하지만 크기가 일정 시간 일 필요는 없다는 점에서보다 일반적입니다.예를 들어, 분배 요약은 서버에 도달하는 요청의 페이로드 크기를 측정하는 데 사용될 수 있습니다.







    // the registry will automatically sample this gauge periodically
    DistributionSummary ds = registry.distributionSummary("dsName", "tagKey1", "tagValue1", ...);
    ds.record(request.sizeInBytes());











### 통계 수집 : 서보











경고



<td class="content">코드가 Java 8에서 컴파일 된 경우, 관측자로 Servo 대신 Spectator를 사용하면 장기간에 걸쳐 Servo를 완전히 대체 할 예정입니다.











Servo 구문에서 모니터는 명명 된 유형 지정 및 태그가 지정된 구성이며 메트릭은 특정 시점의 특정 모니터 값을 나타냅니다.서보 모니터는 관측기 미터와 논리적으로 동일합니다.서보 모니터 생성 및에 의해 제어된다`MonitorRegistry`.위의 경고에도 불구하고, 서보는 있는가[넓은 배열](https://github.com/Netflix/servo/wiki/Getting-Started)관객이 미터가보다 모니터 옵션을.





봄 클라우드 통합은 주사 구성`com.netflix.servo.MonitorRegistry`당신을 위해 인스턴스를.적절한 만든 후에`Monitor`서보의 유형을, 데이터를 기록하는 과정은 관객에 전적으로 유사하다.





#### 서보 모니터 만들기



당신은 서보 사용하는 경우`MonitorRegistry`(특히, 인스턴스 봄 클라우드에서 제공하는 인스턴스`DefaultMonitorRegistry`), 서보 검색 편의 클래스를 제공[카운터](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamiccounter)및[타이머를](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamictimer).이러한 편리한 클래스는 하나가되도록`Monitor`이름과 태그의 고유 한 각 조합에 등록됩니다.





수동으로, 특히 편리한 메소드가 제공되지 않은, 더 이국적인 모니터 유형, 서보의 모니터 유형을 만들 제공하여 적절한 유형의 인스턴스를`MonitorConfig`인스턴스를 :







    MonitorConfig config = MonitorConfig.builder("timerName").withTag("tagKey1", "tagValue1").build();

    // somewhere we should cache this Monitor by MonitorConfig
    Timer timer = new BasicTimer(config);
    monitorRegistry.register(timer);











### 메트릭 백엔드 : Atlas



Atlas는 Netflix에서 거의 실시간 운영 통찰력을위한 차원 시계열 데이터를 관리하기 위해 개발되었습니다.Atlas는 메모리 내 데이터 스토리지를 특징으로하며 매우 많은 수의 메트릭을 매우 신속하게 수집하고보고 할 수 있습니다.





Atlas는 운영 정보를 캡처합니다.비즈니스 인텔리전스는 추세 분석을 위해 수집 된 데이터이지만 운영 인텔리전스는 시스템 내에서 현재 일어나고있는 상황을 보여줍니다.





봄 클라우드가 제공하는`spring-cloud-starter-atlas`당신이 필요로하는 모든 종속성을 갖는다.그런 다음 귀하의 봄 부팅 응용 프로그램을 주석`@EnableAtlas`과와 실행 아틀라스 서버의 위치를 제공하는`netflix.atlas.uri`속성입니다.





#### 글로벌 태그



Spring Cloud를 사용하면 Atlas 백엔드로 전송되는 모든 메트릭에 태그를 추가 할 수 있습니다.글로벌 태그를 사용하여 애플리케이션 이름, 환경, 지역 등으로 측정 항목을 분리 할 수 ​​있습니다.





구현 각 콩`AtlasTagProvider`글로벌 태그 목록에 기여할 것입니다 :







    @Bean
    AtlasTagProvider atlasCommonTags(
        @Value("${spring.application.name}") String appName) {
      return () -> Collections.singletonMap("app", appName);
    }









#### Atlas 사용



인 - 메모리 독립형 Atlas 인스턴스를 부트 스트랩하려면 다음을 수행하십시오.







    $ curl -LO https://github.com/Netflix/atlas/releases/download/v1.4.2/atlas-1.4.2-standalone.jar
    $ java -jar atlas-1.4.2-standalone.jar















팁



<td class="content">r3.2xlarge (61GB RAM)에서 실행되는 Atlas 독립형 노드는 주어진 6 시간 동안 분당 약 2 백만 개의 메트릭을 처리 할 수 ​​있습니다.











일단 실행하고 몇 가지 메트릭을 수집했으면 Atlas 서버에 태그를 나열하여 설정이 올바른지 확인하십시오.







    $ curl http://ATLAS/api/v1/tags















팁



<td class="content">서비스에 대해 여러 요청을 실행 한 후 브라우저에 다음 URL을 붙여 넣어 요청의 대기 시간에 대한 몇 가지 기본적인 정보를 수집 할 수 있습니다.`[http://ATLAS/api/v1/graph?q=name,rest,:eq,:avg](http://atlas/api/v1/graph?q=name,rest,:eq,:avg)`











아틀라스 위키는 포함[샘플 쿼리의 편집](https://github.com/Netflix/atlas/wiki/Single-Line)다양한 시나리오를.





밖으로 확인하십시오[경고 철학](https://github.com/Netflix/atlas/wiki/Alerting-Philosophy)사용과 문서를[이중 지수 평활를](https://github.com/Netflix/atlas/wiki/DES)동적 경고 임계 값을 생성 할 수 있습니다.



















<div class="logo">![Google 번역](./spring-cloud-netflix-doc-images/translate_24dp.png)







# 원본 텍스트





<div class="original-text">Service Discovery is one of the key tenets of a microservice based architecture.









* * *





