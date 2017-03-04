
Spring Cloud
=============

# 원본
http://projects.spring.io/spring-cloud/spring-cloud.html

# 목차

*   [Features](http://projects.spring.io/spring-cloud/spring-cloud.html#_features)
*   [클라우드 네이티브 애플리케이션](http://projects.spring.io/spring-cloud/spring-cloud.html#_cloud_native_applications)
    *   [Spring Cloud Context : 애플리케이션 컨텍스트 서비스](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_context_application_context_services)
        *   [부트 스트랩 응용 프로그램 컨텍스트](http://projects.spring.io/spring-cloud/spring-cloud.html#_the_bootstrap_application_context)
        *   [응용 프로그램 컨텍스트 계층 구조](http://projects.spring.io/spring-cloud/spring-cloud.html#_application_context_hierarchies)
        *   [부트 스트랩 속성 위치 변경](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-properties)
        *   [부트 스트랩 구성 사용자 정의](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_bootstrap_configuration)
        *   [부트 스트랩 속성 소스 사용자 정의](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-property-sources)
        *   [환경 변화](http://projects.spring.io/spring-cloud/spring-cloud.html#_environment_changes)
        *   [새로 고침 범위](http://projects.spring.io/spring-cloud/spring-cloud.html#_refresh_scope)
        *   [암호화 및 암호 해독](http://projects.spring.io/spring-cloud/spring-cloud.html#_encryption_and_decryption)
        *   [종점](http://projects.spring.io/spring-cloud/spring-cloud.html#_endpoints)
    *   [Spring Cloud Commons : 공통 추상화](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_commons_common_abstractions)
        *   [로드 밸런서 클라이언트로서의 Spring RestTemplate](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_resttemplate_as_a_load_balancer_client)
        *   [여러 개의 RestTemplate 객체](http://projects.spring.io/spring-cloud/spring-cloud.html#_multiple_resttemplate_objects)
        *   [네트워크 인터페이스 무시](http://projects.spring.io/spring-cloud/spring-cloud.html#ignore-network-interfaces)
*   [스프링 클라우드 구성](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_config)
    *   [빠른 시작](http://projects.spring.io/spring-cloud/spring-cloud.html#_quick_start)
        *   [클라이언트 측 사용](http://projects.spring.io/spring-cloud/spring-cloud.html#_client_side_usage)
    *   [Spring Cloud 구성 서버](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_config_server)
        *   [환경 저장소](http://projects.spring.io/spring-cloud/spring-cloud.html#_environment_repository)
        *   [건강 지표](http://projects.spring.io/spring-cloud/spring-cloud.html#_health_indicator)
        *   [보안](http://projects.spring.io/spring-cloud/spring-cloud.html#_security)
        *   [암호화 및 암호 해독](http://projects.spring.io/spring-cloud/spring-cloud.html#_encryption_and_decryption_2)
        *   [키 관리](http://projects.spring.io/spring-cloud/spring-cloud.html#_key_management)
        *   [테스트 용 키 저장소 만들기](http://projects.spring.io/spring-cloud/spring-cloud.html#_creating_a_key_store_for_testing)
        *   [여러 키 및 키 회전 사용](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_multiple_keys_and_key_rotation)
    *   [일반 텍스트 검색](http://projects.spring.io/spring-cloud/spring-cloud.html#_serving_plain_text)
    *   [구성 서버 포함](http://projects.spring.io/spring-cloud/spring-cloud.html#_embedding_the_config_server)
    *   [푸시 알림 및 스프링 클라우드 버스](http://projects.spring.io/spring-cloud/spring-cloud.html#_push_notifications_and_spring_cloud_bus)
    *   [Spring Cloud 구성 클라이언트](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_config_client)
        *   [첫 번째 부트 스트랩 구성](http://projects.spring.io/spring-cloud/spring-cloud.html#config-first-bootstrap)
        *   [유레카 퍼스트 부트 스트랩](http://projects.spring.io/spring-cloud/spring-cloud.html#eureka-first-bootstrap)
        *   [구성 클라이언트 실패 빠른](http://projects.spring.io/spring-cloud/spring-cloud.html#config-client-fail-fast)
        *   [구성 클라이언트 재시도](http://projects.spring.io/spring-cloud/spring-cloud.html#config-client-retry)
        *   [원격 구성 리소스 찾기](http://projects.spring.io/spring-cloud/spring-cloud.html#_locating_remote_configuration_resources)
        *   [보안](http://projects.spring.io/spring-cloud/spring-cloud.html#_security_2)
*   [Spring Cloud 넷플 릭스](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_netflix)
    *   [서비스 발견 : 유레카 클라이언트](http://projects.spring.io/spring-cloud/spring-cloud.html#_service_discovery_eureka_clients)
        *   [유레카 등록](http://projects.spring.io/spring-cloud/spring-cloud.html#_registering_with_eureka)
        *   [상태 페이지 및 상태 표시기](http://projects.spring.io/spring-cloud/spring-cloud.html#_status_page_and_health_indicator)
        *   [보안 응용 프로그램 등록](http://projects.spring.io/spring-cloud/spring-cloud.html#_registering_a_secure_application)
        *   [유레카 건강 검사](http://projects.spring.io/spring-cloud/spring-cloud.html#_eureka_s_health_checks)
        *   [인스턴스 및 클라이언트에 대한 유레카 메타 데이터](http://projects.spring.io/spring-cloud/spring-cloud.html#_eureka_metadata_for_instances_and_clients)
        *   [EurekaClient 사용](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_the_eurekaclient)
        *   [기본 Netflix EurekaClient의 대안](http://projects.spring.io/spring-cloud/spring-cloud.html#_alternatives_to_the_native_netflix_eurekaclient)
        *   [서비스 등록이 너무 느린 이유는 무엇입니까?](http://projects.spring.io/spring-cloud/spring-cloud.html#_why_is_it_so_slow_to_register_a_service)
    *   [서비스 발견 : 유레카 서버](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-eureka-server)
        *   [고 가용성, 영역 및 영역](http://projects.spring.io/spring-cloud/spring-cloud.html#_high_availability_zones_and_regions)
        *   [독립 실행 형 모드](http://projects.spring.io/spring-cloud/spring-cloud.html#_standalone_mode)
        *   [또래 인식](http://projects.spring.io/spring-cloud/spring-cloud.html#_peer_awareness)
        *   [IP 주소 선호](http://projects.spring.io/spring-cloud/spring-cloud.html#_prefer_ip_address)
    *   [회로 차단기 : Hystrix 클라이언트](http://projects.spring.io/spring-cloud/spring-cloud.html#_circuit_breaker_hystrix_clients)
        *   [보안 컨텍스트 전파 또는 스프링 스코프 사용](http://projects.spring.io/spring-cloud/spring-cloud.html#_propagating_the_security_context_or_using_spring_scopes)
        *   [건강 지표](http://projects.spring.io/spring-cloud/spring-cloud.html#_health_indicator_2)
        *   [Hystrix 메트릭스 스트림](http://projects.spring.io/spring-cloud/spring-cloud.html#_hystrix_metrics_stream)
    *   [회로 차단기 : Hystrix 대시 보드](http://projects.spring.io/spring-cloud/spring-cloud.html#_circuit_breaker_hystrix_dashboard)
        *   [터빈](http://projects.spring.io/spring-cloud/spring-cloud.html#_turbine)
        *   [터빈 AMQP](http://projects.spring.io/spring-cloud/spring-cloud.html#_turbine_amqp)
    *   [AMQP ConnectionFactory 사용자 정의](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_amqp_connectionfactory)
    *   [클라이언트 측로드 밸런서 : 리본](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon)
        *   [리본 클라이언트 사용자 정의](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_ribbon_client)
        *   [유레카와 함께 리본 사용하기](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_ribbon_with_eureka)
        *   [예 : 유레카가없는 리본 사용법](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon-without-eureka)
        *   [예 : 리본에서 유레카 사용을 비활성화합니다.](http://projects.spring.io/spring-cloud/spring-cloud.html#_example_disable_eureka_use_in_ribbon)
        *   [리본 API를 직접 사용](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_the_ribbon_api_directly)
    *   [선언적 REST 클라이언트 : Feign](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign)
        *   [기본 값 재정의](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-overriding-defaults)
        *   [Hystrix 지원 지원](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-hystrix)
        *   [Hystrix Fallbacks를 기쁘게합니다.](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-hystrix-fallback)
        *   [기꺼이 상속 지원](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-inheritance)
        *   [희망 요청 / 응답 압축](http://projects.spring.io/spring-cloud/spring-cloud.html#_feign_request_response_compression)
        *   [벌채 로깅](http://projects.spring.io/spring-cloud/spring-cloud.html#_feign_logging)
    *   [외부 구성 : Archaius](http://projects.spring.io/spring-cloud/spring-cloud.html#_external_configuration_archaius)
    *   [라우터 및 필터 : Zuul](http://projects.spring.io/spring-cloud/spring-cloud.html#_router_and_filter_zuul)
        *   [임베디드 Zuul 역방향 프록시](http://projects.spring.io/spring-cloud/spring-cloud.html#netflix-zuul-reverse-proxy)
        *   [교살 패턴과 로컬 전달](http://projects.spring.io/spring-cloud/spring-cloud.html#_strangulation_patterns_and_local_forwards)
        *   [Zuul을 통한 파일 업로드](http://projects.spring.io/spring-cloud/spring-cloud.html#_uploading_files_through_zuul)
        *   [Plain Embedded Zuul](http://projects.spring.io/spring-cloud/spring-cloud.html#_plain_embedded_zuul)
        *   [주울 필터 사용 안 함](http://projects.spring.io/spring-cloud/spring-cloud.html#_disable_zuul_filters)
        *   [사이드카로 다국어 지원](http://projects.spring.io/spring-cloud/spring-cloud.html#_polyglot_support_with_sidecar)
    *   [통계 : 관중, 서보 및지도](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_spectator_servo_and_atlas)
        *   [차원 대 계층 적 메트릭 비교](http://projects.spring.io/spring-cloud/spring-cloud.html#_dimensional_vs_hierarchical_metrics)
        *   [기본 메트릭 컬렉션](http://projects.spring.io/spring-cloud/spring-cloud.html#_default_metrics_collection)
        *   [통계 수집 : 관중](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_collection_spectator)
        *   [통계 수집 : 서보](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_collection_servo)
        *   [메트릭 백엔드 : Atlas](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_backend_atlas)
*   [스프링 클라우드 버스](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_bus)
    *   [빠른 시작](http://projects.spring.io/spring-cloud/spring-cloud.html#_quick_start_2)
    *   [인스턴스 주소 지정](http://projects.spring.io/spring-cloud/spring-cloud.html#_addressing_an_instance)
    *   [서비스의 모든 인스턴스 주소 지정](http://projects.spring.io/spring-cloud/spring-cloud.html#_addressing_all_instances_of_a_service)
    *   [응용 프로그램 컨텍스트 ID는 고유해야합니다.](http://projects.spring.io/spring-cloud/spring-cloud.html#_application_context_id_must_be_unique)
    *   [메시지 브로커 사용자 정의](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_message_broker)
    *   [추적 버스 이벤트](http://projects.spring.io/spring-cloud/spring-cloud.html#_tracing_bus_events)
*   [스프링 부트 클라우드 CLI](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_boot_cloud_cli)
    *   [설치](http://projects.spring.io/spring-cloud/spring-cloud.html#_installation)
    *   [Groovy 스크립트 작성 및 응용 프로그램 실행](http://projects.spring.io/spring-cloud/spring-cloud.html#_writing_groovy_scripts_and_running_applications)
    *   [암호화 및 암호 해독](http://projects.spring.io/spring-cloud/spring-cloud.html#_encryption_and_decryption_3)
*   [스프링 클라우드 보안](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_security)
    *   [빠른 시작](http://projects.spring.io/spring-cloud/spring-cloud.html#_quickstart)
        *   [OAuth2 싱글 사인온](http://projects.spring.io/spring-cloud/spring-cloud.html#_oauth2_single_sign_on)
        *   [OAuth2 보호 된 리소스](http://projects.spring.io/spring-cloud/spring-cloud.html#_oauth2_protected_resource)
    *   [상세 정보](http://projects.spring.io/spring-cloud/spring-cloud.html#_more_detail)
        *   [단일 사인온](http://projects.spring.io/spring-cloud/spring-cloud.html#_single_sign_on)
        *   [토큰 중계](http://projects.spring.io/spring-cloud/spring-cloud.html#_token_relay)
    *   [Zuul 프록시의 인증 다운 스트림 구성](http://projects.spring.io/spring-cloud/spring-cloud.html#_configuring_authentication_downstream_of_a_zuul_proxy)






# Spring Cloud
-----

Spring Cloud는 개발자가 분산 시스템 (예 : 구성 관리, 서비스 발견, 회로 차단기, 지능형 라우팅, 마이크로 프록시, 제어 버스, 일회성 토큰, 글로벌 잠금, 리더십 선거, 분산 등)에서 공통 패턴을 신속하게 구축 할 수있는 도구를 제공합니다. 세션, 클러스터 상태). 분산 시스템을 조정하면 보일러 플레이트 패턴이 생기고 Spring Cloud 개발자는 이러한 패턴을 구현하는 서비스와 애플리케이션을 신속하게 구현할 수 있습니다. 개발자의 자체 랩톱, 베어 메탈 (bare metal) 데이터 센터 및 Cloud Foundry와 같은 관리 플랫폼을 포함한 모든 분산 환경에서 잘 작동합니다.









## Features





Spring Cloud는 전형적인 유스 케이스에 대해 좋은 아웃 오브 박스 경험을 제공하고 다른 사람들을 포괄하는 확장 성 메커니즘에 중점을 둡니다.





*   분산 / 버전 관리 된 구성

*   서비스 등록 및 검색

*   라우팅

*   서비스 대 서비스 호출

*   로드 균형 조정

*   회로 차단기

*   전역 잠금

*   지도력 선거 및 클러스터 상태

*   분산 메시징







# 클라우드 네이티브 애플리케이션







[클라우드 네이티브](https://pivotal.io/platform-as-a-service/migrating-to-cloud-native-application-architectures-ebook) 연속 배달과 가치 중심의 개발 분야에서 모범 사례를 쉽게 채택을 장려 응용 프로그램 개발의 스타일입니다. 관련 분야는 건물입니다 [12 인자 앱](http://12factor.net/) 개발 사례가 선언적 프로그래밍과 관리 및 모니터링을 사용하여 예를 들어, 배달 및 운영 목적에 부합되는합니다. 스프링 클라우드는 여러 가지 특정 방식으로 이러한 스타일의 개발을 용이하게하며 출발점은 분산 시스템의 모든 구성 요소가 필요할 때 쉽게 액세스 할 수 있거나 필요로하는 기능 집합입니다.





이러한 기능의 대부분은에 의해 보호됩니다 [봄 부트](http://projects.spring.io/spring-boot) 우리가 봄 클라우드에 구축. Spring Cloud에서는 두 가지 라이브러리 인 Spring Cloud Context와 Spring Cloud Commons를 제공합니다. 봄 클라우드 컨텍스트 유틸리티 및 특별 서비스에 대한 제공 `ApplicationContext`스프링 클라우드 응용 프로그램 (부트 스트랩 상황, 암호화, 범위 및 환경 엔드 포인트를 새로 고침). Spring Cloud Commons는 다른 Spring Cloud 구현 (예 : Spring Cloud Netflix 대 Spring Cloud Consul)에서 사용되는 추상화 및 공통 클래스 세트입니다.





"잘못된 키 크기"로 인해 예외가 발생하고 Sun의 JDK를 사용하는 경우 JCE (Java Cryptography Extension) 무제한 강도 관할 정책 파일을 설치해야합니다. 자세한 내용은 다음 링크를 참조하십시오.





*   [Java 6 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-6-download-429243.html)

*   [Java 7 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html)

*   [Java 8 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html)





JDK / jre / lib / security 폴더 (사용중인 JRE / JDK x64 / x86 버전)로 파일을 추출하십시오.













노트



Spring Cloud는 비 제한적 Apache 2.0 라이센스에 따라 출시되었습니다. 문서의이 섹션에 기여하고 싶거나 오류가 발견되면 {githubmaster} / docs / src / main / asciidoc [github]에서 프로젝트의 소스 코드와 이슈 트래커를 찾으십시오.












## Spring Cloud Context : 애플리케이션 컨텍스트 서비스





Spring Boot는 일반적인 구성 파일을위한 전통적인 위치와 일반적인 관리 및 모니터링 작업을위한 끝점을 가지고있는 Spring을 사용하여 응용 프로그램을 빌드하는 방법에 대한 의견이 많습니다. Spring Cloud는이를 기반으로 시스템의 모든 구성 요소가 사용하거나 필요로하는 기능을 추가합니다.





### 부트 스트랩 응용 프로그램 컨텍스트



Spring Cloud 애플리케이션은 메인 애플리케이션의 상위 컨텍스트 인 "부트 스트랩"컨텍스트를 작성하여 작동합니다. 외부에서 가져온 구성 파일은 외부 소스의 구성 등록 정보로드 및 로컬 외부 구성 파일의 등록 정보 해독을 담당합니다. 두 컨텍스트가 공유 `Environment` 하는 모든 Spring 애플리케이션을위한 외부 속성의 소스입니다. 부트 스트랩 특성은 우선 순위가 높으므로 추가되어 로컬 구성으로 대체 될 수 없습니다.





부트 스트랩 상황은 그렇게하는 대신, 주요 애플리케이션 컨텍스트보다 외부 구성을 찾기위한 다른 규칙을 사용 `application.yml`(또는 `.properties`) 사용 `bootstrap.yml`, 부트 스트랩 및 주요 상황에 대한 외부 구성을 유지하는 것은 잘 구분합니다. 예:





bootstrap.yml



<pre>봄:
  신청:
    이름 : foo
  구름:
    config :
      uri : $ {SPRING_CONFIG_URI : http : // localhost : 8888}</pre>







설정하는 것이 좋습니다 `spring.application.name`(에서 `bootstrap.yml`또는 `application.yml`응용 프로그램이 서버에서 모든 응용 프로그램 별 구성을 필요로하는 경우).





당신은 설정하여 완전히 부트 스트랩 프로세스를 비활성화 할 수 있습니다 `spring.cloud.bootstrap.enabled=false`(시스템 등록 정보에서 예를 들면).







### 응용 프로그램 컨텍스트 계층 구조



당신이에서 응용 프로그램 컨텍스트를 빌드하는 경우 `SpringApplication`또는 `SpringApplicationBuilder`, 다음 부트 스트랩 컨텍스트는 해당 컨텍스트에 대한 부모로 추가됩니다. 하위 컨텍스트가 부모로부터 속성 소스와 프로파일을 상속받는 것은 Spring의 기능이므로 "기본"응용 프로그램 컨텍스트에는 Spring Cloud Config없이 동일한 컨텍스트를 작성하는 것과 비교하여 추가 속성 소스가 포함됩니다. 추가 속성 소스는 다음과 같습니다.





*   (선택 사양)가 "부트 스트랩" `CompositePropertySource`어떤 경우 높은 우선 순위로 나타납니다 `PropertySourceLocators`부트 스트랩 컨텍스트에서 찾을 수 있습니다, 그들은 비어 있지 않은 특성을 갖는다. 한 예로 Spring Cloud Config Server의 특성이있다. 참조 [아래](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-property-sources) 이 속성 소스의 내용을 사용자 정의하는 방법에 대한 지침.

*   "applicationConfig : [classpath : bootstrap.yml]"(스프링 프로파일이 활성화 된 경우 친구). 만약 가지고 있다면 `bootstrap.yml`(또는 특성) 다음, 이러한 특성은 부트 스트랩 컨텍스트를 구성하는 데 사용되며, 그 부모가 설정되어있을 때 그들은 자식 콘텍스트에 첨가하자. 그들은보다 낮은 우선 순위가 `application.yml`(또는 속성)과 봄 부팅 응용 프로그램을 만드는 과정의 정상적인 부분으로 아이에 추가 된 다른 재산 소스를. 참조 [아래에](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-properties) 이러한 속성 소스의 내용을 사용자 정의하는 방법에 대한 지침.





때문에 "부트 스트랩"항목을 우선하지만, 이들로부터 데이터를 포함하지 않는다는 것을 유의 속성 소스의 순서의 규칙 `bootstrap.yml`이 매우 낮은 우선 순위를 갖는, 그러나 기본값을 설정하는데 사용될 수있다.





당신은 단순히 어떤의 부모 컨텍스트 설정하여 상황에 맞는 계층 구조를 확장 할 수 있습니다 `ApplicationContext`, 또는 함께 자신의 인터페이스를 사용하여 생성을, 예를 들면 `SpringApplicationBuilder`편리한 메소드 ( `parent()`, `child()`과 `sibling()`). 부트 스트랩 컨텍스트는 직접 만든 상위 선조의 부모가됩니다. 계층 구조의 모든 컨텍스트는 부울에서 자손으로 부주의하게 값을 승격시키는 것을 피하기 위해 자체 "부트 스트랩"속성 소스 (비어 있음)를 갖습니다. 계층 구조의 모든 상황은 (원칙적으로) 다른 가질 수 `spring.application.name`구성 서버가있는 경우, 따라서 다른 원격 속성 소스를. 일반 Spring 애플리케이션 컨텍스트 동작 규칙은 속성 확인에 적용됩니다. 하위 컨텍스트의 속성은 부모의 속성, 이름 및 속성 소스 이름을 우선합니다 (자식이 부모와 같은 이름을 가진 속성 소스를 가지면 부모는 자녀에게 포함되어 있지 않습니다).





(가) 있습니다 `SpringApplicationBuilder`당신이를 공유 할 수 있습니다 `Environment`전체 계층 사이,하지만 그 기본이 아니다. 따라서 특히 형제 상황은 부모와 공통된 사항을 공유 할지라도 동일한 프로필 또는 속성 소스를 가질 필요가 없습니다.







### 부트 스트랩 속성 위치 변경



`bootstrap.yml`(또는 `.properties`) 위치를 사용하여 지정할 수 있습니다 `spring.cloud.bootstrap.name`(기본 "부트 스트랩") 또는 `spring.cloud.bootstrap.location`시스템 등록 정보에서 예 (기본 빈을). 이러한 속성은 같이 행동 `spring.config.*` 들이 부트 스트랩을 설정하는 데 사용되는 사실, 같은 이름을 가진 변종 `ApplicationContext`는 이들 속성을 설정하여 `Environment`. (에서 활성 프로파일이있는 경우 `spring.profiles.active`또는를 통해 `Environment`해당 프로파일의 특성 그냥 일반 봄 부팅 응용 프로그램, 예에서처럼,뿐만 아니라로드됩니다 당신이 구축하고있는 상황에서 API) `bootstrap-development.properties`는 "개발"프로필은.







### 부트 스트랩 구성 사용자 정의



부트 스트랩 컨텍스트는 당신이 항목을 추가하여 원하는 무엇이든 할 수 있도록 훈련 할 수있다 `/META-INF/spring.factories`키 아래를 `org.springframework.cloud.bootstrap.BootstrapConfiguration`. 이 봄의 쉼표로 구분 된 목록입니다 `@Configuration`컨텍스트를 만드는 데 사용되는 클래스. 당신이에서 autowiring을위한 주요 애플리케이션 컨텍스트에 사용할 수있게하려면 모든 빈은 여기에 작성하고, 또한위한 특별한 계약이 될 수있는 `@Beans`유형의 `ApplicationContextInitializer`. 클래스가 표시 될 수 `@Order` 는 시동 순서를 제어하려는 경우 (기본 순서는 "마지막")입니다.













경고



사용자를 추가 할 때주의해야합니다 `BootstrapConfiguration`추가 클래스가 아니라는 것을 `@ComponentScanned`그들이 필요되지 않을 수 있습니다 귀하의 "주"응용 프로그램 컨텍스트에 실수로. 이미이 적용되지 않습니다 부팅 구성 클래스에 대한 별도의 패키지 이름을 사용 `@ComponentScan`또는 `@SpringBootApplication` 주석 구성 클래스.











부트 스트랩 프로세스는 메인에 이니셜을 주입하여 종료 `SpringApplication`(그것은 독립 실행 형 응용 프로그램으로 실행 또는 응용 프로그램 서버에 배포되어 있는지 여부, 즉 정상적인 봄 부팅 시동 순서) 예. 먼저 부트 스트랩 컨텍스트 검색된 클래스로부터 생성 `spring.factories`하고 모든 `@Beans`형태의 `ApplicationContextInitializer`기본에 첨가 `SpringApplication`가 시작되기 전에.







### 부트 스트랩 속성 소스 사용자 정의



부트 스트랩 프로세스에 의해 추가 된 외부 구성의 기본 속성 소스는 구성 서버,하지만 당신은 종류의 콩을 추가하여 추가 소스를 추가 할 수 있습니다 `PropertySourceLocator`부트 스트랩 컨텍스트 (비아 `spring.factories`). 이 기능을 사용하여 다른 서버 또는 데이터베이스와 같은 추가 속성을 삽입 할 수 있습니다.





예를 들어, 다음과 같은 사소한 사용자 정의 위치 지정자를 고려하십시오.







    @Configuration
    public class CustomPropertySourceLocator implements PropertySourceLocator {

        @Override
        public PropertySource<?> locate(Environment environment) {
            return new MapPropertySource("customProperty",
                    Collections.<String, Object>singletonMap("property.from.sample.custom.source", "worked as intended"));
        }

    }







`Environment`전달되는이의 하나입니다 `ApplicationContext`우리가 추가 속성 소스를 공급하는 일, 즉 생성되는 약. 이 특정 속성 소스의 위치를들을 사용할 수 있도록 이미, 정상 봄 부트가 제공하는 속성 소스가됩니다 `Environment`합니다 (에 키잉에 의해 예를 `spring.application.name`기본 구성 서버 속성 소스 로케이터 에서처럼).





당신이이 클래스와 항아리를 만들 경우 다음 추가 `META-INF/spring.factories`함유 :







<pre>org.springframework.cloud.bootstrap.BootstrapConfiguration = sample.custom.CustomPropertySourceLocator</pre>







다음 "customProperty은" `PropertySource`그 클래스 패스에 그 항아리를 포함하는 모든 응용 프로그램에 표시됩니다.







### 환경 변화



어플리케이션이 청취 할 `EnvironmentChangedEvent`및 (추가 표준 몇 가지 방법의 변화에 반응하여 `ApplicationListeners`첨가 할 수있다 `@Beans`일반적인 방법은 사용자에 의해). 이 때 `EnvironmentChangedEvent`관찰이 변경된 키 값의 목록이되며, 응용 프로그램에 사람들을 사용합니다 :





*   모든 다시 결합 `@ConfigurationProperties`맥락에서 콩을

*   모든 속성에 대한 로거 수준 설정 `logging.level.*`





는 config 클라이언트는 변화에 대한 기본 조사로하지 않습니다 `Environment`, 그리고 (당신이 그것을 설정할 수 있지만, 일반적으로 우리는 변화를 검출하는 방법을 권하고 싶지 않다 `@Scheduled`주석). 그런 다음 축소 아웃 클라이언트 응용 프로그램이있는 경우는 방송을하는 것이 좋습니다 `EnvironmentChangedEvent`(예를 사용하여 그들에게 변화에 대한 폴링을하는 대신 모든 인스턴스에 [봄 클라우드 버스](https://github.com/spring-cloud/spring-cloud-bus) ).





는 `EnvironmentChangedEvent`만큼 당신이 실제로 변경을 할 수있는, 새로 고침 사용 사례의 큰 클래스를 포함 `Environment` 하고 이벤트를 (그 API를 공개하고 핵심 봄의 일부)에 게시합니다. 당신은 변경에 바인딩 확인할 수 있습니다 `@ConfigurationProperties`방문하여 콩 `/configprops` 엔드 포인트 (정상 봄 부팅 액추에이터 기능). 예를 들어이 `DataSource`그 한 수 `maxPoolSize`런타임에 변경 (기본 `DataSource`봄 부팅에 의해 만들어진이입니다 `@ConfigurationProperties`콩)와 동적으로 용량을 증가. 다시 결합 `@ConfigurationProperties`하면 새로 고침보다 효율적으로 관리가 필요 사용 사례의 또 다른 큰 클래스를 포함하지 않으며, 당신은 변화를 필요로하는 곳에 전체에 걸쳐 원자 수 `ApplicationContext`. 우리가 그 문제를 해결합니다 `@RefreshScope`.







### 새로 고침 범위



봄 `@Bean`으로 표시된 `@RefreshScope`구성 변경이있는 경우 특별한 치료를 받게됩니다. 이는 초기화 될 때만 구성을 주입시키는 상태 보존빈의 문제점을 해결합니다. 예를 들어이 경우 `DataSource`데이터베이스 URL을 통해 변경 열려있는 연결을 가지고 `Environment`, 우리는 아마 그 연결의 소유자들이 무슨 일을 완료 할 수 있어야합니다. 그런 다음 누군가 다음에 풀에서 연결을 빌리면 새 URL로 연결됩니다.





새로 고침 범위 Bean은 사용시 (즉, 메서드가 호출 될 때) 초기화되는 지연 프록시이며 범위는 초기화 된 값의 캐시로 작동합니다. 빈이 다음 메소드 호출시 다시 초기화되도록하려면 캐시 항목을 무효화하면됩니다.





는 `RefreshScope`문맥에 콩이며 공개 방법이 `refreshAll()`대상 캐시를 삭제하여 범위에있는 모든 콩을 새로 고칠 수 있습니다. 도 있습니다 `refresh(String)`이름하여 개별 빈을 새로 고칠 수있는 방법은. 이 기능은 노출되어있다 `/refresh`(HTTP 또는 JMX를 통해) 엔드 포인트.













노트



`@RefreshScope`온 (기술적으로) 작동 `@Configuration` 클래스,하지만 놀라운 동작이 발생할 수 있습니다 : 그것은 않습니다 예를 들어 **하지** 모든 것을 의미 `@Beans`클래스에 정의 자체입니다 `@RefreshScope`. 특히, 새로 고침이 시작될 때 자체를하지 않는 한 그들에 의존 할 수 그 콩에 따라 달라 아무것도, 업데이트되고 `@RefreshScope`있는이 새로 고침에 재건되고 종속성이 시점에서 그들은 다시 될 것입니다, 재 주입 ( 새로 고친에서 초기화 `@Configuration`).













### 암호화 및 암호 해독



구성 클라이언트는이 `Environment`로컬 속성 값을 해독하기위한 사전 프로세서를. 이것은 서버 구성과 동일한 룰을 따르며, 비아 같은 외부 구성을 갖는다 `encrypt.*`. 따라서 당신은 형태로 암호화 된 값을 사용할 수 있습니다 `{cipher}*`주 응용 프로그램 컨텍스트를 취득하기 전에 다음 암호가 해독됩니다 유효한 키가있는만큼하고 `Environment`. 클라이언트에서 암호화 기능을 사용하려면 Classpath에 Spring Security RSA (Maven이 "org.springframework.security : spring-security-rsa"를 조정)를 포함시켜야하며 JVM에서 강력한 JCE 확장 기능이 필요합니다.





"잘못된 키 크기"로 인해 예외가 발생하고 Sun의 JDK를 사용하는 경우 JCE (Java Cryptography Extension) 무제한 강도 관할 정책 파일을 설치해야합니다. 자세한 내용은 다음 링크를 참조하십시오.





*   [Java 6 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-6-download-429243.html)

*   [Java 7 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html)

*   [Java 8 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html)





JDK / jre / lib / security 폴더 (사용중인 JRE / JDK x64 / x86 버전)로 파일을 추출하십시오.







### 종점



스프링 부트 액츄에이터 애플리케이션에는 몇 가지 추가 관리 엔드 포인트가 있습니다.





*   POST는 다음의 제품에 `/env`를 업데이트 `Environment`하고 바인딩 `@ConfigurationProperties`과 수준을 기록

*   `/refresh`에 대한 부트 스트랩 컨텍스트를 다시로드하고 상쾌한 `@RefreshScope`콩

*   `/restart`을 폐쇄 `ApplicationContext`하고 다시 시작합니다 (기본적으로 비활성화)

*   `/pause`및 `/resume`호출을위한 `Lifecycle`방법 ( `stop()`및 `start()`온 `ApplicationContext`)











## Spring Cloud Commons : 공통 추상화





서비스 발견,로드 밸런싱 및 회로 차단기와 같은 패턴은 모든 Spring Cloud 클라이언트가 구현과 독립적 (예 : Eureka 또는 Consul을 통한 검색) 할 수있는 공통적 인 추상화 계층에 적합합니다.





### 로드 밸런서 클라이언트로서의 Spring RestTemplate



당신은 자동 구성된 통해 간접적으로 리본을 사용할 수 있습니다 `RestTemplate` RestTemplate 클래스 경로에와 때 `LoadBalancerClient`) bean이 정의된다 :







    public class MyClass {
        @Autowired
        private RestTemplate restTemplate;

        public String doOtherStuff() {
            String results = restTemplate.getForObject("http://stores/stores", String.class);
            return results;
        }
    }







URI는 가상 호스트 이름 (예 : 호스트 이름이 아닌 서비스 이름)을 사용해야합니다. 리본 클라이언트는 전체 실제 주소를 만드는 데 사용됩니다. 참조 [RibbonAutoConfiguration을](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/ribbon/RibbonAutoConfiguration.java) 이 방법에 대한 자세한 내용은 `RestTemplate`설정되어 있습니다.







### 여러 개의 RestTemplate 객체



당신이 원하는 경우 `RestTemplate`부하 분산되지 않도록를하는 생성 `RestTemplate` 빈을 정상으로 주입. 균형 하중에 액세스하려면 `RestTemplate use the provided `@LoadBalanced` `Qualifier`:







    public class MyClass {
        @Autowired
        private RestTemplate restTemplate;

        @Autowired
        @LoadBalanced
        private RestTemplate loadBalanced;

        public String doOtherStuff() {
            return loadBalanced.getForObject("http://stores/stores", String.class);
        }

        public String doStuff() {
            return restTemplate.getForObject("http://example.com", String.class);
        }
    }









### 네트워크 인터페이스 무시



때로는 특정 명명 된 네트워크 인터페이스를 무시하여 서비스 검색 등록 (예 : Docker 컨테이너에서 실행)에서 제외 할 수있는 경우가 있습니다. 원하는 네트워크 인터페이스가 무시되도록하는 정규식 목록을 설정할 수 있습니다. 다음 구성은 "docker0"인터페이스와 "veth"로 시작하는 모든 인터페이스를 무시합니다.





application.yml



<pre>봄:
  구름:
    inetutils :
      ignoredInterfaces :
        - 도커 0
        - 베스. *</pre>











# 스프링 클라우드 구성



Spring Cloud Config는 분산 시스템에서 외부화 된 구성에 대한 서버 및 클라이언트 측 지원을 제공합니다. 구성 서버를 사용하면 모든 환경에서 응용 프로그램의 외부 속성을 중앙에서 관리 할 수 ​​있습니다. 동일 봄에 클라이언트 및 서버지도의 개념 `Environment`과 `PropertySource`추상화, 그들은 봄 응용 프로그램과 잘 맞는, 그러나 어떤 응용 프로그램이 모든 언어에서 실행에 사용할 수 있도록. 응용 프로그램이 개발 파이프 라인을 통해 개발자에서 테스트 및 프로덕션 환경으로 이동하면 해당 환경 간의 구성을 관리 할 수 ​​있으며 응용 프로그램이 마이그레이션 할 때 실행하는 데 필요한 모든 기능을 갖추고 있는지 확인할 수 있습니다. 서버 저장 장치 백엔드의 기본 구현은 git을 사용하므로 구성 환경의 레이블링 된 버전을 쉽게 지원할뿐만 아니라 컨텐츠 관리를위한 다양한 툴링에 액세스 할 수 있습니다. 대체 구현을 추가하고 Spring 구성으로 플러그인을 쉽게 삽입 할 수 있습니다.





## 빠른 시작





서버를 시작하십시오.







<pre>$ cd spring-cloud-config-server
$ mvn spring-boot : 실행</pre>







당신은 당신이 (메인 클래스가 선호하는 대신 경우 IDE에서 실행할 수 있도록 서버는 봄 부팅 응용 프로그램입니다 `ConfigServerApplication`). 그런 다음 클라이언트를 사용해보십시오.







<pre>$ curl localhost : 8888 / foo / development
{ "name": "development", "label": "master", "propertySources": [
  { "name": "https://github.com/scratches/config-repo/foo-development.properties", "source": { "bar": "spam"}}
  { "name": "https://github.com/scratches/config-repo/foo.properties", "source": { "foo": "bar"}}
]}</pre>







속성 소스의 위치에 대한 기본 전략 (에 자식 저장소를 복제하는 것입니다 `spring.cloud.config.server.git.uri`)와 미니를 초기화하는 데 사용 `SpringApplication`. 미니 응용 프로그램의 `Environment`속성 소스를 열거하고 JSON 엔드 포인트를 통해 게시하는 데 사용됩니다.





HTTP 서비스에는 다음과 같은 형식의 자원이 있습니다.







<pre>/ {application} / {profile} [/ {label}]
/{application}-{profile}.yml
/{label}/{application}-{profile}.yml
/{application}-{profile}.properties
/{label}/{application}-{profile}.properties</pre>







은 "응용 프로그램"으로 주입되는 곳 `spring.config.name`에서 `SpringApplication`(즉, 일반 봄 부팅 응용 프로그램에서 "응용 프로그램"일반적으로 어떤), "프로필"활성 프로필 (또는 쉼표로 구분 된 속성 목록) 및 "레이블"하는 선택적 git 레이블 (기본값은 "master"입니다.)





값의 출처 ( "표준"서식의 "propertySources"에 반영됨)가 여러 출처를 가지고 있더라도 YAML 및 속성 양식은 단일 맵으로 병합됩니다.





Spring Cloud Config Server는 git 저장소 (제공되어야 함)에서 원격 클라이언트에 대한 구성을 가져옵니다.







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo







### 클라이언트 측 사용



이러한 기능을 응용 프로그램에서 사용하려면 spring-cloud-config-client (예 : config-client 또는 샘플 응용 프로그램의 테스트 사례 참조)에 따라 달라지는 Spring Boot 응용 프로그램으로 빌드하면됩니다. 종속성을 추가하는 가장 편리한 방법은 봄 부팅 스타터를 통해입니다 `org.springframework.cloud:spring-cloud-starter-config`. 부모 치어와 BOM (도 있습니다 `spring-cloud-starter-parent`메이븐 사용자와 Gradle을 그리고 봄 CLI 사용자를위한 파일 봄 IO 버전 관리 속성에 대한)입니다. Maven 구성 예 :





pom.xml



    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>1.2.3.RELEASE</version>
        <relativePath /> <!-- lookup parent from repository -->
    </parent>

    <dependencyManagement>
        <dependencies>
            <dependency>
                <groupId>org.springframework.cloud</groupId>
                <artifactId>spring-cloud-starter-parent</artifactId>
                <version>1.0.1.RELEASE</version>
                <type>pom</type>
                <scope>import</scope>
            </dependency>
        </dependencies>
    </dependencyManagement>

    <dependencies>
        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-config</artifactId>
        </dependency>
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-test</artifactId>
            <scope>test</scope>
        </dependency>
    </dependencies>

    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
            </plugin>
        </plugins>
    </build>

    <!-- repositories also needed for snapshots and milestones -->







그런 다음이 간단한 HTTP 서버와 같은 표준 스프링 부트 응용 프로그램을 만들 수 있습니다.







<pre>@SpringBootApplication
@RestController
public class Application {

    @RequestMapping ( "/")
    public String home () {
        return "Hello World!";
    }

    공공 정적 무효 메인 (문자열 [] args) {
        SpringApplication.run (Application.class, args);
    }

}</pre>







실행될 때 포트 8888의 기본 로컬 구성 서버에서 외부 구성을 선택합니다 (실행중인 경우). 다음을 사용하여 구성 서버의 위치를 변경할 수 있습니다 시작 동작을 수정하려면 `bootstrap.properties`(좋아 `application.properties`하지만 애플리케이션 컨텍스트의 부트 스트랩 단계에), 예를 들어,







<pre>spring.cloud.config.uri : http://myconfigserver.com</pre>







부트 스트랩 속성은에 표시됩니다 `/env`예를 들어 우선 순위가 높은 속성 소스,로 엔드 포인트







<pre>$ curl localhost : 8080 / env
{
  "프로필": [],
  "configService : https : //github.com/spring-cloud-samples/config-repo/bar.properties": { "foo": "bar"},
  "servletContextInitParams": {},
  "systemProperties": {...},
  ...
}</pre>







( "configService : <원격 저장소의 URL / <파일 이름>"이라는 속성 소스에는 "bar"값을 갖는 속성 "foo"가 포함되어 있으며 가장 우선 순위가 높음).











<td class="icon">

노트



<td class="content">속성 소스 이름의 URL은 config 서버 URL이 아닌 git 저장소입니다.

















## Spring Cloud 구성 서버





서버는 외부 구성 (이름 - 값 쌍 또는 이와 동등한 YAML 내용)을위한 HTTP, 자원 기반 API를 제공합니다. 서버는 사용하여 봄 부팅 응용 프로그램에 쉽게 퍼갈 수 있습니다 `@EnableConfigServer`주석을. 그래서이 응용 프로그램은 설정 서버입니다 :





ConfigServer.java



    @SpringBootApplication
    @EnableConfigServer
    public class ConfigServer {
      public static void main(String[] args) {
        SpringApplication.run(ConfigServer.class, args);
      }
    }







모든 Spring Boot 어플리케이션과 마찬가지로 기본적으로 포트 8080에서 실행되지만 다양한 방법으로 기존 포트 8888로 전환 할 수 있습니다. 또한, 기본 구성 저장소를 설정하여 그것을 시작으로, 이는 가장 쉬운은 `spring.config.name=configserver`(A 존재 `configserver.yml`는 config 서버 항아리). 또 다른 자신의 사용하는 것 `application.properties`, 예를





application.properties



    server.port: 8888
    spring.cloud.config.server.git.uri: file://${user.home}/config-repo







어디 `${user.home}/config-repo`YAML 및 특성 파일이 포함 된 자식 저장소입니다.











<td class="icon">

노트



<td class="content">그것은 예를 들어 드라이브 접두사, 절대 경우 Windows에서 당신은 "/"파일 URL에 추가해야합니다 `[file:///${user.home}/config-repo](file:///$%7Buser.home%7D/config-repo)`.

















<td class="icon">

팁



<td class="content">



위의 예에서 git 저장소를 만드는 방법은 다음과 같습니다.







<pre>$ cd $ HOME
$ mkdir config-repo
$ cd config-repo
$ git init.
$ echo info.foo : bar> application.properties
$ git add -A.
$ git commit -m "application.properties 추가"</pre>























<td class="icon">

경고



<td class="content">git 저장소에 로컬 파일 시스템을 사용하는 것은 테스트 용입니다. 프로덕션 환경에서 서버를 사용하여 구성 저장소를 호스트하십시오.











### 환경 저장소



구성 서버의 구성 데이터를 어디에 저장 하시겠습니까? 이 동작을 지배하는 전략은이다 `EnvironmentRepository`, 제공 `Environment`목적. 이 `Environment`봄에서 도메인의 단순 복사본입니다 `Environment`(을 포함한 `propertySources`주요 기능으로). `Environment`자원은 세 가지 변수에 의해 매개 변수화된다 :





*   `{application}` 클라이언트 쪽에서 "spring.application.name"에 매핑됩니다.

*   `{profile}`클라이언트의 "spring.active.profiles"에 매핑됩니다 (쉼표로 구분 된 목록). 및

*   `{label}` 이 파일은 "버전 관리"된 설정 파일의 레이블을 지정하는 서버 측 기능입니다.





저장소 구현은 일반적으로 단지와 같은 "spring.config.name"에서 봄 부팅 응용 프로그램 로딩 구성 파일처럼 작동 `{application}`매개 변수와 동일 "spring.profiles.active" `{profiles}`매개 변수입니다. 활성 프로파일이 기본 설정보다 우선하고, 다중 프로파일이있는 경우 마지막의 (a에 항목을 추가하는 등 승리 : 프로필의 우선 순위 규칙은 일반 부트 응용 프로그램에서와 동일하다 `Map`).





예 : 클라이언트 응용 프로그램에이 부트 스트랩 구성이 있습니다.





bootstrap.yml



    spring:
      application:
        name: foo
      profiles:
        active: dev,mysql







(보통 Spring Boot 응용 프로그램과 마찬가지로이 등록 정보는 환경 변수 또는 명령 행 인수로 설정 될 수도 있습니다).





저장소는 파일 기반의 경우, 서버는 만듭니다 `Environment`에서 `application.yml`(모든 클라이언트간에 공유)를, 그리고 `foo.yml`(와 `foo.yml`우선 순위를 복용). YAML 파일에 스프링 프로파일을 가리키는 문서가있는 경우, 프로파일은 나열된 프로파일 순서대로 더 높은 우선 순위로 적용되며, 프로파일 특정 YAML (또는 특성) 파일이있는 경우 YAML 파일보다 높은 우선 순위로 적용됩니다 기본값. 높은 precendence는로 변환 `PropertySource`이전에 나열된 `Environment`. (이것들은 독립 실행 형 Spring Boot 응용 프로그램과 동일한 규칙입니다.)





#### 힘내 백엔드



의 기본 구현은 `EnvironmentRepository`감사 변경도 업그레이드 및 물리적 환경 및 관리를위한 매우 편리한 망할 놈의 백엔드를 사용합니다. 당신이 구성 서버의 "spring.cloud.config.server.git.uri"구성 속성을 설정할 수 있습니다 저장소 (예에서의 위치를 변경하려면 `application.yml`). 당신이 그것을 설정하면 `file:`접두사 그렇지 않은 경우는 중요하지 않습니다 (당신이 서버없이 쉽고 빠르게 시작할 수 있도록 로컬 저장소에서 작업해야하지만,이 경우 서버는 복제하지 않고 로컬 저장소에서 직접 운영 Config Server가 "원격"저장소를 변경하지 않기 때문에 노출되지 않습니다. 구성 서버를 확장하여 가용성을 높이려면 서버의 모든 인스턴스가 동일한 저장소를 가리 키도록해야하므로 공유 파일 시스템 만 작동합니다. 심지어이 경우에 그것을 사용하는 것이 좋다 `ssh:`서버가 복제 및 캐시로 로컬 작업 복사본을 사용할 수 있도록, 공유 파일 시스템 저장소에 대한 프로토콜.





이 저장소 구현은 매핑 `{label}`힘내 라벨 (아이디, 브랜치 이름이나 태그를 커밋)에 HTTP 자원의 매개 변수를. git 브랜치 나 태그 이름에 슬래시 ( "/")가 있으면 HTTP URL의 레이블을 (다른 URL 경로와 모호하지 않게) 특수 문자열 "(_)"로 지정해야합니다. curl과 같은 명령 행 클라이언트를 사용하는 경우 URL의 대괄호에주의하십시오 (예 : 따옴표 ''가있는 쉘에서 이스케이프 처리).





##### Git URI의 자리 표시 자



봄 클라우드 구성 서버는 대한 자리 표시와 자식 저장소의 URL 지원 `{application}`과 `{profile}`(그리고 `{label}`당신이 그것을 필요로하지만 라벨이 어쨌든 자식 레이블로 적용되는 것을 기억 경우). 따라서 (예를 들어) 다음을 사용하여 "애플리케이션 당 하나의 저장소"정책을 쉽게 지원할 수 있습니다.







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/myorg/{application}







또는 "하나의 repo 프로필 당"정책은 유사한 패턴 만에를 사용 `{profile}`.







##### 패턴 일치 및 다중 저장소



또한 응용 프로그램 및 프로필 이름에 패턴 일치가있는보다 복잡한 요구 사항에 대한 지원이 있습니다. 패턴 형식의 쉼표로 구분 된 목록입니다 `{application}/{profile}`(와일드 카드로 시작하는 패턴이 인용 될 필요가있다) 와일드 카드 이름. 예:







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              repos:
                simple: https://github.com/simple/config-repo
                special:
                  pattern: special*/dev*,*special*/dev*
                  uri: https://github.com/special/config-repo
                local:
                  pattern: local*
                  uri: file:/home/configsvc/config-repo







경우 `{application}/{profile}`의 패턴과 일치하지 않습니다, 그것은 "spring.cloud.config.server.git.uri"에 정의 된 기본 URI를 사용합니다. 상기 예에서, "간단한"저장소에 패턴이다 `simple/*`(그것은 단지 모든 프로파일에서 "단순"라는 하나의 애플리케이션 일치 IE). "로컬"저장소 (모든 프로필에서 "로컬"로 시작하는 모든 응용 프로그램 이름과 일치하는 `/*`접미사 프로필 정규 표현을하지 않는 패턴에 자동으로 추가됩니다).











<td class="icon">

노트



<td class="content">위의 "간단한"예제에서 사용 된 "한 줄짜리"단축키는 설정할 유일한 속성이 URI 인 경우에만 사용할 수 있습니다. 다른 것을 설정해야하는 경우 (자격 증명, 패턴 등) 전체 양식을 사용해야합니다.











`pattern`당신은 YAML 배열을 사용할 수 있도록 REPO의 속성은 실제로 배열 (또는 `[0]`, `[1]`등 특성 파일의 접미사)는 여러 패턴에 결합 할 수 있습니다. 프로필이 여러 개인 앱을 실행하려면이 작업이 필요할 수 있습니다. 예:







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              repos:
                development:
                  pattern:
                    - */development
                    - */staging
                  uri: https://github.com/development/config-repo
                staging:
                  pattern:
                    - */qa
                    - */production
                  uri: https://github.com/staging/config-repo













<td class="icon">

노트



<td class="content">봄 클라우드에서 끝나지 않는 프로파일을 포함하는 패턴을 추측 할 것이다 `*`당신이 실제로이 패턴으로 시작하는 프로파일의 목록을 일치시킬 것을 의미한다 (그래서 `*/staging`에 대한 바로 가기입니다 `["*/staging", "*/staging,*"]`). 이는 "개발"프로파일에서 로컬로 애플리케이션을 실행해야하지만, 예를 들어 "클라우드"프로파일을 원격으로 실행해야하는 경우에 일반적입니다.











모든 저장소는 선택적으로 지정할 수 있습니다 해당 디렉토리를 검색 설정 하위 디렉토리에있는 파일 및 패턴을 저장할 수 있습니다 `searchPaths`. 예를 들어 최상위 레벨에서 :







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              searchPaths: foo,bar*







이 예제에서 서버는 최상위 레벨과 "foo /"하위 디렉토리 및 "bar"로 시작하는 이름의 하위 디렉토리에서 구성 파일을 검색합니다.





기본적으로 서버는 구성이 처음 요청 될 때 원격 저장소를 복제합니다. 시작할 때 저장소를 복제하도록 서버를 구성 할 수 있습니다. 예를 들어 최상위 레벨에서 :







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://git/common/config-repo.git
              repos:
                team-a:
                    pattern: team-a-*
                    cloneOnStart: true
                    uri: http://git/team-a/config-repo.git
                team-b:
                    pattern: team-b-*
                    cloneOnStart: false
                    uri: http://git/team-b/config-repo.git
                team-c:
                    pattern: team-c-*
                    uri: http://git/team-a/config-repo.git







이 예제에서 서버는 시작시 임의의 요청을 수락하기 전에 팀 -a의 config-repo를 복제합니다. 다른 모든 리포지토리는 리포지토리의 구성이 요청 될 때까지 복제되지 않습니다.





원격 저장소에서 HTTP 기본 인증을 사용하려면 "username"과 "password"속성을 URL에 별도로 추가하십시오 (예 :







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              username: trolley
              password: strongpassword







당신이 HTTPS 및 사용자 자격 증명을 사용하지 않는 경우 기본 디렉토리에 키 (저장하면, SSH는 상자 밖으로 작동합니다 `~/.ssh`SSH를 위치, 예를 들면 "로)와 URI 점을 [git@github.com](mailto:git@github.com) / cloud- 구성 : 구성 ". 저장소는 JGit을 사용하여 액세스하므로 해당 문서를 찾을 수 있어야합니다. HTTPS 프록시 설정이 설정 될 수 `~/.git/config`또는 시스템 특성 (통해 다른 JVM 공정과 동일한 방법으로 `-Dhttps.proxyHost`하고 `-Dhttps.proxyPort`).









#### 파일 시스템 백엔드



설정 서버에는 Git을 사용하지 않는 "네이티브"프로필이 있지만 로컬 클래스 경로 또는 파일 시스템 ( "spring.cloud.config.server"로 가리키는 모든 정적 URL)에서 구성 파일을로드합니다 .native.searchLocations "). 기본 프로필을 사용하려면 "spring.profiles.active = native"를 사용하여 구성 서버를 시작하십시오.











<td class="icon">

노트



<td class="content">사용하는 것을 잊지 `file:`파일 자원에 대한 접두사 (접두사없이 기본값은 일반적으로 클래스 경로입니다). 그냥 봄 부팅 구성으로 당신은 포함 할 수 있습니다 `${}`스타일의 환경 자리를하지만, Windows의 절대 경로 추가 "/", 예를 들어 필요로 기억`[file:///${user.home}/config-repo](file:///$%7Buser.home%7D/config-repo)`

















<td class="icon">

경고



<td class="content">의 초기 값은 `searchLocations`로컬 스프링 부트 프로그램 (그래서 동일하다 `[classpath:/, classpath:/config, file:./, file:./config]`). 이 노출되지 않고 `application.properties`, 서버에 존재하는 임의의 프로퍼티 소스 클라이언트로 전송되기 전에 제거되어 있기 때문에 모든 클라이언트는 서버로부터.

















<td class="icon">

팁



<td class="content">파일 시스템 백엔드는 신속하게 시작하고 테스트하기에 좋습니다. 프로덕션 환경에서 사용하려면 파일 시스템이 안정적이어야하며 모든 구성 서버 인스턴스에서 공유해야합니다.











검색 위치에 대한 자리 표시자를 포함 할 수 있습니다 `{application}`, `{profile}`하고 `{label}`. 이 방법으로 경로의 디렉토리를 분리하고 자신에게 맞는 전략 (예 : 응용 프로그램 별 하위 디렉토리 또는 프로필 당 하위 디렉토리)을 선택할 수 있습니다.





당신이 검색 위치에 자리 표시자를 사용하지 않는 경우,이 저장소는 추가 `{label}`속성 파일이 각 검색 위치에서로드되도록, 검색 경로에 접미사로 HTTP 자원의 매개 변수 **및** 레이블과 동일한 이름의 하위 디렉토리 ( 레이블이 지정된 속성은 Spring 환경에서 우선 순위를가집니다). 따라서 어떤 자리와 기본 동작으로 끝나는 검색 위치를 추가하는 것과 같은이 `/{label}/. For example `file:/tmp/config` 동일하다`file:/tmp/config,file:/tmp/config/{label}`







#### 모든 응용 프로그램과 구성 공유



파일 기반 (즉, 자식, SVN 및 기본) 저장소에서 파일 이름을 가진 자원과 `application*`모든 클라이언트 응용 프로그램 (그래서 사이에 공유 `application.properties`, `application.yml`, `application-*.properties`등). 이러한 파일 이름의 자원을 사용하여 전역 기본값을 구성하고 필요에 따라 응용 프로그램 특정 파일로 대체 할 수 있습니다.





#_property_overrides [속성 재정의] 기능은 전역 기본값을 설정하는 데 사용할 수도 있으며 자리 표시 자 응용 프로그램에서 로컬 우선 순위를 재정의 할 수 있습니다.











<td class="icon">

팁



<td class="content">"네이티브"프로파일 (로컬 파일 시스템 백엔드)을 사용하면 서버 자체 구성의 일부가 아닌 명시 적 검색 위치를 사용하는 것이 좋습니다. 그렇지 않으면 `application*` 그들은 서버의 일부이기 때문에 기본 검색 위치에 자원이 제거됩니다.













#### 속성 재정의



구성 서버에는 정상적인 스프링 부트 훅을 사용하여 응용 프로그램이 실수로 변경할 수없는 모든 응용 프로그램에 구성 속성을 제공 할 수있는 "재정의"기능이 있습니다. 재정의를 선언하려면 단지에 이름 - 값 쌍의 맵을 추가 `spring.cloud.config.server.overrides`. 예를 들어







    spring:
      cloud:
        config:
          server:
            overrides:
              foo: bar







읽기 고객을 config (설정) 모든 응용 프로그램의 원인이됩니다 `foo=bar` 자신의 구성을 독립적으로합니다. 물론 응용 프로그램은 구성 서버의 데이터를 원하는 방식으로 사용할 수 있으므로 재정의는 적용 할 수 없지만 Spring Cloud 구성 클라이언트 인 경우 유용한 기본 동작을 제공합니다.











<td class="icon">

팁



<td class="content">은 "$"또는 "은 {"는, 예를 들어 탈출 ( "\") 백 슬래시를 사용하여 "$ {}"이스케이프 (클라이언트에 해결) 할 수있다 정상, 봄 환경 자리 `\${app.foo:bar}`앱하지 않는 한에 "바"를 해결합니다 자체 "app.foo"를 제공합니다. YAML에서 백 슬래시 자체를 이스케이프 할 필요는 없지만 서버에서 오버라이드를 구성 할 때는 속성 파일에서 이스케이프해야합니다.











클라이언트의 모든 재정의 우선 순위를 기본값과 비슷하게 변경할 수 있으므로 응용 프로그램에서 환경 변수 또는 시스템 등록 정보에 자체 값을 제공 할 수 있습니다. 플래그는`









### 건강 지표



구성 서버 구성이 경우 확인하는 건강 지표와 함께 제공 `EnvironmentRepository`하고있다. 기본적으로는 요청 `EnvironmentRepository` 라는 응용 프로그램 `app`의 `default`프로파일 및 제공하는 기본 레이블 `EnvironmentRepository`구현입니다.





사용자 정의 프로파일 및 사용자 정의 레이블과 함께 더 많은 어플리케이션을 점검하도록 Health 표시기를 구성 할 수 있습니다.







    spring:
      cloud:
        config:
          server:
            health:
              repositories:
                myservice:
                  label: mylabel
                myservice-dev:
                  name: myservice
                  profiles: development







당신은 설정하여 건강 지표를 사용하지 않도록 설정할 수 있습니다 `spring.cloud.config.server.health.enabled=false`.







### 보안



물리적 네트워크 보안에서부터 OAuth2 베어러 토큰에 이르는 모든 방식으로 설정 서버를 자유롭게 보호 할 수 있으며 Spring Security와 Spring Boot를 사용하면 쉽게 모든 것을 할 수 있습니다.





HTTP 기본 보안 구성 기본 봄 부팅을 사용하려면, 그냥 (예를 통해 클래스 패스에 봄 보안 포함 `spring-boot-starter-security`). 기본값은 "사용자"연습에 매우 유용 될 수 없습니다 임의로 생성 된 암호의 이름, 그래서 우리는 당신이 (를 통해 암호를 구성하는 것이 좋습니다 `security.user.password`)과 (을 암호화하는 것이 수행하는 방법에 대한 지침은 아래를 참조하십시오 ).







### 암호화 및 암호 해독









<td class="icon">

중대한



<td class="content">**전제 조건 :** 당신이 당신의 JVM에 설치된 전체 강도 JCE를 필요로하는 암호화 및 복호화 기능 (기본값이 아닙니다)를 사용합니다. Oracle에서 "Java Cryptography Extension (JCE) 무제한 강도 관할 정책 파일"을 다운로드하고 설치 지침을 따르십시오 (기본적으로 JRE lib / security 디렉토리에있는 2 개의 정책 파일을 다운로드 한 정책 파일로 대체하십시오).











원격 속성 소스 (값으로 시작 암호화 된 콘텐츠를 포함하는 경우 `{cipher}`) 그들은 HTTP를 통해 클라이언트에 전송하기 전에 암호를 해독 할 것입니다. 이 설정의 가장 큰 장점은 속성 값이 "휴식"(예 : 자식 저장소에서) 일 때 일반 텍스트 일 ​​필요가 없다는 것입니다. 값을 암호 해독 할 수 없으면이 값은 속성 원본에서 제거되고 추가 속성은 같은 키로 추가되지만 접두사는 "잘못되었습니다." "적용 할 수 없음"을 의미하는 값 (일반적으로 "<n / a>"). 이것은 주로 암호문이 실수로 누출되거나 암호로 사용되는 것을 방지하기위한 것입니다.





당신이 설정 클라이언트 응용 프로그램에 대한 원격 구성 저장소를 설정하는 경우는 포함 할 수 있습니다 `application.yml`예를 들어이 등을 :





application.yml



    spring:
      datasource:
        username: dbuser
        password: '{cipher}FKSAJDFGYOS8F7GLHAKERGFHLSAJ'







.properties 파일의 암호화 된 값은 따옴표로 묶어서는 안됩니다. 그렇지 않으면 값이 해독되지 않습니다.





application.properties



<pre>spring.datasource.username : dbuser
spring.datasource.password : {암호} FKSAJDFGYOS8F7GLHAKERGFHLSAJ</pre>







이 일반 텍스트를 공유 git 저장소로 안전하게 푸시 할 수 있으며 비밀 암호가 보호됩니다.





서버는 또한 노출 `/encrypt`하고 `/decrypt`(이 확보하고 공인 에이전트에 의해 액세스되는 것으로 가정) 엔드 포인트. 원격 구성 파일을 편집하는 경우 당신은에 게시하여 값을 암호화하기 위해 구성 서버를 사용하여 `/encrypt`엔드 포인트, 예를 들어,







<pre>$ curl localhost : 8888 / encrypt -d mysecret
682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda</pre>







역 동작도를 통해 사용할 수 있습니다 `/decrypt`(서버가 대칭 키 또는 전체 키 쌍으로 구성되어 제공)







<pre>$ curl localhost : 8888 / decrypt -d 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
나의 비밀</pre>













<td class="icon">

팁



<td class="content">당신은 컬과 같이 테스트하는 경우, 사용 `--data-urlencode`(대신 `-d`명시 적)을 설정하거나 `Content-Type: text/plain`확인 컬 특수 문자가있는 경우 정확하게 데이터를 인코딩하기 위해 ( '+'는 특히 까다 롭다).











암호화 된 값을 타고 추가 `{cipher}`, 잠재적으로 안전하지 않은 매장은 YAML 또는 속성에 넣어 제출하기 전에 접두사를, 당신은 커밋하기 전에 원격으로 밀어 넣습니다.





`/encrypt`과 `/decrypt`끝점은 두 형태의 경로를 받아 `/*/{name}/{profiles}`클라이언트 메인 환경 자원으로 호출 할 때 애플리케이션 (명) 및 프로파일에 따라 암호화를 제어하기 위해 사용될 수있다.











<td class="icon">

노트



<td class="content">당신은 또한을 제공해야이 세분화 된 방법으로 암호화 제어하는 `@Bean`타입의 `TextEncryptorLocator`이름과 프로필마다 다른 암호 화기를 만듭니다. 기본적으로 제공되는 암호화는이 작업을 수행하지 않으므로 모든 암호화가 동일한 키를 사용합니다.











`spring`(설치 Spring Cloud CLI 확장자) 명령 행 클라이언트는, 예를 암호화하고 해독하는 데 사용할 수 있습니다







<pre>$ spring encrypt mysecret --key foo
682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
$ spring decrypt --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
나의 비밀</pre>







파일 (예 : 암호화를위한 RSA 공개 키)에서 키를 사용하려면 키 값 앞에 "@"를 붙이고 파일 경로를 제공하십시오.







<pre>$ spring encrypt mysecret --key @ $ {HOME} /. ssh / id_rsa.pub
AQAjPgt3eFZQXwt8tsHAVv / QHiY5sI2dRcR + ...</pre>







key 인수의 (a에도 불구하고 필수 `--`접두사).







### 키 관리



구성 서버는 대칭 (공유) 키 또는 비대칭 (RSA 키 쌍) 키를 사용할 수 있습니다. 비대칭 선택은 보안 측면에서 우수하지만 구성 할 단일 속성 값이므로 대칭 키를 사용하는 것이 더 편리합니다.





방금 설정해야합니다 대칭 키 구성하려면 `encrypt.key`비밀 String으로 (또는 환경 변수를 사용하는 `ENCRYPT_KEY`일반 텍스트 구성 파일에서 그것을 유지하기 위해 참조).





비대칭 키를 구성하려면 (의 PEM 인코딩 된 텍스트 값으로 키를 설정할 수 있습니다 `encrypt.key`), 또는 키 스토어를 통해 (예에 의해 생성으로 `keytool`의 JDK와 함께 제공 유틸리티). 키 스토어 등록 정보는 다음 `encrypt.keyStore.*`과 `*`같





*   `location`(A `Resource`위치)

*   `password` (키 스토어의 잠금을 해제하기 위해)

*   `alias` (상점에서 어떤 키가 사용되는지 식별하기 위해).





암호화는 공개 키를 사용하여 수행되며 개인 키는 암호 해독에 필요합니다. 따라서 암호화를 원한다면 원칙적으로 서버의 공개 키 만 구성 할 수 있습니다 (개인 키로 로컬에서 값을 해독 할 준비가되어 있음). 실제로는 핵심 관리 프로세스가 서버에 집중되는 대신 모든 클라이언트를 중심으로 확산되므로이를 수행하고 싶지 않을 수 있습니다. 반면에 config 서버가 실제로 상대적으로 안전하지 않고 소수의 클라이언트 만 암호화 된 속성이 필요한 경우 유용한 옵션입니다.







### 테스트 용 키 저장소 만들기



테스트 용 키 저장소를 만들려면 다음과 같이하면됩니다.







<pre>$ keytool -genkeypair -alias mytestkey -keyalg RSA \
  -dname "CN = 웹 서버, OU = 단위, O = 조직, L = 도시, S = 상태, C = 미국"
  -keypass changeme -keystore server.jks -storepass letmein</pre>







풋 `server.jks`(예를 들어) 클래스 경로에 파일을 한 다음에 `application.yml`는 config 서버 :







    encrypt:
      keyStore:
        location: classpath:/server.jks
        password: letmein
        alias: mytestkey
        secret: changeme









### 여러 키 및 키 회전 사용



받는 사람 또한 `{cipher}`암호화 된 속성 값에 접두사의 구성 서버를 찾습니다 `{name:value}`제 (Base64로 인코딩 된)가 암호문의 시작 전에 접두사 (제로 또는 많은). 키가 전달됩니다 `TextEncryptorLocator`그것은을 찾을 필요가 어떤 논리 할 수있는 `TextEncryptor`암호에 대해. 당신은 (키 스토어를 구성한 경우 `encrypt.keystore.location`) 기본 로케이터는이 같은 암호 텍스트 즉, "키"접두사가 제공 별칭 가게에서 키를 찾습니다 :







    foo:
      bar: `{cipher}{key:testkey}...`







locator는 "testkey"라는 이름의 키를 찾을 것입니다. 비밀도를 통해 공급 될 수 `{secret:…​}`접두사 가치하지만, 그렇지 않은 경우 기본값은 (당신이 keytore를 구축하고 비밀을 지정하지 않을 때 무엇을 얻을입니다) 키 저장소 암호를 사용하는 것입니다. 당신이 경우에 **할** 비밀을 제공 당신은 또한 사용자 정의를 사용하여 비밀을 암호화하는 것이 좋습니다 `SecretLocator`.





키가 구성 데이터의 몇 바이트 만 암호화하는 데 사용되는 경우 (즉, 다른 곳에서 사용되지 않는 경우) 암호화 위반으로 인해 키 순환이 거의 필요하지 않지만 보안 위반이있는 경우 키를 변경해야 할 수도 있습니다. 예. 이 경우 모든 클라이언트는 소스 설정 파일을 변경 (예를 들어 자식에) 새로운 사용해야합니다 `{key:…​}`키 별명이 구성 서버 키 스토어에서 사용할 수 있는지 사전에 물론 검사, 모든 암호에 접두사.











<td class="icon">

팁



<td class="content">`{name:value}`접두사도에 게시 일반 텍스트 추가 할 수 있습니다 `/encrypt`당신은 구성 서버가 암호 해독뿐만 아니라 모든 암호화를 처리 할 수 있도록하려는 경우, 엔드 포인트.

















## 일반 텍스트 검색





대신에 사용하는 `Environment`추상화 (또는 YAML 또는 속성 형식으로 그것의 다른 표현 중 하나) 응용 프로그램은 자신의 환경에 맞는 일반 일반 텍스트 구성 파일을해야 할 수도 있습니다. 는 config 서버에서 추가 엔드를 통해이 제공 `/{name}/{profile}/{label}/{path}` "이름", "프로필"및 "라벨"은 일정한 환경 엔드와 같은 의미를 가질 경우, 그러나 "경로"파일 이름 (예이다 `log.xml`). 이 엔드 포인트의 소스 파일은 환경 엔드 포인트와 동일한 방법으로 위치합니다. 동일한 검색 경로가 특성 또는 YAML 파일에 사용되지만 모든 일치하는 자원을 모으는 대신 일치하는 첫 번째 파일 만 리턴됩니다.





자원이있는 후, 일반 형식 (의 자리가 `${…​}`) 유효 사용하여 해결 `Environment`제공되는 응용 프로그램의 이름, 프로필 및 레이블을. 이 f}으로 자원 엔드 포인트는 환경 엔드 포인트와 긴밀하게 통합됩니다. 예를 들어, GIT (또는 SVN) 저장소에 대한 레이아웃이있는 경우 :







<pre>application.yml
nginx.conf</pre>







위치는 `nginx.conf`다음과 같습니다 :







<pre>서버 {
    80을 듣는다.
    server_name $ {nginx.server.name};
}</pre>







과 `application.yml`같은 :







    nginx:
      server:
        name: example.com
    ---
    spring:
      profiles: development
    nginx:
      server:
        name: develop.com







다음 `/foo/default/master/nginx.conf`리소스는 다음과 같습니다 :







<pre>서버 {
    80을 듣는다.
    server_name example.com;
}</pre>







과 `/foo/development/master/nginx.conf`같은 :







<pre>서버 {
    80을 듣는다.
    server_name develop.com;
}</pre>













<td class="icon">

노트



<td class="content">단지 환경 구성에 대한 소스 파일처럼 "프로필"은 파일 이름을 확인하는 데 사용됩니다, 그래서 당신은 프로필 - 특정 파일을 원하는 경우 다음 `/*/development/*/logback.xml`라는 파일에 의해 해결 될 것 `logback-development.xml`(에 우선 `logback.xml`).















## 구성 서버 포함





구성 서버는 독립 실행 형 응용 프로그램으로 가장 잘 실행되지만 필요한 경우 다른 응용 프로그램에 포함 할 수 있습니다. 그냥 사용 `@EnableConfigServer`주석을. 이러한 경우에 유용 할 수있는 선택적인 속성은 `spring.cloud.config.server.bootstrap`서버가 자신의 원격 저장소에서 자동으로 구성한다는 것을 표시하는 플래그이다. 이 플래그는 시작을 지연시킬 수 있으므로 기본적으로 해제되어 있지만 다른 응용 프로그램에 포함 된 경우 다른 응용 프로그램과 같은 방법으로 초기화하는 것이 좋습니다.











<td class="icon">

노트



<td class="content">그것은 분명하지만 부트 스트랩 플래그를 사용하는 경우 설정 서버 이름 및 저장소 URI가 구성되어 있어야합니다 있음을 알아 두셔야합니다 `bootstrap.yml`.











할 수 있습니다 (선택 사항) 세트 서버 엔드 포인트의 위치를 변경하려면 `spring.cloud.config.server.prefix`, "/ 설정", 예를 들어 접두사에서 자원 봉사. 접두사는 시작해야하지만 "/"로 끝나지 않아야합니다. 그것은에 적용된다 `@RequestMappings`(즉, 봄 부팅 접두사 아래 구성 서버에서 `server.servletPath`하고 `server.contextPath`).





기본적으로 엔드 포인트가없는 임베디드 구성 서버 인 백엔드 저장소 (구성 서버가 아닌)에서 응용 프로그램의 구성을 직접 읽으려는 경우. 당신이 사용하지 않는 경우에는 전체 엔드 포인트를 전환 할 수 있습니다 `@EnableConfigServer` 주석 (단지 설정을 `spring.cloud.config.server.bootstrap=true`).









## 푸시 알림 및 스프링 클라우드 버스





많은 소스 코드 저장소 공급자 (예 : Github, Gitlab 또는 Bitbucket)는 Webhook을 통해 저장소의 변경 사항을 알려줍니다. 제공자의 사용자 인터페이스를 통해 웹 훅을 URL 및 관심있는 이벤트 세트로 구성 할 수 있습니다. 예를 들어 [Github에서이](https://developer.github.com/v3/activity/events/types/#pushevent) 커밋의 목록이 포함 된 JSON의 시체와 함께으로 webhook에 게시하고 헤더 "X-Github에서-이벤트"와 같은 "푸시"합니다. 당신이에 대한 종속성 추가하면 `spring-cloud-config-monitor`라이브러리를하고, 당신의 구성 서버에서 봄 클라우드 버스를 활성화 한 다음 "/ 모니터"엔드 포인트를 사용할 수 있습니다.





은 webhook가 활성화되면 구성 서버가 보내드립니다 `RefreshRemoteApplicationEvent`가 변경되었을 수 있습니다 생각하는 애플리케이션을 대상으로한다. 변경 감지는 전략적으로 수행 할 수 있지만 기본적으로 응용 프로그램 이름과 일치하는 파일의 변경 사항을 찾습니다 (예 : "foo.properties"는 "foo"응용 프로그램을 대상으로하고 "application.properties"는 모든 응용 프로그램을 대상으로 함) . 당신이 동작을 재정의하려는 경우 전략은 `PropertyPathNotificationExtractor` 매개 변수로 요청 헤더와 본문을 받아 변경 파일 경로의 목록을 반환한다.





기본 구성은 Github, Gitlab 또는 Bitbucket을 사용하여 즉시 사용할 수 있습니다. Github에서, Gitlab 또는의 Bitbucket에서 JSON 알림뿐만 아니라 당신은 양식 인코딩 몸 매개 변수를 "/ 모니터"를 게시하여 변경 알림을 트리거 할 수 있습니다 `path={name}`. 이것은 "{name}"패턴 (와일드 카드를 포함 할 수 있음)과 일치하는 응용 프로그램으로 브로드 캐스팅됩니다.











<td class="icon">

노트



<td class="content">는 `RefreshRemoteApplicationEvent`가있는 경우에만 송신 될 것이다 `spring-cloud-bus`는 config 서버에 상기 클라이언트 어플리케이션이 활성화된다.

















<td class="icon">

노트



<td class="content">기본 설정은 또한 로컬 자식 저장소에서 파일 시스템 변경을 감지합니다 (이 경우 webhook은 사용되지 않지만 설정 파일을 편집하자마자 새로 고침이 브로드 캐스트됩니다).















## Spring Cloud 구성 클라이언트





봄 부팅 응용 프로그램은 봄 구성 서버 (또는 응용 프로그램 개발자가 제공 한 다른 외부 속성 원)의 즉시 활용할 수 있습니다, 또한 관련된 몇 가지 추가 유용한 기능 데리러 `Environment`이벤트를 변경합니다.





### 첫 번째 부트 스트랩 구성



이는 클래스 경로에 Spring Cloud Config Client가있는 모든 애플리케이션의 기본 동작입니다. 구성 클라이언트가 시작되면 그것은 (부트 스트랩 구성 등록 정보를 통해 구성 서버에 결합 `spring.cloud.config.uri`)과 봄을 초기화 `Environment`원격 속성 소스와.





이것의 최종 결과는 구성 서버를 소비 할 모든 클라이언트 응용 프로그램이 필요하다 `bootstrap.yml`에서 서버 주소 (또는 환경 변수) `spring.cloud.config.uri`(에 기본값에 "http : // localhost를 : 8888").







### 유레카 퍼스트 부트 스트랩



Spring Cloud Netflix와 Eureka Service Discovery를 사용하고 있다면 원한다면 Eureka에 Config Server를 등록 할 수 있지만 기본적으로 "Config First"모드에서는 클라이언트가 등록을 이용할 수 없습니다.





당신이 구성 서버를 찾을 수 유레카를 사용하려는 경우, 당신이 할 수있는 설정하여 `spring.cloud.config.discovery.enabled=true`(기본 "false"로). 그 최종 결과는 클라이언트 모두가 필요 앱 있다는 `bootstrap.yml`에 예 유레카 서버 주소로 (또는 환경 변수) `eureka.client.serviceUrl.defaultZone`. 이 옵션을 사용하는 가격은 서비스 등록을 찾기 위해 시작할 때 여분의 네트워크 왕복입니다. 유레카가 고정 된 지점 인 경우 구성 서버가 좌표를 변경할 수있는 이점이 있습니다. 기본 서비스 ID는 "CONFIGSERVER"하지만 당신과 함께 클라이언트에 해당을 변경할 수 있습니다 `spring.cloud.config.discovery.serviceId`(그리고 설정하여 예 서비스에 대한 일반적인 방법으로 서버에 `spring.application.name`).





발견 클라이언트 구현은 모두 (우리가 유레카 예 : 메타 데이터 맵의 어떤 종류를 지원합니다 `eureka.instance.metadataMap`). 클라이언트가 올바르게 연결할 수 있도록 구성 서버의 일부 추가 등록 정보를 서비스 등록 메타 데이터에 구성해야 할 수 있습니다. 구성 서버가 HTTP Basic으로 보안 설정되면 "사용자 이름"및 "암호"로 자격 증명을 구성 할 수 있습니다. 구성 서버에 컨텍스트 경로가있는 경우 "configPath"를 설정할 수 있습니다. 예를 들어, 유레카 클라이언트 인 구성 서버의 경우 :





bootstrap.yml



    eureka:
      instance:
        ...
        metadataMap:
          username: osufhalskjrtl
          password: lviuhlszvaorhvlo5847
          configPath: /config









### 구성 클라이언트 실패 빠른



경우에 따라 구성 서버에 연결할 수없는 경우 서비스 시작에 실패하는 것이 바람직 할 수 있습니다. 이 원하는 동작 인 경우, 부트 스트랩 구성 속성을 설정 `spring.cloud.config.failFast=true`하고, 클라이언트는 예외 중지한다.







### 구성 클라이언트 재시도



앱이 시작될 때 설정 서버를 사용할 수 없을 것으로 예상되는 경우 오류가 발생한 후에도 계속 시도하도록 요청할 수 있습니다. 먼저 설정해야합니다 `spring.cloud.config.failFast=true`, 그리고 당신은 추가해야 `spring-retry`하고 `spring-boot-starter-aop`클래스 경로에. 기본 동작은 초기 백 오프 간격이 1000ms이고 후속 백 오프에 대해 지수 배율 1.1을 사용하여 6 회 재 시도하는 것입니다. 다음을 사용하여 이러한 속성 (및 기타) 구성 할 수 있습니다 `spring.cloud.config.retry.*`구성 속성을.











<td class="icon">

팁



<td class="content">재시도 전체를 제어 할 수있는 추가 `@Bean`유형의 `RetryOperationsInterceptor`ID가 "configServerRetryInterceptor"로. 봄 시도는이 `RetryInterceptorBuilder`일을 만들 쉽게 만드는.













### 원격 구성 리소스 찾기



구성 서비스에서 속성 소스를 제공 `/{name}/{profile}/{label}`클라이언트 응용 프로그램의 기본 바인딩이있는 곳,





*   "name"= `${spring.application.name}`

*   "프로필"= `${spring.profiles.active}`(실제로 `Environment.getActiveProfiles()`)

*   "label"= "master"





그들 모두는 설정에 의해 무시 될 수있다 `spring.cloud.config.*` (여기서 `*`"이름", "프로필"또는 "라벨"입니다). "레이블"은 이전 버전의 구성으로 롤백 할 때 유용합니다. 기본 구성 서버 구현에서는 git 레이블, 분기 이름 또는 커밋 ID가 될 수 있습니다. 레이블은 쉼표로 구분 된 목록으로 제공 될 수도 있습니다.이 경우 목록에있는 항목은 성공할 때까지 하나씩 시도됩니다. 이것은 선택 사항 (예 : 예를 들어, 기능 분기에 작업 할 때 당신이 당신의 지점으로 설정 레이블을 정렬 할 수있는 경우에 유용 할 수 있지만 수 있습니다 `spring.cloud.config.label=myfeature,develop`).







### 보안



서버에서 HTTP 기본 보안을 사용하면 클라이언트는 암호 (및 기본값이 아닌 경우 사용자 이름)를 알아야합니다. 설정 서버 URI 나 별도의 사용자 이름과 패스워드 속성을 통해 할 수 있습니다.





bootstrap.yml



    spring:
      cloud:
        config:
         uri: https://user:secret@myconfig.mycompany.com







또는





bootstrap.yml



    spring:
      cloud:
        config:
         uri: https://myconfig.mycompany.com
         username: user
         password: secret







`spring.cloud.config.password`와 `spring.cloud.config.username` 값은 URI에 제공되는 것을 우선합니다.





Cloud Foundry에 응용 프로그램을 배포하는 경우 암호를 제공하는 가장 좋은 방법은 서비스 자격 증명 (예 : URI)을 사용하는 것이므로 설정 파일에있을 필요가 없기 때문입니다. "configserver"라는 Cloud Foundry에서 사용자가 제공하는 서비스와 로컬로 작동하는 예제 :





bootstrap.yml



    spring:
      cloud:
        config:
         uri: ${vcap.services.configserver.credentials.uri:http://user:password@localhost:8888}







보안의 또 다른 형태를 사용하는 경우 당신은 제공해야 할 수 있습니다 `RestTemplate`받는 사람 `ConfigServicePropertySourceLocator`(부트 스트랩 맥락에서 그것을 잡아 하나를 주입하여 예를).









# Spring Cloud 넷플 릭스



이 프로젝트는 자동 환경 설정과 스프링 환경 및 기타 스프링 프로그래밍 모델 관용구에 대한 바인딩을 통해 스프링 부트 애플리케이션을위한 Netflix OSS 통합을 제공합니다. 몇 가지 간단한 주석을 사용하면 애플리케이션 내부의 공통 패턴을 신속하게 활성화 및 구성하고 전투 테스트를 거친 Netflix 구성 요소로 대규모 분산 시스템을 구축 할 수 있습니다. 제공되는 패턴에는 서비스 발견 (Eureka), 회로 차단기 (Hystrix), 지능형 라우팅 (Zuul) 및 클라이언트 측로드 균형 조정 (리본)이 포함됩니다.





## 서비스 발견 : 유레카 클라이언트





서비스 검색은 마이크로 서비스 기반 아키텍처의 핵심 교리 중 하나입니다. 각 클라이언트 또는 일부 형식의 컨벤션 구성을 손으로 처리하는 것은 매우 어려울 수 있으며 매우 취성이 있습니다. 유레카는 Netflix 서비스 검색 서버 및 클라이언트입니다. 서버는 등록 된 서비스에 대한 상태를 다른 서버로 복제하여 각 서버가 고 가용성으로 구성 및 배치 될 수 있습니다.





### 유레카 등록



클라이언트가 유레카에 등록하면 호스트 및 포트, 상태 표시기 URL, 홈 페이지 등과 같은 메타 데이터를 제공합니다. 유레카는 서비스에 속한 각 인스턴스에서 하트 비트 메시지를받습니다. 하트 비트가 구성 가능한 시간표에 실패하면 보통 인스턴스는 레지스트리에서 제거됩니다.





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







(즉, 완전히 정상적인 스프링 부트 응용 프로그램). 우리가 사용하는이 예에서 `@EnableEurekaClient`명시 적으로 만 유레카 사용할 수와 함께 당신은 또한 사용할 수 있습니다 `@EnableDiscoveryClient`. Eureka 서버를 찾으려면 구성이 필요합니다. 예:





application.yml



<pre>유레카:
  고객:
    serviceUrl :
      defaultZone : http : // localhost : 8761 / eureka /</pre>







여기서 "defaultZone"은 기본 설정을 나타내지 않는 클라이언트 (즉 유용한 기본값)에 대한 서비스 URL을 제공하는 마법 문자열 대체 값입니다.





기본 프로그램 이름 (서비스 ID)는 가상 호스트와 비보안 포트는 상기에서 촬영 `Environment`하고, `${spring.application.name}`, `${spring.application.name}`및 `${server.port}`는 각각.





`@EnableEurekaClient`응용 프로그램을 유레카 "인스턴스"(즉, 자체 등록)와 "클라이언트"(즉, 다른 서비스를 찾기 위해 레지스트리에 쿼리 할 수 ​​있음)로 만듭니다. 인스턴스 동작에 의해 구동되는 `eureka.instance.*`구성 키,하지만 당신은 응용 프로그램이이 있는지 확인하는 경우 기본값은 잘 될 것입니다 `spring.application.name`(이 유레카 서비스 ID, 또는 VIP에 대한 기본값입니다).





참조 [EurekaInstanceConfigBean](https://github.com/%7Bgithub-repo%7D/tree/%7Bgithub-tag%7D/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java) 및 [EurekaClientConfigBean를](https://github.com/%7Bgithub-repo%7D/tree/%7Bgithub-tag%7D/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/eureka/EurekaClientConfigBean.java) 구성 가능한 옵션의 자세한 내용은.







### 상태 페이지 및 상태 표시기



Eureka 인스턴스의 상태 페이지 및 상태 표시기는 각각 Spring Boot Actuator 응용 프로그램의 유용한 끝점의 기본 위치 인 "/ info"및 "/ health"로 기본 설정됩니다. 당신은 당신이 기본이 아닌 컨텍스트 경로 나 서블릿 경로 (예를 들어 사용하는 경우에도 액추에이터 응용 프로그램이 변경해야합니다 `server.servletPath=/foo`) 또는 관리 엔드 포인트 경로 (예 : `management.contextPath=/admin`). 예:





application.yml



<pre>유레카:
  예:
    statusPageUrlPath : $ {management.context-path} / info
    healthCheckUrlPath : $ {management.context-path} / 건강</pre>







이러한 링크는 클라이언트가 사용하는 메타 데이터에 표시되며 일부 시나리오에서는 응용 프로그램에 요청을 보낼지 여부를 결정하는 데 사용되므로 정확하면 유용합니다.







### 보안 응용 프로그램 등록



앱이 HTTPS를 통해 연락을 원하는 경우에 당신은 두 개의 플래그를 설정할 수 있습니다 `EurekaInstanceConfig`, _즉_ `eureka.instance.[nonSecurePortEnabled,securePortEnabled]=[false,true]` 각각. 이렇게하면 Eureka가 보안 통신에 대한 명시적인 선호를 보여주는 인스턴스 정보를 게시하게됩니다. Spring Cloud은 `DiscoveryClient`항상 반환 `[https://…​](https://%E2%80%A6%E2%80%8B/);`이 방식으로 구성 서비스에 대한 URI를하고, 유레카 (기본) 인스턴스 정보는 안전한 상태 점검 URL이있을 것이다.





유레카가 내부적으로 작동하는 방식 때문에 명시 적으로 명시 적으로 무시하지 않는 한 상태 및 홈 페이지에 대해 보안되지 않은 URL을 게시합니다. 자리 표시자를 사용하여 eureka 인스턴스 URL을 구성 할 수 있습니다 (예 :





application.yml



<pre>유레카:
  예:
    statusPageUrl : https : // $ {eureka.hostname} / info
    healthCheckUrl : https : // $ {eureka.hostname} / 건강
    homePageUrl : https : // $ {eureka.hostname} /</pre>







(즉, 주 `${eureka.hostname}`유레카의 이후 버전에서만 사용할 기본 자리 표시 자입니다. 당신은뿐만 아니라, 예를 들어 사용을 봄 자리와 같은 일을 달성 할 수있다 `${eureka.instance.hostName}`.)











<td class="icon">

노트



<td class="content">앱이 프록시 뒤에 있고 SSL 종료가 프록시에있는 경우 (예 : Cloud Foundry 또는 다른 플랫폼에서 서비스로 실행하는 경우) 프록시 "전달 된"헤더를 가로 채고 처리해야합니다. 응용 프로그램. 'X-Forwarded - \ *'헤더를 명시 적으로 설정하면 Spring Boot 애플리케이션의 임베디드 Tomcat 컨테이너가 자동으로이 기능을 수행한다. 틀린 표시는 앱이 자체적으로 렌더링 한 링크가 잘못된 것입니다 (잘못된 호스트, 포트 또는 프로토콜).













### 유레카 건강 검사



기본적으로 Eureka는 클라이언트 하트 비트를 사용하여 클라이언트가 작동 중인지 확인합니다. 별도로 명시하지 않는 한 Discovery Client는 Spring Boot Actuator 당 응용 프로그램의 현재 상태 확인 상태를 전파하지 않습니다. 성공적으로 등록한 후 유레카는 응용 프로그램이 항상 UP 상태임을 발표합니다. 이 동작은 유레카 상태 검사를 사용하도록 설정하여 응용 프로그램 상태를 유레카로 전파함으로써 변경 될 수 있습니다. 결과적으로 다른 모든 응용 프로그램은 'UP'이외의 상태에서 응용 프로그램으로 트래픽을 전송하지 않습니다.





application.yml



<pre>유레카:
  고객:
    건강 체크:
      enabled : true</pre>







당신이 건강 검진을 통해 더 많은 제어를 필요로하는 경우, 당신은 당신의 자신의 구현을 고려할 수 있습니다 `com.netflix.appinfo.HealthCheckHandler`.







### 인스턴스 및 클라이언트에 대한 유레카 메타 데이터



Eureka 메타 데이터가 어떻게 작동하는지 이해하는 데 약간의 시간을 할애 할 가치가 있으므로 플랫폼에서 의미있는 방식으로 사용할 수 있습니다. 호스트 이름, IP 주소, 포트 번호, 상태 페이지 및 상태 확인과 같은 것들에 대한 표준 메타 데이터가 있습니다. 이들은 서비스 레지스트리에 게시되고 클라이언트가 직접적으로 서비스에 연락하는 데 사용됩니다. 추가 메타 데이터의 인스턴스 등록에 추가 될 수 `eureka.instance.metadataMap`있으며, 이는 원격 클라이언트에 액세스 할 수 있지만,이 메타 데이터의 의미를 인식하지 않는 한, 일반적으로, 클라이언트의 동작을 변경하지 않을 것이다. Spring Cloud가 이미 메타 데이터 맵에 의미를 할당 한 몇 가지 특별한 경우가 있습니다.





#### Cloudfoundry에서 유레카 사용하기



Cloudfoundry는 글로벌 라우터를 갖추고있어 동일한 앱의 모든 인스턴스가 동일한 호스트 이름을 갖습니다 (비슷한 아키텍처를 가진 다른 PaaS 솔루션에서도 동일 함). 이것은 반드시 Eureka를 사용하는 데 장애가되는 것은 아니지만 라우터를 사용하는 경우 (플랫폼을 설정하는 방법에 따라 권장 또는 필수) 호스트 이름과 포트 번호를 명시 적으로 설정해야합니다 (보안 또는 비보안 ) 라우터를 사용합니다. 인스턴스 메타 데이터를 사용하여 클라이언트의 인스턴스 (예 : 사용자 정의 부하 분산 장치)를 구별 할 수도 있습니다. 기본적으로는 `eureka.instance.instanceId`입니다 `vcap.application.instance_id`. 예 :





application.yml



<pre>유레카:
  예:
    호스트 이름 : $ {vcap.application.uris [0]}
    nonSecurePort : 80</pre>







Cloudfoundry 인스턴스에서 보안 규칙을 설정하는 방법에 따라 직접 서비스 간 호출에 호스트 VM의 IP 주소를 등록하고 사용할 수 있습니다. 이 기능은 중추 웹 서비스 (에 (아직) 사용할 수 없습니다 [PWS](https://run.pivotal.io/) ).







#### AWS에서 Eureka 사용



애플리케이션가 AWS 클라우드에 배치 될 예정이면 유레카 인스턴스 아마존 인식하도록 구성 할 것이며, 이는 사용자 지정하여 수행 할 수 [EurekaInstanceConfigBean를](https://github.com/%7Bgithub-repo%7D/tree/%7Bgithub-tag%7D/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java) 다음 방법 :







    @Bean
    @Profile("!default")
    public EurekaInstanceConfigBean eurekaInstanceConfig() {
      EurekaInstanceConfigBean b = new EurekaInstanceConfigBean();
      AmazonInfo info = AmazonInfo.Builder.newBuilder().autoBuild("eureka");
      b.setDataCenterInfo(info);
      return b;
    }









#### 유레카 인스턴스 ID 변경



바닐라 넷플 릭스 유레카 인스턴스는 호스트 이름과 동일한 ID로 등록됩니다 (예 : 호스트 당 하나의 서비스 만). 봄 클라우드 유레카는 다음과 같다 재치있는 기본을 제공합니다 `${spring.cloud.client.hostname}:${spring.application.name}:${spring.application.instance_id:${server.port}}}`. 예를 들어 `myhost:myappname:8080`.





봄 클라우드를 사용하여 당신의 고유 식별자를 제공하여이를 대체 할 수 있습니다 `eureka.instance.instanceId`. 예 :





application.yml



<pre>유레카:
  예:
    instanceId : $ {spring.application.name} : $ {spring.application.instance_id : $ {random.value}}</pre>







이 메타 데이터와 localhost에 배포 된 여러 서비스 인스턴스를 사용하면 무작위 값이 인스턴스를 고유하게 만듭니다. Cloudfoundry에서이 `spring.application.instance_id`랜덤 값이 필요하지 않도록, 봄 부팅 액추에이터 응용 프로그램에서 자동으로 채워집니다.









### EurekaClient 사용



당신이 응용 프로그램을 일단 `@EnableDiscoveryClient`(또는 `@EnableEurekaClient`) 당신은에서 서비스 인스턴스를 검색하는 데 사용할 수 있습니다 [유레카 서버](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-eureka-server) . 이를위한 한 가지 방법은 기본을 사용하는 것이다 `com.netflix.discovery.EurekaClient`(Spring Cloud 반대로 `DiscoveryClient`), 예를 들면







<pre>@Autowired
개인 EurekaClient discoveryClient;

public String serviceUrl () {
    InstanceInfo 인스턴스 = discoveryClient.getNextServerFromEureka ( "저장", 거짓);
    return instance.getHomePageUrl ();
}</pre>













<td class="icon">

팁



<td class="content">



사용하지 마십시오 `EurekaClient`의 `@PostConstruct`방법 또는에서 `@Scheduled`합니다 (이 경우 아무 곳이나 방법은 `ApplicationContext`아직 시작되지 않을 수 있습니다). 그것은 초기화됩니다 `SmartLifecycle`(과 `phase=0`) 그래서 당신이 사용할 수있는 신뢰할 수있는 최초의 또 다른에 `SmartLifecycle`더 높은 단계로.

















### 기본 Netflix EurekaClient의 대안



넌 넷플릭스 원재료를 사용하지 않은 `EurekaClient`보통 일종의 래퍼 뒤에 사용하는 것이 더 편리하다. 봄 클라우드에 대한 지원이 [척하기](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign) (A REST 클라이언트 빌더)도 [스프링`RestTemplate`](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon) 대신 실제 URL의 논리적 인 유레카 서비스 식별자 (VIP를) 사용합니다. 당신은 간단하게 설정할 수있는 물리적 서버의 고정 목록 리본을 구성하려면 `<client>.ribbon.listOfServers`물리적 주소 (또는 호스트 이름)의 쉼표로 구분 된 목록에 `<client>`클라이언트의 ID입니다.





당신은 또한 사용할 수 있습니다 `org.springframework.cloud.client.discovery.DiscoveryClient` 넷플릭스, 예를 들어, 특정 아닙니다 발견 클라이언트에 대한 간단한 API를 제공하는을







<pre>@Autowired
개인용 DiscoveryClient discoveryClient;

public String serviceUrl () {
    List <ServiceInstance> list = client.getInstances ( "STORES");
    if (list! = null && list.size ()> 0) {
        return list.get (0) .getUri ();
    }
    null를 돌려 준다.
}</pre>









### 서비스 등록이 너무 느린 이유는 무엇입니까?



인스턴스가된다는 것은 또한 (클라이언트를 통해 레지스트리에 주기적 하트 비트 포함 `serviceUrl`기본 기간 30초과를). 인스턴스, 서버 및 클라이언트가 모두 로컬 캐시에 동일한 메타 데이터를 가지고 있기 때문에 (예 : 3 비트가 필요할 수 있음) 클라이언트가 서비스를 검색 할 수 없습니다. 사용자는 사용 기간이 변경 `eureka.instance.leaseRenewalIntervalInSeconds`이 다른 서비스에 접속 된 클라이언트를 얻는 과정을 빠르게한다. 프로덕션 환경에서는 임대 갱신 기간에 대한 가정을 서버에서 내부적으로 계산하기 때문에 기본값을 사용하는 것이 좋습니다.











## 서비스 발견 : 유레카 서버





유레카 서버의 예 (예 : spring-cloud-starter-eureka-server를 사용하여 클래스 경로 설정)







    @SpringBootApplication
    @EnableEurekaServer
    public class Application {

        public static void main(String[] args) {
            new SpringApplicationBuilder(Application.class).web(true).run(args);
        }

    }







서버는 UI와 홈페이지를 갖고, 아래 일반 유레카 기능마다 HTTP API의 종단점 `/eureka/*`.





유레카 배경 읽기 : 참조 [플럭스 커패시터](https://github.com/cfregly/fluxcapacitor/wiki/NetflixOSS-FAQ#eureka-service-discovery-load-balancer) 와 [구글의 그룹 토론을](https://groups.google.com/forum/?fromgroups#!topic/eureka_netflix/g3p2r7gHnN0) .











<td class="icon">

팁



<td class="content">



Gradle의 의존성 해결 규칙과 부모 bom 기능의 부족으로 인해 spring-cloud-starter-eureka-server에 의존하기 만하면 응용 프로그램 시작시 오류가 발생할 수 있습니다. 이 문제를 해결하려면 Spring 종속성 관리 플러그인을 추가해야하며 Spring 클라우드 스타터 상위 bom을 다음과 같이 가져와야합니다.





build.gradle



    buildscript {
      dependencies {
        classpath "io.spring.gradle:dependency-management-plugin:0.4.0.RELEASE"
      }
    }

    apply plugin: "io.spring.dependency-management"

    dependencyManagement {
      imports {
        mavenBom 'org.springframework.cloud:spring-cloud-starter-parent:1.0.0.RELEASE'
      }
    }

















### 고 가용성, 영역 및 영역



Eureka 서버에는 백엔드 저장소가 없지만 레지스트리의 서비스 인스턴스는 등록을 최신 상태로 유지하기 위해 하트 비트를 보내야합니다 (메모리에서이 작업을 수행 할 수 있습니다). 또한 클라이언트는 메모리에 유레카 등록 캐시를 가지고 있기 때문에 (서비스에 대한 모든 단일 요청에 대해 레지스트리에 갈 필요가 없습니다).





기본적으로 모든 유레카 서버는 유레카 클라이언트이기도하며 피어를 찾기 위해 적어도 하나의 서비스 URL이 필요합니다. 제공하지 않으면 서비스가 실행되고 작동하지만 피어와 함께 등록 할 수 없다는 것에 대한 많은 소음이 로그에 기록됩니다.





참고 [리본 지원 자세한 내용은 아래](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon) 영역 및 지역에 대한 클라이언트 측에.







### 독립 실행 형 모드



두 개의 캐시 (클라이언트 및 서버)와 하트 비트의 결합으로 독립 실행 형 유레카 서버는 모니터 또는 탄력적 인 런타임 (예 : Cloud Foundry)을 유지하는 한 실패에 상당히 탄력적입니다. 독립 실행 형 모드에서는 클라이언트 측 동작을 계속 끌 수 있으므로 계속 시도하지 않고 피어에 도달하지 못할 수도 있습니다. 예:





application.yml (독립 실행 형 유레카 서버)



<pre>섬기는 사람:
  포트 : 8761

유레카:
  예:
    호스트 이름 : localhost
  고객:
    registerWithEureka : false
    fetchRegistry : 거짓
    serviceUrl :
      defaultZone : http : // $ {eureka.instance.hostname} : $ {server.port} / eureka /</pre>







(가) 알 `serviceUrl`로컬 인스턴스와 동일한 호스트를 가리키고 있습니다.







### 또래 인식



유레카는 여러 인스턴스를 실행하고 서로 등록하도록 요청함으로써 훨씬 더 탄력적으로 사용할 수 있습니다. 사실,이 때문에 당신이 그것을 작동하도록 할 필요가 유효한를 추가하고, 기본 동작입니다 `serviceUrl`피어, 예를





application.yml (두 개의 피어 인식 유레카 서버)



<pre>---
봄:
  프로필 : peer1
유레카:
  예:
    호스트 이름 : peer1
  고객:
    serviceUrl :
      defaultZone : http : // peer2 / eureka /

---
봄:
  프로필 : peer2
유레카:
  예:
    호스트 이름 : peer2
  고객:
    serviceUrl :
      defaultZone : http : // peer1 / eureka /</pre>







이 예제에서는 두 개의 호스트 (peer1 및 peer2)에서 동일한 서버를 실행하고 다른 Spring 프로파일에서 실행하여 사용할 수있는 YAML 파일을 가지고 있습니다. 당신은 조작하여 (생산에 그 일을 훨씬 값이 아니다) 단일 호스트에서 피어 인식을 테스트하기 위해이 구성을 사용할 수있는 `/etc/hosts`호스트 이름을 해결하기 위해이. 사실,이 `eureka.instance.hostname`당신이 자신의 호스트 이름을 알고있는 컴퓨터에서 실행중인 경우 필요하지 않습니다 (그것은 사용하여 조회됩니다 `java.net.InetAddress`기본적으로).





시스템에 여러 피어를 추가 할 수 있으며, 둘 이상의 피어가 모두 하나의 가장자리로 서로 연결되어 있으면 서로간에 등록을 동기화합니다. 피어가 물리적으로 분리 된 경우 (데이터 센터 내부 또는 여러 데이터 센터간에) 시스템은 원칙적으로 스플릿 브레인 유형 장애를 극복 할 수 있습니다.







### IP 주소 선호



어떤 경우에는 유레카가 호스트 이름이 아닌 서비스의 IP 주소를 광고하는 것이 바람직합니다. 집합 `eureka.instance.preferIpAddress` 을 `true`응용 프로그램 유레카에 등록 할 때, 호스트 이름 대신 IP 주소를 사용한다.











## 회로 차단기 : Hystrix 클라이언트





넷플릭스라는 라이브러리를 만들었습니다 [Hystrix](https://github.com/Netflix/Hystrix) 구현하는 [회로 차단기 패턴을](http://martinfowler.com/bliki/CircuitBreaker.html) . 마이크로 서비스 아키텍처에서는 서비스 호출의 다중 레이어를 갖는 것이 일반적입니다.





![HystrixGraph](./spring-cloud-doc-images/HystrixGraph.png)

그림 1\. 마이크로 서비스 그래프





서비스 수준이 낮 으면 서비스가 실패하여 연쇄 적으로 장애가 발생할 수 있습니다. 특정 서비스에 대한 통화가 특정 임계 값에 도달하면 (Hystrix에서는 5 초 동안 20 개의 실패가 기본값 임) 회선이 열리고 통화가 이루어지지 않습니다. 오류 및 개방 회로의 경우 폴백은 개발자가 제공 할 수 있습니다.





![HystrixFallback](./spring-cloud-doc-images/HystrixFallback.png)

그림 2\. Hystrix 폴백으로 계단식 오류 방지





개방 회로가 있으면 계단식 오류가 발생하지 않으므로 압도되거나 실패한 서비스를 치료할 수 있습니다. 폴백은 또 다른 Hystrix 보호 호출, 정적 데이터 또는 정상적인 빈 값일 수 있습니다. 폴백은 체인으로 연결되어 첫 번째 폴백이 다른 비즈니스 호출을 만들어 정적 데이터로 다시 폴백 할 수 있습니다.





부팅 앱의 예 :







<pre>@SpringBootApplication
@EnableCircuitBreaker
public class Application {

    공공 정적 무효 메인 (문자열 [] args) {
        새로운 SpringApplicationBuilder (Application.class) .web (true) .run (args);
    }

}

@구성 요소
공용 클래스 StoreIntegration {

    @HystrixCommand (fallbackMethod = "defaultStores")
    공용 객체 getStores (Map <String, Object> 매개 변수) {
        // 실패 할 수있는 일을하십시오.
    }

    공용 객체 defaultStores (Map <String, Object> 매개 변수) {
        return / * 유용한 정보 * /;
    }
}</pre>







이 `@HystrixCommand`라는 넷플 릭스있는 contrib 라이브러리에서 제공하는 ["javanica"](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica) . 스프링 클라우드는 Hystrix 회로 차단기에 연결된 프록시에서 주석을 사용하여 스프링 빈을 자동으로 래핑합니다. 회로 차단기는 회로를 열고 닫는시기와 고장이 발생할 경우 수행 할 작업을 계산합니다.





를 구성하려면 `@HystrixCommand`당신은 사용할 수 `commandProperties` 의 목록 속성을 `@HystrixProperty`주석. 참조하십시오 [여기에](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica#configuration) 자세한 내용은. 참고 항목 [Hystrix 위키](https://github.com/Netflix/Hystrix/wiki/Configuration) 사용할 수있는 속성에 대한 자세한 내용을.





### 보안 컨텍스트 전파 또는 스프링 스코프 사용



당신은 어떤 스레드 로컬 컨텍스트가에 전파하려는 경우 `@HystrixCommand`는 (시간 초과의 경우) 스레드 풀에서 명령을 실행하기 때문에 작동하지 않습니다 디폴트 선언. 일부 구성을 사용하여 발신자와 동일한 스레드를 사용하거나 주석에서 다른 "격리 전략"을 사용하도록 요청하여 Hystrix를 전환 할 수 있습니다. 예 :







    @HystrixCommand(fallbackMethod = "stubMyService",
        commandProperties = {
          @HystrixProperty(name="execution.isolation.strategy", value="SEMAPHORE")
        }
    )
    ...







당신이 사용하는 경우 같은 일이 적용 `@SessionScope`나 `@RequestScope`. 범위가 지정된 컨텍스트를 찾을 수 없다는 런타임 예외 때문에이 작업을 수행해야하는시기를 알 수 있습니다.







### 건강 지표



접속 회로 차단기의 상태도에 노출되어 `/health`호출 애플리케이션의 엔드 포인트.







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



Hystrix 메트릭 스트림을 사용하려면에 대한 종속성을 포함한다 `spring-boot-starter-actuator`. 이 노출됩니다 `/hystrix.stream`관리 엔드 포인트로.







        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-actuator</artifactId>
        </dependency>













## 회로 차단기 : Hystrix 대시 보드





Hystrix의 주요 이점 중 하나는 각 HystrixCommand에 대해 수집하는 일련의 메트릭입니다. Hystrix Dashboard는 각 회로 차단기의 상태를 효율적으로 표시합니다.





![Hystrix](./spring-cloud-doc-images/Hystrix.png)

그림 3\. Hystrix 대시 보드





Hystrix 대시 보드와 봄 부트 메인 클래스에 주석을 실행합니다 `@EnableHystrixDashboard`. 그런 다음 방문 `/hystrix`및 개별 인스턴스에 대시 보드를 가리 `/hystrix.stream`Hystrix 클라이언트 응용 프로그램에서 엔드 포인트.





### 터빈



개별 인스턴스를 보면 Hystrix 데이터는 시스템의 전반적인 상태와 관련하여별로 유용하지 않습니다. [터빈](https://github.com/Netflix/Turbine) 관련 모든 집계하는 응용 프로그램입니다 `/hystrix.stream`결합으로 엔드 포인트를 `/turbine.stream`Hystrix 대시 보드에 사용. 개별 인스턴스는 Eureka를 통해 위치합니다. 터빈을 실행하면 사용하여 메인 클래스에 주석을만큼 간단하다 `@EnableTurbine`(예를 들어, 클래스 경로를 설정하는 스프링 클라우드 스타터 터빈을 사용하여) 주석. 에서 문서화 된 구성 등록 정보의 모든 [터빈 1 위키](https://github.com/Netflix/Turbine/wiki/Configuration-(1.x)) 적용됩니다. 유일한 차이점은이 있다는 것입니다 `turbine.instanceUrlSuffix`이 자동으로하지 않는 한 처리로 앞에 추가 포트를 필요로하지 않는다 `turbine.instanceInsertPort=false`.





구성 키는 `turbine.appConfig`터빈 인스턴스를 조회하는 데 사용할 유레카 serviceIds의 목록입니다. : 터빈 스트림은 다음과 같은 URL을 사용 Hystrix 대시 보드에 사용된다 `[http://my.turbine.sever:8080/turbine.stream?cluster=<CLUSTERNAME>](http://my.turbine.sever:8080/turbine.stream?cluster=%3CCLUSTERNAME%3E);`(클러스터 파라미터 이름이 "기본"인 경우 생략 될 수있다)를. `cluster`매개 변수의 항목과 일치해야합니다 `turbine.aggregator.clusterConfig`. eureka에서 반환 된 값은 대문자이므로 Eureka에 등록 된 앱이 '고객'인 경우이 예제가 작동 할 것으로 기대합니다.







<pre>터빈:
  어 그리 게이터 :
    clusterConfig : 고객
  appConfig : 고객</pre>







은 `clusterName`에 SPEL 표현하여 사용자 정의 할 수 있습니다 `turbine.clusterNameExpression`루트의 인스턴스 `InstanceInfo`. 기본값은 `appName`유레카 서비스 id합니다 (즉, 클러스터 키로 끝 즉, `InstanceInfo`고객이있다 `appName`"고객"의 참조). 각기 다른 예로들 수 `turbine.clusterNameExpression=aSGName`AWS ASG 이름에서 클러스터 이름을 얻을 것이다. 다른 예 :







<pre>터빈:
  어 그리 게이터 :
    clusterConfig : SYSTEM, USER
  appConfig : 고객, 상점, UI, 관리자
  clusterName 표현식 : metadata [ 'cluster']</pre>







이 경우 4 개 서비스의 클러스터 이름은 메타 데이터 맵에서 가져오고 "SYSTEM"및 "USER"가 포함 된 값이 있어야합니다.





모든 응용 프로그램에 "기본"클러스터를 사용하려면 작은 따옴표로 묶인 문자열 리터럴 표현식이 필요합니다.







<pre>터빈:
  appConfig : 고객, 상점
  clusterNameExpression : '기본'</pre>







봄 클라우드가 제공하는 `spring-cloud-starter-turbine`당신은 터빈 서버를 실행 얻기 위해 필요한 모든 종속성을 갖는다. 그냥 봄 부팅 응용 프로그램을 작성하고 그것을 주석 `@EnableTurbine`.







### 터빈 AMQP



일부 환경 (예 : PaaS 설정)에서는 모든 분산 Hystrix 명령에서 메트릭을 가져 오는 클래식 터빈 모델이 작동하지 않습니다. 이 경우 Hystrix가 Turbine에 메트릭을 푸시하게하고 Spring Cloud에서 AMQP 메시징으로 메트릭을 푸시 할 수 있습니다. 클라이언트에 할 필요가 종속성을 추가 할 것입니다 `spring-cloud-netflix-hystrix-amqp`및 사용할 수있는 토끼 브로커가 있는지 확인합니다 (클라이언트 자격 증명을 구성하는 방법에 대한 자세한 내용은 봄 부트 설명서를 참조하지만, 로컬 브로커 상자 밖으로 작동합니다 또는 Cloud Foundry에서).





서버 측에서 그냥 봄 부팅 응용 프로그램을 작성하고 그것을 주석 `@EnableTurbineAmqp`과 기본적으로 포트 8989에 올 것이다 (모든 경로, 해당 포트에 Hystrix 대시 보드를 가리 킵니다). 당신이 중 하나를 사용하여 포트를 사용자 정의 할 수 있습니다 `server.port`또는 `turbine.amqp.port`. 당신이있는 경우 `spring-boot-starter-web`및 `spring-boot-starter-actuator`뿐만 아니라 클래스 패스에, 당신은 제공 (기본적으로 톰캣)와 별도의 포트에 액추에이터 엔드 포인트를 열 수있는 `management.port`다른 어떤을.





그런 다음 개별 Hystrix 스트림 대신 Hystrix Dashboard를 Turbine AMQP Server로 지정할 수 있습니다. 터빈 AMQP는 myhost의 포트 8989에서 실행중인 경우, 다음 넣어 `[http://myhost:8989](http://myhost:8989/)`Hystrix 대시 보드에서 스트림 입력 필드에. 회선은 각각의 serviceId가 접두어로 붙고 그 뒤에 점과 회로 이름이옵니다.





봄 클라우드가 제공하는 `spring-cloud-starter-turbine-amqp`당신은 터빈 AMQP 서버를 실행 얻기 위해 필요한 모든 종속성을 갖는다. Netty 기반이기 때문에 Java 8이 필요합니다.











## AMQP ConnectionFactory 사용자 정의





당신이 AMQP를 사용하는 경우가있을 필요가 `ConnectionFactory`응용 프로그램 컨텍스트 (봄 토끼에서). 하나 있으면 `ConnectionFactory`그 사용될 또는 자격 하나 존재하는 경우 `@HystrixConnectionFactory`(클라이언트)와 `@TurbineConnectionFactory`,이 다른 것보다 바람직 할 것이다 (서버), 그렇지 않으면 `@Primary`하나가 사용된다. 규정되지 않은 연결 팩토리가 여러 개 있으면 오류가 발생합니다.





(1.2.2 기준) 봄 부팅이 생성하는 주 `ConnectionFactory`입니다 _하지_ `@Primary` 당신이 버스를 하나의 연결 팩토리를 사용하려는 다른 비즈니스 메시지, 당신은 둘 다 작성하고 주석을해야합니다 그래서 만약, `@*ConnectionFactory`그리고 `@Primary`각각을.









## 클라이언트 측로드 밸런서 : 리본





리본은 HTTP 및 TCP 클라이언트의 동작을 제어 할 수있는 클라이언트 측로드 밸런서입니다. 당신이 사용하는, 그래서 만약 이미 리본을 사용 꾀병 `@FeignClient`다음이 섹션에도 적용됩니다.





리본의 중심 개념은 명명 된 클라이언트의 개념입니다. (예를 사용하여 각 부하 분산 장치는 필요에 따라 원격 서버에 접속하기 위해 함께 작동 구성 요소의 앙상블의 일부, 그리고 앙상블은 응용 프로그램 개발자로주는 이름을 가진 `@FeignClient` 주석). Spring Cloud은 같은 새로운 앙상블 작성 `ApplicationContext`하여 명명 된 각 클라이언트에 대한 수요를 `RibbonClientConfiguration`. 이것은 (다른 것들 중에서)를 포함 `ILoadBalancer`하는 `RestClient`, 및 `ServerListFilter`.





### 리본 클라이언트 사용자 정의



당신은 외부 속성을 사용하여 리본 클라이언트의 일부 비트를 구성 할 수 있습니다 `<client>.ribbon.*`당신은 봄 부팅 구성 파일을 사용할 수있는 것을 제외하고는 기본적으로 넷플 릭스 API를 사용하는 것보다 더 차이가없는. 기본 옵션은 정적 필드로 검사 할 수있다 `CommonClientConfigKey`(리본 코어의 일부).





Spring Cloud은 또한 당신 (의 위에 추가 구성을 선언하여 클라이언트의 모든 권한 걸릴 수 있습니다 `RibbonClientConfiguration`사용) `@RibbonClient`. 예:







    @Configuration
    @RibbonClient(name = "foo", configuration = FooConfiguration.class)
    public class TestConfiguration {
    }







이 경우 클라이언트가 이미 구성 요소로 구성되어 `RibbonClientConfiguration`어느와 함께 `FooConfiguration` (후자는 일반적으로 이전보다 우선합니다 경우).











<td class="icon">

경고



<td class="content">이 `FooConfiguration`있어야한다 `@Configuration`하지만이 아닌 관리 걸릴 `@ComponentScan`그렇지 않으면 모두에 의해 공유됩니다, 기본 응용 프로그램 컨텍스트를 `@RibbonClients`. 당신이 사용하는 경우 `@ComponentScan`(또는 `@SpringBootApplication`당신이 포함되지 않도록하기위한 조치를 취할 필요) (예를 들어 별도의 겹치지 않는 패키지에 넣어, 또는 명시 적으로 검사 할 패키지를 지정 `@ComponentScan`).











봄 클라우드 넷플릭스는 리본 기본적으로 (다음 콩을 제공 `BeanType`beanName에을 : `ClassName`)





*   `IClientConfig` ribbonClientConfig : `DefaultClientConfigImpl`

*   `IRule` ribbonRule : `ZoneAvoidanceRule`

*   `IPing` ribbonPing : `NoOpPing`

*   `ServerList<Server>` ribbonServerList : `ConfigurationBasedServerList`

*   `ServerListFilter<Server>` ribbonServerListFilter : `ZonePreferenceServerListFilter`

*   `ILoadBalancer` ribbonLoadBalancer : `ZoneAwareLoadBalancer`





그 유형 중 하나의 콩 만들기 및에 배치 `@RibbonClient` 구성하면 (예 : `FooConfiguration`위)가 설명 된 콩의 각각을 대체 할 수 있습니다. 예:







    @Configuration
    public class FooConfiguration {
        @Bean
        public IPing ribbonPing(IClientConfig config) {
            return new PingUrl();
        }
    }







이것은 대체 `NoOpPing`와 함께 `PingUrl`.







### 유레카와 함께 리본 사용하기



유레카는 리본 상기와 함께 사용하는 경우 `ribbonServerList` 의 확장으로 오버라이드 (override) `DiscoveryEnabledNIWSServerList` 유레카에서 서버 목록을 채 웁니다있다. 또한 대체 `IPing`와 인터페이스 `NIWSDiscoveryPing`서버가있는 경우 유레카 명 규모가 결정되는합니다. `ServerList`기본적으로 설치되는이 인 `DomainExtractingServerList`이의 목적은 (넷플 릭스에 의존하는 것입니다) AWS AMI 메타 데이터를 사용하지 않고 부하 분산 장치에 대한 물리적 메타 데이터를 사용할 수 있도록하는 것입니다. 기본적으로 서버 목록 "영역"(있도록 클라이언트 집합 인스턴스 메타 데이터에 제공된 정보로 구성된다 `eureka.instance.metadataMap.zone`), 및 경우는 (영역 프록시 서버의 호스트 이름의 도메인 이름을 사용할 수없는 것 인 경우 플래그 `approximateZoneFromHostname`)가 설정됩니다. 영역 정보를 사용할 일단이 사용될 수있다 `ServerListFilter`(기본이 때문에 클라이언트와 동일한 영역에있는 서버를 찾는 데 기본적으로 사용한다 `ZonePreferenceServerListFilter`).







### 예 : 유레카가없는 리본 사용법



Eureka는 원격 서버의 발견을 추상화하는 편리한 방법이므로 클라이언트에 URL을 하드 코딩 할 필요는 없지만 사용하지 않으려는 경우에도 Ribbon 및 Feign은 여전히 ​​사용하기 쉽습니다. 당신이 선언 한 가정 `@RibbonClient`"매장"에 대한, 그리고 유레카는 (심지어 클래스 패스가 아닌)를 사용하지 않을 것입니다. 리본 클라이언트는 기본적으로 구성된 서버 목록으로 구성되며 다음과 같은 구성을 제공 할 수 있습니다





application.yml



<pre>백화점:
  리본:
    listOfServers : example.com, google.com</pre>









### 예 : 리본에서 유레카 사용을 비활성화합니다.



속성을 설정하면 `ribbon.eureka.enabled = false`명시 적으로 리본에서 유레카의 사용을 중지됩니다.





application.yml



<pre>리본:
  유레카:
   enabled : false</pre>









### 리본 API를 직접 사용



당신은 또한 사용할 수 있습니다 `LoadBalancerClient`직접. 예:







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





[꾀병은](https://github.com/Netflix/feign) 선언적 웹 서비스 클라이언트이다. 따라서 웹 서비스 클라이언트를 쉽게 작성할 수 있습니다. Feign을 사용하려면 인터페이스를 만들고 주석을 달아 라. Feign 주석과 JAX-RS 주석을 포함하는 플러그 가능한 주석 지원 기능을 제공합니다. Feign은 또한 플러그 형 인코더와 디코더를 지원합니다. Spring Cloud 스프링 MVC 주석과 같은 사용에 대한 지원을 추가 `HttpMessageConverters`봄 웹에서 기본적으로 사용합니다. Spring Cloud는 Ribbon과 Eureka를 통합하여 Feign을 사용할 때로드 밸런싱 된 HTTP 클라이언트를 제공합니다.





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







에서 `@FeignClient`주석 문자열 값 ( "저장"위)는 리본로드 밸런서 (참조 만드는 데 사용되는 임의의 클라이언트 이름입니다 [리본 지원 자세한 내용은 아래를](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon) ). 또한 사용하여 URL을 지정할 수 있습니다 `url`속성 (절대 값 또는 그냥 호스트 이름).





위의 리본 클라이언트는 "상점"서비스의 실제 주소를 검색하려고합니다. 응용 프로그램이 유레카 클라이언트 인 경우 유레카 서비스 레지스트리의 서비스가 해결됩니다. 당신은 유레카를 사용하지 않으려면, 당신은 단순히 외부 구성 (참조에서 서버 목록을 구성 할 수 있습니다 [예를 들어 위](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon-without-eureka) ).





### 기본 값 재정의



Spring Cloud의 Feign 지원의 핵심 개념은 명명 된 클라이언트의 개념입니다. 각 꾀병 클라이언트는 필요에 따라 원격 서버에 접속하기 위해 함께 작동 구성 요소의 앙상블의 일부이며, 앙상블 당신이 사용하는 응용 프로그램 개발자로 제공 이름이 `@FeignClient`주석을. Spring Cloud은 같은 새로운 앙상블 작성 `ApplicationContext`하여 명명 된 각 클라이언트에 대한 수요를 `FeignClientsConfiguration`. 이것은 (다른 것들 중에서)를 포함 `feign.Decoder`하는 `feign.Encoder`, 및 `feign.Contract`.





봄 클라우드는 (의 위에 추가 구성 선언함으로써 꾀병 클라이언트의 전체 제어 할 수 있습니다 `FeignClientsConfiguration`) 사용하여 `@FeignClient`. 예:







    @FeignClient(name = "stores", configuration = FooConfiguration.class)
    public interface StoreClient {
        //..
    }







이 경우 클라이언트가 이미 구성 요소로 구성되어 `FeignClientsConfiguration`어떤과 함께 `FooConfiguration`(후자가 전자보다 우선합니다 경우).











<td class="icon">

경고



<td class="content">이 `FooConfiguration`있어야한다 `@Configuration`하지만이 아닌 관리 걸릴 `@ComponentScan`그렇지 않으면 모든 사용됩니다, 기본 응용 프로그램 컨텍스트를 `@FeignClient`. 당신이 사용하는 경우 `@ComponentScan`(또는 `@SpringBootApplication`당신이 포함되지 않도록하기위한 조치를 취할 필요) (예를 들어 별도의 겹치지 않는 패키지에 넣어, 또는 명시 적으로 검사 할 패키지를 지정 `@ComponentScan`).

















<td class="icon">

노트



<td class="content">`serviceId`속성은 이제 찬성되지 않습니다 `name`속성.

















<td class="icon">

경고



<td class="content">이전에는 사용 `url`속성은 필요하지 않은 `name`속성을. 사용하는 것이 `name`지금 필요합니다.











자리가 지원됩니다 `name`및 `url`속성.







    @FeignClient(name = "${feign.name}", url = "${feign.url}")
    public interface StoreClient {
        //..
    }







봄 클라우드 넷플릭스는 꾀병을 위해 기본적으로 다음 콩 제공 ( `BeanType`beanName에을 : `ClassName`)





*   `Decoder`feignDecoder : `ResponseEntityDecoder`(래핑 `SpringDecoder`)

*   `Encoder` feignEncoder : `SpringEncoder`

*   `Logger` feignLogger : `Slf4jLogger`

*   `Contract` feignContract : `SpringMvcContract`

*   `Feign.Builder` feignBuilder : `HystrixFeign.Builder`





봄 클라우드 넷플릭스는 _하지 않습니다_ 꾀병 기본적으로 다음 콩을 제공하지만 여전히 꾀병 클라이언트를 만들 수있는 응용 프로그램 컨텍스트에서 이러한 종류의 콩을 검색 :





*   `Logger.Level`

*   `Retryer`

*   `ErrorDecoder`

*   `Request.Options`

*   `Collection<RequestInterceptor>`





그 유형 중 하나의 콩 만들기 및에 배치 `@FeignClient`구성하면 (예 : `FooConfiguration`위)가 설명 된 콩의 각각을 대체 할 수 있습니다. 예:







    @Configuration
    public class FooConfiguration {
        @Bean
        public Contract feignContractg() {
            return new feign.Contract.Default();
        }

        @Bean
        public BasicAuthRequestInterceptor basicAuthRequestInterceptor() {
            return new BasicAuthRequestInterceptor("user", "password");
        }
    }







이 대체 `SpringMvcContract`로 `feign.Contract.Default`하고, 추가 `RequestInterceptor`의 컬렉션 `RequestInterceptor`.





기본 구성이 지정 될 수있는 `@EnableFeignClients`특성을 `defaultConfiguration`상술 한 바와 같이 유사한 방식. 차이점은이 구성에 적용 할 것입니다 _모든_ 꾀병 클라이언트.







### Hystrix 지원 지원



Hystrix가 classpath에 있다면, 기본적으로 Feign은 모든 메소드를 회로 차단기로 감쌀 것이다. 을 반환하는 `com.netflix.hystrix.HystrixCommand`도 사용할 수 있습니다. 이렇게하면에 호출 (반응 패턴을 사용할 수 있습니다 `.toObservable()`하거나 `.observe()`또는 호출과 비동기 사용 ( `.queue()`).





척하기위한 Hystrix 지원을 사용하지 않으려면 설정 `feign.hystrix.enabled=false`.





클라이언트 당 기준으로 Hystrix 지원을 비활성화하려면 바닐라 작성 `Feign.Builder`은 "프로토 타입"범위, 예를 들면와를 :







    @Configuration
    public class FooConfiguration {
        @Bean
        @Scope("prototype")
        public Feign.Builder feignBuilder() {
            return Feign.builder();
        }
    }









### Hystrix Fallbacks를 기쁘게합니다.



Hystrix는 회로가 열려 있거나 오류가있을 때 실행되는 기본 코드 경로 인 폴백의 개념을 지원합니다. A는 주어진에 대한 폴백을 사용하려면 `@FeignClient`설정된 `fallback`대체를 구현하는 클래스의 이름 속성을.







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













<td class="icon">

경고



<td class="content">Feign의 대체 기능 구현과 Hystrix 대체 버전의 작동 방식에는 제한이 있습니다. 폴백은 현재 반환 방법에 대해 지원되지 않습니다 `com.netflix.hystrix.HystrixCommand`및 `rx.Observable`.













### 기꺼이 상속 지원



Feign은 단일 상속 인터페이스를 통해 상용구 API를 지원합니다. 이를 통해 공통 작업을 편리한 기본 인터페이스로 그룹화 할 수 있습니다. Spring MVC와 함께 REST 엔드 포인트와 Feign 클라이언트에 대해 동일한 계약을 공유 할 수있다.





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









### 희망 요청 / 응답 압축



귀하는 귀하의 Feign 요청에 대해 요청 또는 응답 GZIP 압축을 활성화하는 것을 고려할 수 있습니다. 다음 중 하나의 특성을 사용하여이를 수행 할 수 있습니다.







    feign.compression.request.enabled=true
    feign.compression.response.enabled=true







긴급 요청 압축을 사용하면 웹 서버에 설정할 수있는 것과 비슷한 설정을 사용할 수 있습니다.







    feign.compression.request.enabled=true
    feign.compression.request.mime-types=text/xml,application/xml,application/json
    feign.compression.request.min-request-size=2048







이러한 등록 정보를 사용하면 압축 미디어 유형 및 최소 요청 임계 값 길이에 대한 선택을 할 수 있습니다.







### 벌채 로깅



작성된 각 Feign 클라이언트에 대해 로거가 작성됩니다. 기본적으로 로거 이름은 Feign 클라이언트를 만드는 데 사용 된 인터페이스의 전체 클래스 이름입니다. 척하기 로깅 만에 응답 `DEBUG`수준.





application.yml



    logging.level.project.user.UserClient: DEBUG







`Logger.Level`는 클라이언트에 따라 구성 할 수 있습니다 목적은, 얼마를 기록하는 척하기 알려줍니다. 선택 사항은 다음과 같습니다.





*   `NONE`아니, 로깅 ( **DEFAULT** ).

*   `BASIC`, 요청 메소드와 URL 및 응답 상태 코드와 실행 시간 만 로깅하십시오.

*   `HEADERS`, 요청 및 응답 헤더와 함께 기본 정보를 기록하십시오.

*   `FULL`, 요청과 응답에 대한 헤더, 본문 및 메타 데이터를 기록합니다.





예를 들어, 다음을 설정할 것이다 `Logger.Level`하기 `FULL`:







    @Configuration
    public class FooConfiguration {
        @Bean
        Logger.Level feignLoggerLevel() {
            return Logger.Level.FULL;
        }
    }













## 외부 구성 : Archaius





[Archaius는](https://github.com/Netflix/archaius) 넷플 릭스 클라이언트 측 구성 라이브러리입니다. 모든 Netflix OSS 구성 요소가 구성에 사용하는 라이브러리입니다. Archaius는의 확장 [아파치 코 몬즈 구성](https://commons.apache.org/proper/commons-configuration) 프로젝트. 소스를 폴링하여 변경 사항을 보거나 소스가 변경 사항을 클라이언트에 푸시하여 구성을 갱신 할 수 있습니다. Archaius는 동적 <Type> 속성 클래스를 속성의 핸들로 사용합니다.





아키라 우스의 예



    class ArchaiusTest {
        DynamicStringProperty myprop = DynamicPropertyFactory
                .getInstance()
                .getStringProperty("my.prop");

        void doSomething() {
            OtherClass.someMethod(myprop.get());
        }
    }







Archaius는 고유 한 구성 파일 세트 및로드 우선 순위를 가지고 있습니다. Spring 애플리케이션은 일반적으로 Archaius를 직접 사용하지 않아야하지만 Netflix 툴을 기본적으로 구성해야 할 필요성은 여전히 ​​남아 있습니다. Spring Cloud에는 Spring Environment Bridge가있어서 Archaius는 Spring Environment로부터 속성을 읽을 수 있습니다. 이를 통해 스프링 부트 프로젝트는 일반 구성 툴체인을 사용하면서 문서화 된대로 Netflix 툴을 구성 할 수 있습니다.









## 라우터 및 필터 : Zuul





마이크로 서비스 아키텍처의 필수 부분에서 라우팅. 예를 들어, `/`웹 어플리케이션에 매핑 될 수 있고, `/api/users`사용자의 서비스에 대응하고, `/api/shop`점포 서비스 매핑된다. [Zuul는](https://github.com/Netflix/zuul) 넷플릭스에 의해 JVM 기반의 라우터와 서버 측 부하 분산 장치입니다.





[넷플릭스는 Zuul을 사용하여](http://www.slideshare.net/MikeyCohen1/edge-architecture-ieee-international-conference-on-cloud-engineering-32240146/27) 다음과 같은 사항에 대해 :





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





### 임베디드 Zuul 역방향 프록시



Spring Cloud는 UI 애플리케이션이 하나 이상의 백엔드 서비스에 대한 호출을 프록시하기를 원하는 매우 일반적인 사용 사례의 개발을 용이하게하기 위해 임베디드 Zuul 프록시를 만들었습니다. 이 기능은 필요한 모든 백엔드에 대해 독립적으로 CORS 및 인증 문제를 관리 할 필요가 없도록 사용자 인터페이스가 필요한 백엔드 서비스로 프록시 할 때 유용합니다.





그것을 사용하려면, 함께 봄 부트 메인 클래스에 주석 `@EnableZuulProxy`, 이는 해당 서비스에 시내 전화를 전달합니다. 규칙에 따라, 유레카 ID "사용자"와 서비스에있는 프록시의 요청받을 것 `/users`(제거 접두사와 참조). 프록시는 Eureka를 통해 전달할 인스턴스를 찾기 위해 리본을 사용하며 모든 요청은 hystrix 명령으로 실행되므로 Hystrix 메트릭에 실패가 표시되고 일단 회로가 열리면 프록시는 서비스에 접속하려고 시도하지 않습니다.





설정 자동으로 추가 서비스 갖는 건너 뛰려면 `zuul.ignored-services`서비스 ID 패턴 목록에 있습니다. 서비스가 무시되고 명시 적으로 구성된 라우트 맵에 포함 된 패턴과 일치하면 무시되지 않습니다. 예:





application.yml



     zuul:
      ignoredServices: '*'
      routes:
        users: /myusers/**







이 예에서, 모든 서비스가 무시되는 **것을 제외하고** '사용자'.





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







이것은 "/ myusers"에 대한 http 호출이 "users_service"서비스로 전달됨을 의미합니다. 라우트에는 개미 스타일 패턴으로 지정할 수있는 "경로"가 있어야하므로 "/ myusers / *"는 하나의 레벨과 만 일치하지만 "/ myusers / {asterisk} {별표}"는 계층 적으로 일치합니다.





백엔드의 위치는 "serviceId"(유레카 서비스의 경우) 또는 "url"(물리적 위치의 경우)으로 지정할 수 있습니다.





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          url: http://example.com/users_service







이 간단한 url-routes는 HystrixCommand처럼 실행되지 않으며 다중 URL을 리본으로로드 밸런싱 할 수 없습니다. (이것은 현재 리본에서 해제 유레카 지원이 필요합니다 : 참조 서비스-경로를 지정하고 서비스 id를위한 리본 클라이언트를 구성이를 위해 [자세한 정보는 위](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon-without-eureka) ), 예를 들어,





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







regexmapper를 사용하여 serviceId와 route 사이에 규칙을 제공 할 수 있습니다. serviceId에서 변수를 추출하여 경로 패턴에 주입하기 위해 group이라는 정규 표현식을 사용합니다.





ApplicationConfiguration.java



    @Bean
    public PatternServiceRouteMapper serviceRouteMapper() {
        return new PatternServiceRouteMapper(
            "(?<name>^.+)-(?<version>v.+$)",
            "${version}/${name}");
    }







즉, serviceId "myusers-v1"은 "/ v1 / myusers / {asterisk} {별표}"경로에 매핑됩니다. 모든 정규식이 허용되지만 모든 명명 된 그룹은 servicePattern과 routePattern에 모두 있어야합니다. servicePattern이 serviceId와 일치하지 않으면 기본 동작이 사용됩니다. 위의 예에서 serviceId "myusers"는 경로 "/ myusers / {asterisk} {asterisk}"에 매핑됩니다 (버전이 없음).이 기능은 기본적으로 사용되지 않으며 발견 된 서비스에만 적용됩니다.





설정된 모든 매핑에 접두사를 추가하려면 `zuul.prefix`다음과 같은 값으로, `/api`. 요청이 기본적으로 전달되기 전에 프록시 접두사 (와 떨어져이 동작을 전환 요청에서 제거된다 `zuul.stripPrefix=false`). 개별 경로에서 서비스 별 접두어를 제거 할 수도 있습니다 (예 :





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          stripPrefix: false







이 예에서 "/ myusers / 101"에 대한 요청은 "users"서비스의 "/ myusers / 101"로 전달됩니다.





`zuul.routes`항목은 실제로 유형의 개체에 바인딩 `ProxyRouteLocator`. 해당 객체의 속성을 보면 "재시도"플래그도 있음을 알 수 있습니다. 해당 플래그를 "true"로 설정하면 리본 클라이언트가 실패한 요청을 자동으로 다시 시도합니다 (필요하면 리본 클라이언트 구성을 사용하여 재시도 작업의 매개 변수를 수정할 수 있음).





`X-Forwarded-Host`헤더는 기본적으로 전달 요청에 추가됩니다. 집합을 해제합니다 `zuul.addProxyHeaders = false`. 접두어 경로는 기본적으로 제거되고 백엔드에 대한 요청은 헤더 "X-Forwarded-Prefix"(위의 예에서 "/ myusers")를 선택합니다.





와 응용 프로그램은 `@EnableZuulProxy`당신이 기본 경로를 ( "/")로 설정하면 예를 들어, 독립 서버로 동작 할 수있다 `zuul.route.home: /`"홈"서비스 행 노선의 모든 트래픽 (예 : "/ {별표} {별표}") 할 것이다.





보다 세분화 된 무시가 필요할 경우 무시할 특정 패턴을 지정할 수 있습니다. 이 패턴은 라우트 위치 지정 프로세스의 시작에서 평가되는데, 이는 일치를 보장하기 위해 접두어가 패턴에 포함되어야 함을 의미합니다. 무시 된 패턴은 모든 서비스에 적용되며 다른 경로 사양보다 우선합니다.





application.yml



     zuul:
      ignoredPatterns: /**/admin/**
      routes:
        users: /myusers/**







즉, "/ myusers / 101"과 같은 모든 호출은 "users"서비스의 "/ 101"로 전달됩니다. 그러나 "/ admin /"을 포함한 전화는 해결되지 않습니다.







### 교살 패턴과 로컬 전달



기존 애플리케이션이나 API를 마이그레이션 할 때 일반적인 패턴은 이전 엔드 포인트를 "교살하여 다른 구현으로 천천히 대체하는 것"입니다. Zuul 프록시는 이전 엔드 포인트 클라이언트의 모든 트래픽을 처리하는 데 사용할 수 있기 때문에이 도구를 사용하면 유용하지만 일부 요청은 새 엔드 포인트로 리디렉션합니다.





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







이 예에서는 다른 패턴 중 하나와 일치하지 않는 모든 요청에 ​​매핑되는 '기존'앱을 차단하고 있습니다. 의 경로는 `/first/{asterisk}{asterisk}`외부 URL로 새로운 서비스로 추출되었다. 그리고에서 경로 `/second/{asterisk}{asterisk}`forwared있다 그래서 그들은 보통 봄과 예, 로컬로 처리 할 수 있습니다 `@RequestMapping`. 의 경로 `/third/{asterisk}{asterisk}`도 전달되지만, 다른 접두사로 (즉,이 `/third/foo`전달됩니다 `/3rd/foo`).











<td class="icon">

노트



<td class="content">무시 된 패턴은 완전히 무시되지 않고 프록시에 의해 처리되지 않습니다 (따라서 효과적으로 로컬로 전달됩니다).













### Zuul을 통한 파일 업로드



당신이 경우 `@EnableZuulProxy`당신은 파일을 업로드 할 프록시 경로를 사용할 수 있습니다 그리고 그것은 단지 한 파일이 작으로 작동합니다. 큰 파일의 경우 봄 우회 대안 경로가 `DispatcherServlet`"/ zuul / *"에 (다중 처리를 방지하기 위해). 즉, 만약 `zuul.routes.customers=/customers/{asterisk}{asterisk}`당신이 "/ zuul / 고객 / *"큰 파일을 게시 할 수 있습니다. 서블릿 경로를 통해 구체화된다 `zuul.servletPath`. 대용량 파일은 프록시 경로가 리본로드 밸런서를 통해 이동하는 경우 시간 초과 설정을 높여야합니다 (예 :





application.yml



    hystrix.command.default.execution.isolation.thread.timeoutInMilliseconds: 60000
    ribbon:
      ConnectTimeout: 3000
      ReadTimeout: 60000







스트리밍을 대용량 파일로 작업하려면 요청에서 청크 분할 인코딩을 사용해야합니다 (일부 브라우저에서는 기본적으로 수행하지 않음). 예 : 명령 줄에서 :







<pre>$ curl -v -H "전송 인코딩 : 청크 분할"\
    -F " file=@mylarge.iso"로컬 호스트 : 9999 / zuul / 간단한 / 파일</pre>









### Plain Embedded Zuul



당신이 사용하는 경우, 또한 프록시없이 Zuul 서버를 실행하거나, 선택적으로 프록시 플랫폼의 일부에 전환 할 수 있습니다 `@EnableZuulServer`(대신 `@EnableZuulProxy`). 만약 유형의 애플리케이션에 추가하는 콩 `ZuulFilter` 들이 함께 한, 자동적으로 설치된다 `@EnableZuulProxy`하지만 않고 프록시 필터 중 하나가 자동으로 추가된다.





이 경우 Zuul 서버에 대한 경로는 "zuul.routes. *"를 구성하여 계속 지정되지만 서비스 발견 및 프록시가 없으므로 "serviceId"및 "url"설정은 무시됩니다. 예 :





application.yml



     zuul:
      routes:
        api: /api/**







"/ api / {asterisk} {별표}"의 모든 경로를 Zuul 필터 체인에 매핑합니다.







### 주울 필터 사용 안 함



봄 클라우드에 대한 Zuul이 다수 포함되어 `ZuulFilter`모두 프록시 서버 모드에서 기본적으로 활성화 콩. 참조 [zuul 필터 패키지를](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/zuul/filters) 사용할 수 있습니다 가능한 필터에 대해. 당신이 하나를 사용하지 않으려면, 간단하게 설정 `zuul.<SimpleClassName>.<filterType>.disable=true`. 관례 적으로, 패키지는 후 `filters`Zuul 필터 유형입니다. 예를 들어 사용하지 않도록 설정하는 `org.springframework.cloud.netflix.zuul.filters.post.SendResponseFilter`설정 `zuul.SendResponseFilter.post.disable=true`.







### 사이드카로 다국어 지원



Eureka, Ribbon 및 Config Server를 활용하고자하는 jvm이 아닌 언어를 사용합니까? 봄 클라우드 넷플릭스 사이드카가 영감을받은 [넷플릭스 프라나](https://github.com/Netflix/Prana) . 여기에는 주어진 서비스에 대한 모든 인스턴스 (예 : 호스트 및 포트)를 가져 오는 간단한 http API가 포함되어 있습니다. Eureka에서 경로 항목을 가져온 Zuul 프록시를 통해 서비스 호출을 프록시 할 수도 있습니다. Spring Cloud Config Server는 호스트 조회 또는 Zuul 프록시를 통해 직접 액세스 할 수 있습니다. 비 jvm 앱은 헬스 체크를 구현하여 앱이 위 또는 아래로 움직이는 경우 사이드카가 eureka에보고 할 수 있도록해야합니다.





사이드카를 사용하려면, 함께 봄 부팅 응용 프로그램을 만듭니다 `@EnableSidecar`. 이 주석은 포함 `@EnableCircuitBreaker`, `@EnableDiscoveryClient`하고 `@EnableZuulProxy`. 비 -JVM 응용 프로그램과 같은 호스트에서 결과 응용 프로그램을 실행하십시오.





측면 차 추가 구성하려면 다음 `sidecar.port`과 `sidecar.health-uri`에를 `application.yml`. `sidecar.port`속성은 비 JVM 앱이 수신 대기하는 포트입니다. 이것은 사이드카가 앱을 유레카에 제대로 등록 할 수있게 해줍니다. 는 `sidecar.health-uri` 봄 부팅 상태 표시기를 mimicks 비 JVM을 응용 프로그램에 액세스 할 수있는 URI입니다. 다음과 같은 json 문서를 반환해야합니다.





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







에 대한 API를 `DiscoveryClient.getInstances()`하는 방법이다 `/hosts/{serviceId}`. 여기에 대한 예제 응답입니다 `/hosts/customers`즉 다른 호스트에 두 개의 인스턴스를 반환합니다. 에서 (사이드카가 포트 5678에있는 경우)이 API는 비 JVM을 응용 프로그램에 액세스 할 수 있습니다 `[http://localhost:5678/hosts/{serviceId}](http://localhost:5678/hosts/%7BserviceId%7D)`.





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







Zuul 프록시 자동으로 유레카에 공지 된 각 서비스에 대한 경로를 추가 `/<serviceId>`, 그래서 고객 서비스에서 확인할 수있다 `/customers`. 비 JVM을 앱을 통해 고객 서비스에 액세스 할 수 있습니다 `[http://localhost:5678/customers](http://localhost:5678/customers)` (사이드카가 포트 5678에서 수신 대기 가정).





구성 서버가 Eureka에 등록 된 경우 비 jvm 응용 프로그램은 Zuul 프록시를 통해 액세스 할 수 있습니다. ConfigServer의 서비스 id 인 경우 `configserver` 와 사이드카가 포트 5678에, 다음이에서 액세스 할 수 있습니다 [에 http : // localhost를 : 5678 / configserver](http://localhost:5678/configserver)





비 jvm 앱은 YAML 문서를 반환하는 구성 서버의 기능을 이용할 수 있습니다. 예를 들어, 호출 [http://sidecar.local.spring.io:5678/configserver/default-master.yml는](http://sidecar.local.spring.io:5678/configserver/default-master.yml) 다음과 같은 YAML 문서이 발생할 수 있습니다







    eureka:
      client:
        serviceUrl:
          defaultZone: http://localhost:8761/eureka/
      password: password
    info:
      description: Spring Cloud Samples
      url: https://github.com/spring-cloud-samples













## 통계 : 관중, 서보 및지도





Spectator / Servo와 Atlas를 함께 사용하면 거의 실시간 운영 통찰력을 제공합니다.





Spectator와 Servo는 Netflix의 메트릭 컬렉션 라이브러리입니다. Atlas는 차원 시계열 데이터를 관리하기위한 Netflix 메트릭 백엔드입니다.





Servo는 Netflix를 수년간 사용했으며 여전히 사용할 수 있지만 점차적으로 Java 8에서만 작동하도록 설계된 Spectator를 단계적으로 단계적으로 제거하고 있습니다. Spring Cloud Netflix는 둘 다 지원하지만 Java 8 기반 응용 프로그램은 Spectator .





### 차원 대 계층 적 메트릭 비교



스프링 부트 액츄에이터 메트릭은 계층 적이며 메트릭은 이름으로 만 구분됩니다. 이러한 이름은 종종 마침표로 구분 된 이름에 키 / 값 속성 쌍 (차원)을 포함하는 이름 지정 규칙을 따릅니다. root 및 star-star라는 두 개의 끝점에 대해 다음과 같은 측정 항목을 고려하십시오.







    {
        "counter.status.200.root": 20,
        "counter.status.400.root": 3,
        "counter.status.200.star-star": 5,
    }







첫 x 째 메트릭은 단위 시간당 루트 엔드 포인트에 대한 정상적인 요청 성공 횟수를 제공합니다. 그러나 시스템에 20 개의 엔드 포인트가 있고 모든 엔드 포인트에 대한 성공적인 요청 수가 필요한 경우에는 어떨까요? 일부 계층 통계 백엔드는 당신은 와일드 카드를 지정할 수있는 것 **그 모든 20 메트릭을 읽고 결과를 집계한다.** **또는, 당신은 제공 할 수있는** **것을 차단과 같은 메트릭 기록** **에 상관없이 엔드 포인트의 모든 성공적인 요청을하지만, 지금은 20 + 1 가지 통계를 작성해야합니다.** **이 서비스의 모든 엔드 포인트에 대한 성공적인 요청의 총 수를 알고 싶다면 마찬가지로 같은 와일드 카드를 지정할 수 있습니다** .`counter.status.200.`**`HandlerInterceptorAdapter``counter.status.200.all``counter.status.2`**`.*`





계층 적 메트릭 백엔드에서 와일드 카드 지원이 있더라도 명명 일관성은 어려울 수 있습니다. 특히 이름 문자열에있는 이러한 태그의 위치는 시간이지나면서 질의를 위반할 수 있습니다. 예를 들어 위의 계층 적 메트릭에 HTTP 메서드에 대해 추가 차원을 추가한다고 가정합니다. 그런 다음 `counter.status.200.root`이된다 없습니다 `counter.status.200.method.get.root`등 우리는 `counter.status.200.*`갑자기 더 이상 같은 의미 론적 의미를 가지고있다. 또한 새로운 차원이 코드베이스 전체에 균일하게 적용되지 않으면 특정 쿼리가 불가능해질 수 있습니다. 이것은 빨리 빠져 나갈 수 있습니다.





Netflix 측정 항목에는 태그가 지정됩니다 (일명 차원). 각 메트릭에는 이름이 있지만이 단일 메트릭에는 더 많은 쿼리 유연성을 허용하는 여러 통계 및 '태그'키 / 값 쌍이 포함될 수 있습니다. 실제로 통계 자체는 특수 태그에 기록됩니다.





Netflix Servo 또는 Spectator로 기록한 위에 설명 된 루트 끝점의 타이머에는 상태 코드 당 4 개의 통계가 포함됩니다. 여기서 카운트 통계는 Spring Boot Actuator의 카운터와 동일합니다. 지금까지 HTTP 200과 400이 발생했다면 사용 가능한 데이터 포인트는 8 개가됩니다.







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



추가 종속성 또는 구성하지 않고, 봄 클라우드 기반 서비스는 서보 자동 구성됩니다 `MonitorRegistry`모든 스프링 MVC 요청에 대한 통계 수집을 시작. 기본적으로, 이름 서보 타이머 `rest`태그 MVC 각 요청에 대해 기록한다 :





1.  HTTP 메소드

2.  HTTP 상태 (예 : 200, 400, 500)

3.  URI (URI가 비어 있으면 "root"), Atlas에 대해 살균 됨

4.  요청 처리기가 예외를 던진 경우 예외 클래스 이름

5.  발신자는 경우 키 일치와 요청 헤더는 `netflix.metrics.rest.callerHeader`요청에 설정되어 있습니다. 에 대한 기본 키가 없습니다 `netflix.metrics.rest.callerHeader`. 발신자 정보를 수집하려면 응용 프로그램 속성에 추가해야합니다.





설정 `netflix.metrics.rest.metricName`에서 메트릭의 이름을 변경하려면 속성을 `rest`사용자가 제공하는 이름.





스프링 AOP가 활성화되어있는 경우 `org.aspectj:aspectjweaver`런타임 클래스 경로에 존재하는, Spring Cloud도로 만든 모든 클라이언트 호출에 대한 통계를 수집합니다 `RestTemplate`. 의 이름을 가진 서보 타이머 `restclient`태그 각 MVC 요청에 대해 기록 될 것입니다 :





1.  HTTP 메소드

2.  HTTP 상태 (예 : 200, 500, 400)는이 경우 "CLIENT_ERROR"경우 응답이 널 (null), 또는 "IO_ERROR"반환 `IOException`의 실행 중에 발생 `RestTemplate`방법

3.  Atlas에 대해 살생 된 URI

4.  고객 이름







### 통계 수집 : 관중



구경꾼 통계를 사용하려면 종속성에 포함 `spring-boot-starter-spectator`:







        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-spectator</artifactId>
        </dependency>







Spectator 용어에서 미터는 명명 된, 입력 된 및 태그가있는 구성이고 메트릭은 특정 시점의 주어진 미터의 값을 나타냅니다. 관측기 미터는 현재 여러 가지 구현이있는 레지스트리에 의해 생성되고 제어됩니다. Spectator는 4 미터 유형을 제공합니다 : 카운터, 타이머, 게이지 및 분배 요약.





Spring Cloud 관객 통합은 주사 구성 `com.netflix.spectator.api.Registry`당신을 위해 인스턴스를. 구체적으로는 구성 `ServoRegistry`REST 통계의 수집 및 하나의 서보 API에서 아틀라스 백엔드에 대한 메트릭의 수출을 통합하기 위해 인스턴스를. 실제로,이 코드가 서보 모니터와 구경꾼 미터 모두 봄 부팅 액추에이터에 의해 훔쳐됩니다의 혼합물을 사용할 수 있다는 것을 의미 `MetricReader`인스턴스와 모두 아틀라스 백엔드로 배송됩니다.





#### 관중 카운터



카운터는 일부 이벤트가 발생하는 비율을 측정하는 데 사용됩니다.







    // create a counter with a name and a set of tags
    Counter counter = registry.counter("counterName", "tagKey1", "tagValue1", ...);
    counter.increment(); // increment when an event occurs
    counter.increment(10); // increment by a discrete amount







카운터는 단일 시간 정규화 통계를 기록합니다.







#### 관중 타이머



타이머는 일부 이벤트가 얼마나 오래 걸리는지 측정하는 데 사용됩니다. 봄 클라우드는 자동으로 조건부 스프링 MVC 요청과에 대한 타이머 기록 `RestTemplate`후 대기 시간 등의 요청 관련 통계에 대한 대시 보드를 만들 수 있습니다 요청을 :





대기 시간 요청

image :: RequestLatency.png []







    // create a timer with a name and a set of tags
    Timer timer = registry.timer("timerName", "tagKey1", "tagValue1", ...);

    // execute an operation and time it at the same time
    T result = timer.record(() -> fooReturnsT());

    // alternatively, if you must manually record the time
    Long start = System.nanoTime();
    T result = fooReturnsT();
    timer.record(System.nanoTime() - start, TimeUnit.NANOSECONDS);







타이머는 count, max, totalOfSquares 및 totalTime의 4 가지 통계를 동시에 기록합니다. 카운트 통계는 항상 호출 한 경우 카운터에서 제공하는 하나의 정규화 된 값과 일치합니다 `increment()`당신은 타이밍을 기록 할 때마다의 카운터에 한 번을, 그래서 하나의 작업에 대해 개별적으로 계산하고 시간에 거의 필요하지 않습니다.





들어 [장기 실행 작업](https://github.com/Netflix/spectator/wiki/Timer-Usage#longtasktimer) , 관객은 특별한을 제공합니다 `LongTaskTimer`.







#### 스펙 테이터 게이지



게이지는 실행중인 상태의 대기열 또는 스레드 수와 같은 현재 값을 결정하는 데 사용됩니다. 게이지는 샘플링되므로 샘플간에 이러한 값이 변동하는 방식에 대한 정보는 제공하지 않습니다.





게이지의 정상적인 사용에는 초기화시 ID, 샘플링 할 객체에 대한 참조, 객체를 기반으로 숫자 값을 가져 오거나 계산하는 함수를 사용하여 게이지를 등록하는 작업이 포함됩니다. 객체에 대한 참조는 별도로 전달되며 Spectator 레지스트리는 객체에 대한 약한 참조를 유지합니다. 객체가 가비지 수집 된 경우 Spectator는 자동으로 등록을 삭제합니다. 참조 [노트](https://github.com/Netflix/spectator/wiki/Gauge-Usage#using-lambda) 이 API가 잘못 사용되는 경우 잠재적 메모리 누수에 대한 관객의 문서를.







    // the registry will automatically sample this gauge periodically
    registry.gauge("gaugeName", pool, Pool::numberOfRunningThreads);

    // manually sample a value in code at periodic intervals -- last resort!
    registry.gauge("gaugeName", Arrays.asList("tagKey1", "tagValue1", ...), 1000);









#### 관람객 분포 요약



분배 요약은 이벤트 분배를 추적하는 데 사용됩니다. 이것은 타이머와 비슷하지만 크기가 일정 시간 일 필요는 없다는 점에서보다 일반적입니다. 예를 들어, 분배 요약은 서버에 도달하는 요청의 페이로드 크기를 측정하는 데 사용될 수 있습니다.







    // the registry will automatically sample this gauge periodically
    DistributionSummary ds = registry.distributionSummary("dsName", "tagKey1", "tagValue1", ...);
    ds.record(request.sizeInBytes());











### 통계 수집 : 서보









<td class="icon">

경고



<td class="content">코드가 Java 8에서 컴파일 된 경우, 관측자로 Servo 대신 Spectator를 사용하면 장기간에 걸쳐 Servo를 완전히 대체 할 예정입니다.











Servo 구문에서 모니터는 명명 된 유형 지정 및 태그가 지정된 구성이며 메트릭은 특정 시점의 특정 모니터 값을 나타냅니다. 서보 모니터는 관측기 미터와 논리적으로 동일합니다. 서보 모니터 생성 및에 의해 제어된다 `MonitorRegistry`. 위의 경고에도 불구하고, 서보는 있는가 [넓은 배열](https://github.com/Netflix/servo/wiki/Getting-Started) 관객이 미터가보다 모니터 옵션을.





봄 클라우드 통합은 주사 구성 `com.netflix.servo.MonitorRegistry`당신을 위해 인스턴스를. 적절한 만든 후에 `Monitor`서보의 유형을, 데이터를 기록하는 과정은 관객에 전적으로 유사하다.





#### 서보 모니터 만들기



당신은 서보 사용하는 경우 `MonitorRegistry`(특히, 인스턴스 봄 클라우드에서 제공하는 인스턴스 `DefaultMonitorRegistry`), 서보 검색 편의 클래스를 제공 [카운터](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamiccounter) 및 [타이머를](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamictimer) . 이러한 편리한 클래스는 하나가되도록 `Monitor`이름과 태그의 고유 한 각 조합에 등록됩니다.





수동으로, 특히 편리한 메소드가 제공되지 않은, 더 이국적인 모니터 유형, 서보의 모니터 유형을 만들 제공하여 적절한 유형의 인스턴스를 `MonitorConfig`인스턴스를 :







    MonitorConfig config = MonitorConfig.builder("timerName").withTag("tagKey1", "tagValue1").build();

    // somewhere we should cache this Monitor by MonitorConfig
    Timer timer = new BasicTimer(config);
    monitorRegistry.register(timer);











### 메트릭 백엔드 : Atlas



Atlas는 Netflix에서 거의 실시간 운영 통찰력을위한 차원 시계열 데이터를 관리하기 위해 개발되었습니다. Atlas는 메모리 내 데이터 스토리지를 특징으로하며 매우 많은 수의 메트릭을 매우 신속하게 수집하고보고 할 수 있습니다.





Atlas는 운영 정보를 캡처합니다. 비즈니스 인텔리전스는 추세 분석을 위해 수집 된 데이터이지만 운영 인텔리전스는 시스템 내에서 현재 일어나고있는 상황을 보여줍니다.





봄 클라우드가 제공하는 `spring-cloud-starter-atlas`당신이 필요로하는 모든 종속성을 갖는다. 그런 다음 귀하의 봄 부팅 응용 프로그램을 주석 `@EnableAtlas`과와 실행 아틀라스 서버의 위치를 제공하는 `netflix.atlas.uri`속성입니다.





#### 글로벌 태그



Spring Cloud를 사용하면 Atlas 백엔드로 전송되는 모든 메트릭에 태그를 추가 할 수 있습니다. 글로벌 태그를 사용하여 애플리케이션 이름, 환경, 지역 등으로 측정 항목을 분리 할 수 ​​있습니다.





구현 각 콩 `AtlasTagProvider`글로벌 태그 목록에 기여할 것입니다 :







    @Bean
    AtlasTagProvider atlasCommonTags(
        @Value("${spring.application.name}") String appName) {
      return () -> Collections.singletonMap("app", appName);
    }









#### Atlas 사용



인 - 메모리 독립형 Atlas 인스턴스를 부트 스트랩하려면 다음을 수행하십시오.







    $ curl -LO https://github.com/Netflix/atlas/releases/download/v1.4.2/atlas-1.4.2-standalone.jar
    $ java -jar atlas-1.4.2-standalone.jar













<td class="icon">

팁



<td class="content">r3.2xlarge (61GB RAM)에서 실행되는 Atlas 독립형 노드는 주어진 6 시간 동안 분당 약 2 백만 개의 메트릭을 처리 할 수 ​​있습니다.











일단 실행하고 몇 가지 메트릭을 수집했으면 Atlas 서버에 태그를 나열하여 설정이 올바른지 확인하십시오.







    $ curl http://ATLAS/api/v1/tags













<td class="icon">

팁



<td class="content">서비스에 대해 여러 요청을 실행 한 후 브라우저에 다음 URL을 붙여 넣어 요청의 대기 시간에 대한 몇 가지 기본적인 정보를 수집 할 수 있습니다. `[http://ATLAS/api/v1/graph?q=name,rest,:eq,:avg](http://atlas/api/v1/graph?q=name,rest,:eq,:avg)`











아틀라스 위키는 포함 [샘플 쿼리의 편집](https://github.com/Netflix/atlas/wiki/Single-Line) 다양한 시나리오를.





밖으로 확인하십시오 [경고 철학](https://github.com/Netflix/atlas/wiki/Alerting-Philosophy) 사용과 문서를 [이중 지수 평활를](https://github.com/Netflix/atlas/wiki/DES) 동적 경고 임계 값을 생성 할 수 있습니다.











# 스프링 클라우드 버스







Spring Cloud Bus는 분산 시스템의 노드를 간단한 메시지 브로커와 링크합니다. 그런 다음 상태 변경 (예 : 구성 변경) 또는 기타 관리 지침을 브로드 캐스트하는 데 사용할 수 있습니다. 핵심 아이디어는 버스가 확장 된 스프링 부트 애플리케이션을위한 분산 액츄에이터와 비슷하지만 앱 간의 통신 채널로도 사용될 수 있다는 것입니다. 유일한 구현은 현재 AMQP 브로커를 전송으로 사용하지만 동일한 기본 기능 집합 (그리고 전송에 따라 좀 더 많음)은 다른 전송을위한 로드맵에 있습니다.





[https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc](https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc)









## 빠른 시작





스프링 클라우드 버스는 클래스 패스에서 자체를 감지하면 스프링 부트 자동 구성을 추가하여 작동합니다. 당신이 버스를 활성화 할 필요가 추가하는 것입니다 `spring-cloud-starter-bus-amqp`귀하의 의존성 관리와 Spring Cloud은 나머지 처리합니다. 확인 RabbitMQ를 사용할 수 있는지 확인하고 제공하도록 구성된 `ConnectionFactory`: 당신은 아무것도 할 필요가 없습니다 로컬 호스트에서 실행하지만, 브로커 자격 증명을 정의하는 봄 클라우드 커넥터, 또는 봄 부팅 규칙을 사용하여 원격으로 실행하는 경우 예를 들어,





application.yml



<pre>봄:
  rabbitmq :
    호스트 : mybroker.com
    포트 : 5672
    사용자 이름 : 사용자
    비밀 번호 : 비밀</pre>







버스는 현재 모든 노드 수신 대기 또는 특정 서비스 (유레카에 정의 된대로)를위한 모든 노드로의 메시지 전송을 지원합니다. 미래에는 선택기 기준이 추가 될 것입니다 (예 : 데이터 센터 Y의 서비스 X 노드 등 ...). 는 HTTP 엔드 포인트는 아래에 `/bus/*`액츄에이터 네임 스페이스. 현재 두 가지가 구현되어 있습니다. 첫 번째는 `/bus/env`, 각 노드 봄 환경을 업데이트 / 키 값 쌍을 전송합니다. 두 번째는, `/bus/refresh`그들은 모두 자신의에 ping을했던 것처럼, 각 응용 프로그램의 구성을 다시로드합니다 `/refresh`엔드 포인트.









## 인스턴스 주소 지정





대상은 다음과 같습니다 "9000? / 버스 / 갱신 대상 = 고객"는 HTTP 엔드 포인트는 "대상"매개 변수, 예를 들어 동의 `ApplicationContext`ID를. ID가 버스의 인스턴스에 의해 소유되면 메시지를 처리하고 다른 모든 인스턴스는 ID를 무시합니다. 봄 부트는 당신의 ID를 설정 `ContextIdApplicationContextInitializer`의 조합으로 `spring.application.name`, 활성 프로필과 `server.port`기본적으로.









## 서비스의 모든 인스턴스 주소 지정





"대상"매개 변수는 봄에 사용된다 `PathMatcher`(콜론과 경로 분리와 `:`인스턴스가 메시지를 처리 할 수 있는지를 확인하기 위해). 위의 예제를 사용하여 "/ 버스 / 갱신 대상 = 고객 : **"상관없이로 설정 한 프로필과 포트의 "고객"서비스의 모든 인스턴스를 대상으로합니다 `ApplicationContext`ID.









## 응용 프로그램 컨텍스트 ID는 고유해야합니다.





버스는 한 번 원본, 두 번 이벤트 처리를 제거하려고 `ApplicationEvent`한 번 대기열에서. 이렇게하려면 보내는 응용 프로그램 컨텍스트 ID가 현재 응용 프로그램 컨텍스트 ID를 다시 확인합니다. 서비스의 여러 인스턴스에 동일한 응용 프로그램 컨텍스트 ID가 있으면 이벤트가 처리되지 않습니다. 로컬 컴퓨터에서 실행되는 각 서비스는 다른 포트에 있으며 응용 프로그램 컨텍스트 ID의 일부가됩니다. Cloud Foundry는 차별화 지수를 제공합니다. 애플리케이션 컨텍스트 ID가 고유한지 확인하려면 설정 `spring.application.index`서비스의 각 인스턴스에 대해 고유 뭔가. 예를 들어, 격자, 설정 `spring.application.index=${INSTANCE_INDEX}`application.properties (또는 bootstrap.properties configserver를 사용하는 경우)에.









## 메시지 브로커 사용자 정의





봄 클라우드 버스 사용 [봄 클라우드 스트림](https://cloud.spring.io/spring-cloud-stream) 만 클래스 패스에있는 당신의 선택의 바인더 구현을 포함 할 필요가 흐르도록 메시지를 얻을 수 있도록 메시지를 방송 할 수 있습니다. 편리한 스타터 구체적으로 AMQP, 카프카와 레디 스와 버스가있다 ( `spring-cloud-starter-bus-[amqp,kafka,redis]`). 인스턴스에 대한 AMQP 브로커 주소를 변경할 수 있도록 일반적으로 봄 클라우드 스트림, 미들웨어를 구성하는 봄 부팅 자동 규칙에 의존 `spring.rabbitmq.*` 구성 등록. 봄 클라우드 버스의 기본 구성 등록 정보의 소수가 있습니다 `spring.cloud.bus.*` (예 : `spring.cloud.bus.destination`상기 externall 미들웨어 사용하는 항목의 이름입니다). 일반적으로 기본값으로 충분합니다.





메시지 브로커 설정을 사용자 정의하는 방법에 대해 자세히 알고 싶으면 Spring Cloud Stream 문서를 참조하십시오.









## 추적 버스 이벤트





버스 이벤트 (의 서브 클래스 `RemoteApplicationEvent`)를 설정하여 추적 할 수 있습니다 `spring.cloud.bus.trace.enabled=true`. 그런 다음 봄 부팅이 작업을 수행하는 경우 `TraceRepository`(존재하는 경우) 각 서비스 인스턴스에서 전송 된 각 이벤트와 모든 ACK들을 보여줍니다. (로부터 예 `/trace`엔드 포인트)







    {
      "timestamp": "2015-11-26T10:24:44.411+0000",
      "info": {
        "signal": "spring.cloud.bus.ack",
        "type": "RefreshRemoteApplicationEvent",
        "id": "c4d374b7-58ea-4928-a312-31984def293b",
        "origin": "stores:8081",
        "destination": "*:**"
      }
      },
      {
      "timestamp": "2015-11-26T10:24:41.864+0000",
      "info": {
        "signal": "spring.cloud.bus.sent",
        "type": "RefreshRemoteApplicationEvent",
        "id": "c4d374b7-58ea-4928-a312-31984def293b",
        "origin": "customers:9000",
        "destination": "*:**"
      }
      },
      {
      "timestamp": "2015-11-26T10:24:41.862+0000",
      "info": {
        "signal": "spring.cloud.bus.ack",
        "type": "RefreshRemoteApplicationEvent",
        "id": "c4d374b7-58ea-4928-a312-31984def293b",
        "origin": "customers:9000",
        "destination": "*:**"
      }
    }







이 추적은이 것을 보여준다 `RefreshRemoteApplicationEvent`에서 전송 된 `customers:9000`모든 서비스를 방송하고,이 수신 (애크) 한 `customers:9000`과 `stores:8081`.





상기 ACK 신호를 직접 처리하기 위해 당신은 추가 할 수 `@EventListener` 에 대한 `AckRemoteAppplicationEvent`및 `SentApplicationEvent`앱에 대한 유형을 (그리고 추적을 사용 가능). 아니면 활용할 수 `TraceRepository`거기에서 데이터를 마이닝.











<td class="icon">

노트



<td class="content">모든 버스 응용 프로그램은 acks를 추적 할 수 있지만 때때로 데이터에 대해 더 복잡한 쿼리를 수행 할 수있는 중앙 서비스에서이 작업을 수행하는 것이 유용합니다. 또는 특수화 된 추적 서비스로 전달하십시오.













# 스프링 부트 클라우드 CLI







봄 부팅 CLI가 제공하는 [봄 부트](http://projects.spring.io/spring-boot) 에 대한 명령 줄 기능을 [Spring Cloud](https://github.com/spring-cloud) . 당신은 봄 클라우드 구성 요소 응용 프로그램을 실행하는 데 (예를 그루비 스크립트를 작성할 수 있습니다 `@EnableEurekaServer`). 또한 암호화 및 복호화와 같은 작업을 수행하여 비밀 구성 값으로 Spring Cloud Config 클라이언트를 지원할 수 있습니다.





[https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc](https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc)









## 설치





확인 설치해야합니다, 당신은 [봄 부트 CLI](https://github.com/spring-projects/spring-boot) (1.2.0 이상) :







<pre>$ 봄 버전
Spring CLI v1.2.3.RELEASE</pre>







예 : GVM 사용자







    $ gvm install springboot 1.3.0.M5
    $ gvm use springboot 1.3.0.M5







Spring Cloud 플러그인을 설치한다.







    $ mvn install
    $ spring install org.springframework.cloud:spring-cloud-cli:1.1.0.BUILD-SNAPSHOT













<td class="icon">

중대한



<td class="content">**전제 조건 :** 당신이 당신의 JVM에 설치된 전체 강도 JCE를 필요로하는 암호화 및 복호화 기능 (기본값이 아닙니다)를 사용합니다. Oracle에서 "Java Cryptography Extension (JCE) 무제한 강도 관할 정책 파일"을 다운로드하고 설치 지침을 따르십시오 (기본적으로 JRE lib / security 디렉토리에있는 2 개의 정책 파일을 다운로드 한 정책 파일로 대체하십시오).















## Groovy 스크립트 작성 및 응용 프로그램 실행





봄 클라우드 CLI는 같은과 Spring Cloud 선언적 기능의 대부분에 대한 지원이 `@Enable*`주석의 클래스를. 예를 들어, 다음은 유레카 서버입니다.





app.groovy



    @EnableEurekaServer
    class Eureka {}







이 명령 줄에서 다음과 같이 실행할 수 있습니다.







<pre>$ spring run app.groovy</pre>







추가 종속성을 포함하려면, 종종 그냥 예를 들어, 해당 기능이 활성화 주석을 추가하기에 충분 `@EnableConfigServer`, `@EnableOAuth2Sso`또는 `@EnableEurekaClient`. 수동으로 사용자가 사용할 수 있습니다 종속성 포함하려면 `@Grab`AMQP에서 수신하는 클라이언트 응용 프로그램을 설정하는 예를 들어 특별한 "봄 부팅"짧은 스타일 이슈 좌표로, 즉 단지 이슈 ID (그룹 또는 버전 정보에 대한 필요성)과를, Spring CLoud Bus의 관리 이벤트 용 :





app.groovy



    @Grab('spring-cloud-starter-bus-amqp')
    @RestController
    class Service {
      @RequestMapping('/')
      def home() { [message: 'Hello'] }
    }











## 암호화 및 암호 해독





Spring Cloud CLI에는 "encrypt"와 "decrypt"명령이있다. 둘 다 필수적인 "--key"로 지정된 키를 사용하여 동일한 형식의 인수를 허용합니다.







<pre>$ spring encrypt mysecret --key foo
682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
$ spring decrypt --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
나의 비밀</pre>







파일에서 키를 사용하려면 (예 : encyption을위한 RSA 공개 키) 키 값 앞에 "@"를 붙이고 파일 경로를 제공하십시오.







<pre>$ spring encrypt mysecret --key @ $ {HOME} /. ssh / id_rsa.pub
AQAjPgt3eFZQXwt8tsHAVv / QHiY5sI2dRcR + ...</pre>









# 스프링 클라우드 보안







Spring Cloud Security는 최소한의 소란으로 보안 애플리케이션 및 서비스를 구축하기위한 일련의 프리미티브를 제공합니다. 외부 적으로 (또는 중앙 집중적으로) 구성 할 수있는 선언적 모델은 일반적으로 중앙 압흔 관리 서비스와 함께 공동 작동하는 원격 구성 요소의 대형 시스템 구현에 적합합니다. 또한 Cloud Foundry와 같은 서비스 플랫폼에서 사용하기가 매우 쉽습니다. Spring Boot and Spring Security OAuth2를 기반으로 싱글 사인온 (single sign on), 토큰 릴레이 및 토큰 교환과 같은 공통 패턴을 구현하는 시스템을 신속하게 생성 할 수 있습니다.





[https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc](https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc)









## 빠른 시작





### OAuth2 싱글 사인온



다음은 HTTP 기본 인증과 단일 사용자 계정을 가진 Spring Cloud "Hello World"앱입니다.





app.groovy



    @Grab('spring-boot-starter-security')
    @Controller
    class Application {

      @RequestMapping('/')
      String home() {
        'Hello World'
      }

    }







당신은 그것을 실행할 수 있습니다 `spring run app.groovy`(사용자 이름이 "사용자"입니다) 및 비밀번호에 대한 로그를보십시오. 지금까지는 Spring Boot app의 기본값입니다.





다음은 OAuth2 SSO가 적용된 Spring Cloud 앱입니다.





app.groovy



    @Controller
    @EnableOAuth2Sso
    class Application {

      @RequestMapping('/')
      String home() {
        'Hello World'
      }

    }







차이점이 있습니까? 이 앱은 실제로 OAuth2 신상을 알지 못하기 때문에 이전 앱과 정확히 동일하게 작동합니다.





github에서 앱을 쉽게 등록 할 수 있으므로 자신의 도메인에 프로덕션 응용 프로그램이 필요한 경우 시도하십시오. localhost : 8080에서 테스트 할 수 있다면 응용 프로그램 구성에서 다음 등록 정보를 설정하십시오.





application.yml



    spring:
      oauth2:
        client:
          clientId: bd1c0a783ccdd1c9b9e4
          clientSecret: 1a9030fbca47a5b2c28e92f19050bb77824b5ad1
          accessTokenUri: https://github.com/login/oauth/access_token
          userAuthorizationUri: https://github.com/login/oauth/authorize
          clientAuthenticationScheme: form
        resource:
          userInfoUri: https://api.github.com/user
          preferTokenInfo: false







위의 앱을 실행하면 인증을 위해 github로 리디렉션됩니다. github에 이미 로그인 한 경우 인증을받지 못합니다. 이 자격 증명은 앱이 포트 8080에서 실행되는 경우에만 작동합니다.





클라이언트는 액세스 사용자가 설정할 수있는 토큰을 획득 할 때 요청하는 범위를 제한 `spring.oauth2.client.scope`(또는 쉼표로 구분 YAML의 배열). 기본적으로 범위는 비어 있으며 권한 서버가 보유해야하는 클라이언트 등록의 설정에 따라 기본값을 결정해야합니다.











<td class="icon">

노트



<td class="content">위의 예는 모두 Groovy 스크립트입니다. 자바 (또는 그루비)에서 동일한 코드를 작성하려는 경우에는 (예를 들어 볼 수있는 클래스 패스에 봄 보안 OAuth2를 추가 할 필요가 [여기에 샘플](https://github.com/spring-cloud-samples/sso) ).













### OAuth2 보호 된 리소스



OAuth2 토큰을 사용하여 API 리소스를 보호하고 싶습니까? 다음은 위의 클라이언트와 쌍을 이루는 간단한 예제입니다.





app.groovy



    @Grab('spring-cloud-starter-security')
    @RestController
    @EnableResourceServer
    class Application {

      @RequestMapping('/')
      def home() {
        [message: 'Hello World']
      }

    }







및





application.yml



    spring:
      oauth2:
        resource:
          userInfoUri: https://api.github.com/user
          preferTokenInfo: false













## 상세 정보





### 단일 사인온











노트



OAuth2 SSO 및 리소스 서버 기능은 모두 Spring Boot 버전 1.3으로 이전되었습니다. 당신은에서 문서를 찾을 수 있습니다 [봄 부팅 사용자 설명서를](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/) .













### 토큰 중계



토큰 릴레이는 OAuth2 고객이 클라이언트 역할을하고 들어오는 토큰을 나가는 리소스 요청으로 전달하는 곳입니다. 소비자는 순수 클라이언트 (SSO 응용 프로그램과 같은) 또는 자원 서버가 될 수 있습니다.





#### 클라이언트 토큰 릴레이



앱이있는 경우 [Spring Cloud Zuul](http://cloud.spring.io/spring-cloud.html#netflix-zuul-reverse-proxy) (사용 포함 된 역방향 프록시를 `@EnableZuulProxy`) 다음은 프록시 된 서비스 하류 OAuth2를 액세스 토큰을 전달하도록 요청할 수 있습니다. 따라서 위의 SSO 앱은 다음과 같이 간단하게 향상시킬 수 있습니다.





app.groovy



    @Controller
    @EnableOAuth2Sso
    @EnableZuulProxy
    class Application {

    }







그것은 (추가에서 사용자를 loggin에와 토큰을 잡는까지)에 토큰 하류 인증을 통과 할 것이다 `/proxy/*` 서비스를 제공합니다. 이러한 서비스를 구현하는 경우 `@EnableOAuth2Resource`그들은 올바른 헤더에 유효한 토큰을 얻을 것이다.





어떻게 작동합니까? `@EnableOAuth2Sso`주석에 끌어 `spring-cloud-starter-security`(당신은 기존의 응용 프로그램에서 수동으로 할 수있는), 그리고 차례로 그는 몇 가지 자동 트리거 `ZuulFilter`Zuul 클래스 경로 (경유에 있기 때문에 그 자체가 활성화되고 `@EnableZuulProxy`). {github} /tree/master/src/main/java/org/springframework/cloud/security/oauth2/proxy/OAuth2TokenRelayFilter.java [필터]는 현재 인증 된 사용자로부터 액세스 토큰을 추출하여 요청에 넣습니다 헤더를 포함한다.







#### 리소스 서버 토큰 릴레이



앱이있는 경우 `@EnableOAuth2Resource`또한 클라이언트 (즉, 그것은을 가지고있다 `spring.oauth2.client.clientId`그것을 사용하지 않는 경우에도), 다음 `OAuth2RestOperations`그 제공된다 `@Autowired` (이로 선언 Spring Cloud에 의해 사용자 `@Primary`도) 앞으로 토큰을 것입니다. 당신은 토큰을 전달하지 않으려는 (당신이 아니라 당신에게 토큰을 보낸 클라이언트보다, 자신의 역할을 할 수 있으므로 즉, 올바른 선택입니다) 당신은 당신의 자신을 만들 필요가있는 경우 `OAuth2RestOperations`대신 기본 autowiring에 하나. 다음은 autowired 나머지 템플릿 ( "foo.com"은 주변 서버와 동일한 토큰을 허용하는 리소스 서버)의 사용을 보여주는 기본 예제입니다.





MyController.java



    @Autowired
    private OAuth2RestOperations restTemplate;

    @RequestMapping("/relay")
    public String relay() {
        ResponseEntity<String> response =
          restTemplate.getForEntity("https://foo.com/bar", String.class);
        return "Success! (" + response.getBody() + ")";
    }















## Zuul 프록시의 인증 다운 스트림 구성





당신은 하류의 권한 부여 동작을 제어 할 수 있습니다 `@EnableZuulProxy`스루 `proxy.auth.*`설정을. 예:





application.yml



    proxy:
      auth:
        routes:
          customers: oauth2
          stores: passthru
          recommendations: none







이 예에서 '고객'서비스는 OAuth2 토큰 릴레이를 가져 오며, '상점'서비스는 통과 (인증 헤더가 다운 스트림으로 전달됨)되고 '추천'서비스는 인증 헤더가 제거됩니다. 기본 동작은 사용 가능한 토큰이있는 경우 토큰 릴레이를 수행하고 그렇지 않으면 패스 스루를 수행하는 것입니다.





자세한 내용은 {github} / tree / master / src / main / java / org / springframework / cloud / security / oauth2 / proxy / ProxyAuthenticationProperties [ProxyAuthenticationProperties]를 참조하십시오.










최종 업데이트 : 2016-01-26 10:56:04 UTC




![Google 번역](./spring-cloud-doc-images/translate_24dp.png)







# 원본 텍스트





Spring Boot has an opinionated view of how to build an application with Spring: for instance it has conventional locations for common configuration file, and endpoints for common management and monitoring tasks.





* * *






