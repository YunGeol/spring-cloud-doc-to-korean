# Spring Cloud


목차

*   [풍모](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_features)
*   [클라우드 네이티브 애플리케이션](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_cloud_native_applications)
    *   [Spring Cloud Context : 애플리케이션 컨텍스트 서비스](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_context_application_context_services)
        *   [부트 스트랩 응용 프로그램 컨텍스트](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_the_bootstrap_application_context)
        *   [응용 프로그램 컨텍스트 계층 구조](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_application_context_hierarchies)
        *   [부트 스트랩 속성 위치 변경](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#customizing-bootstrap-properties)
        *   [원격 등록 정보 값 재 지정](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#overriding-bootstrap-properties)
        *   [부트 스트랩 구성 사용자 정의](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_customizing_the_bootstrap_configuration)
        *   [부트 스트랩 속성 소스 사용자 정의](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#customizing-bootstrap-property-sources)
        *   [환경 변화](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_environment_changes)
        *   [새로 고침 범위](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_refresh_scope)
        *   [암호화 및 암호 해독](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_encryption_and_decryption)
        *   [종점](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_endpoints)
    *   [Spring Cloud Commons : 공통 추상화](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_commons_common_abstractions)
        *   [@EnableDiscoveryClient](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#__enablediscoveryclient)
        *   [ServiceRegistry](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_serviceregistry)
        *   [로드 밸런서 클라이언트로서의 Spring RestTemplate](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_resttemplate_as_a_load_balancer_client)
        *   [여러 RestTemplate 객체](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_multiple_resttemplate_objects)
        *   [네트워크 인터페이스 무시](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#ignore-network-interfaces)
*   [스프링 클라우드 구성](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_config)
    *   [빠른 시작](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_quick_start)
        *   [클라이언트 측 사용](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_client_side_usage)
    *   [스프링 클라우드 구성 서버](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_config_server)
        *   [환경 저장소](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_environment_repository)
        *   [건강 지표](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_health_indicator)
        *   [보안](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_security)
        *   [암호화 및 암호 해독](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_encryption_and_decryption_2)
        *   [키 관리](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_key_management)
        *   [테스트 용 키 저장소 만들기](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_creating_a_key_store_for_testing)
        *   [여러 키 및 키 회전 사용](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_multiple_keys_and_key_rotation)
        *   [암호화 된 속성 제공](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_serving_encrypted_properties)
    *   [대체 형식 검색](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_serving_alternative_formats)
    *   [Serving Plain Text](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_serving_plain_text)
    *   [Embedding the Config Server](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_embedding_the_config_server)
    *   [Push Notifications and Spring Cloud Bus](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_push_notifications_and_spring_cloud_bus)
    *   [Spring Cloud Config Client](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_config_client)
        *   [Config First Bootstrap](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#config-first-bootstrap)
        *   [Discovery First Bootstrap](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#discovery-first-bootstrap)
        *   [Config Client Fail Fast](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#config-client-fail-fast)
        *   [Config Client Retry](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#config-client-retry)
        *   [Locating Remote Configuration Resources](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_locating_remote_configuration_resources)
        *   [Security](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_security_2)
*   [Spring Cloud Netflix](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_netflix)
    *   [Service Discovery: Eureka Clients](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_service_discovery_eureka_clients)
        *   [Registering with Eureka](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_registering_with_eureka)
        *   [Authenticating with the Eureka Server](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_authenticating_with_the_eureka_server)
        *   [Status Page and Health Indicator](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_status_page_and_health_indicator)
        *   [Registering a Secure Application](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_registering_a_secure_application)
        *   [Eureka’s Health Checks](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_eureka_s_health_checks)
        *   [Eureka Metadata for Instances and Clients](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_eureka_metadata_for_instances_and_clients)
        *   [Using the EurekaClient](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_the_eurekaclient)
        *   [Alternatives to the native Netflix EurekaClient](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_alternatives_to_the_native_netflix_eurekaclient)
        *   [Why is it so Slow to Register a Service?](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_why_is_it_so_slow_to_register_a_service)
    *   [Service Discovery: Eureka Server](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-eureka-server)
        *   [High Availability, Zones and Regions](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_high_availability_zones_and_regions)
        *   [Standalone Mode](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_standalone_mode)
        *   [Peer Awareness](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_peer_awareness)
        *   [Prefer IP Address](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_prefer_ip_address)
    *   [Circuit Breaker: Hystrix Clients](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_circuit_breaker_hystrix_clients)
        *   [Propagating the Security Context or using Spring Scopes](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_propagating_the_security_context_or_using_spring_scopes)
        *   [Health Indicator](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_health_indicator_2)
        *   [Hystrix Metrics Stream](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_hystrix_metrics_stream)
    *   [Circuit Breaker: Hystrix Dashboard](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_circuit_breaker_hystrix_dashboard)
        *   [Turbine](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_turbine)
        *   [Turbine Stream](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_turbine_stream)
    *   [Client Side Load Balancer: Ribbon](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon)
        *   [Customizing the Ribbon Client](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_customizing_the_ribbon_client)
        *   [Using Ribbon with Eureka](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_ribbon_with_eureka)
        *   [Example: How to Use Ribbon Without Eureka](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon-without-eureka)
        *   [Example: Disable Eureka use in Ribbon](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_example_disable_eureka_use_in_ribbon)
        *   [Using the Ribbon API Directly](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_the_ribbon_api_directly)
    *   [Declarative REST Client: Feign](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign)
        *   [Overriding Feign Defaults](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-overriding-defaults)
        *   [Feign Hystrix Support](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-hystrix)
        *   [Feign Hystrix Fallbacks](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-hystrix-fallback)
        *   [Feign Inheritance Support](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-inheritance)
        *   [Feign request/response compression](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_feign_request_response_compression)
        *   [Feign logging](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_feign_logging)
    *   [External Configuration: Archaius](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_external_configuration_archaius)
    *   [Router and Filter: Zuul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_router_and_filter_zuul)
        *   [Embedded Zuul Reverse Proxy](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#netflix-zuul-reverse-proxy)
        *   [Cookies and Sensitive Headers](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_cookies_and_sensitive_headers)
        *   [The Routes Endpoint](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_the_routes_endpoint)
        *   [Strangulation Patterns and Local Forwards](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_strangulation_patterns_and_local_forwards)
        *   [Uploading Files through Zuul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_uploading_files_through_zuul)
        *   [Plain Embedded Zuul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_plain_embedded_zuul)
        *   [Disable Zuul Filters](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_disable_zuul_filters)
        *   [Polyglot support with Sidecar](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_polyglot_support_with_sidecar)
    *   [RxJava with Spring MVC](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#netflix-rxjava-springmvc)
    *   [Metrics: Spectator, Servo, and Atlas](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#netflix-metrics)
        *   [Dimensional vs. Hierarchical Metrics](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_dimensional_vs_hierarchical_metrics)
        *   [Default Metrics Collection](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_default_metrics_collection)
        *   [Metrics Collection: Spectator](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#netflix-metrics-spectator)
        *   [Metrics Collection: Servo](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#netflix-metrics-servo)
        *   [Metrics Backend: Atlas](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#netflix-metrics-atlas)
*   [Spring Cloud Stream](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_stream)
    *   [Introducing Spring Cloud Stream](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_introducing_spring_cloud_stream)
    *   [Main Concepts](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_main_concepts)
        *   [Application Model](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_application_model)
        *   [The Binder Abstraction](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_the_binder_abstraction)
        *   [Persistent Publish-Subscribe Support](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_persistent_publish_subscribe_support)
        *   [Consumer Groups](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#consumer-groups)
        *   [Partitioning Support](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#partitioning)
    *   [Programming Model](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_programming_model)
        *   [Declaring and Binding Channels](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_declaring_and_binding_channels)
    *   [Binders](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_binders)
        *   [Producers and Consumers](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_producers_and_consumers)
        *   [Binder SPI](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_binder_spi)
        *   [Binder Detection](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_binder_detection)
        *   [Multiple Binders on the Classpath](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#multiple-binders)
        *   [Connecting to Multiple Systems](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#multiple-systems)
        *   [Binder configuration properties](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_binder_configuration_properties)
        *   [Implementation strategies](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_implementation_strategies)
    *   [Configuration Options](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_configuration_options)
        *   [Spring Cloud Stream Properties](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_stream_properties)
        *   [Binding Properties](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#binding-properties)
    *   [Binder-Specific Configuration](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#binder-specific-configuration)
        *   [Rabbit-Specific Settings](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_rabbit_specific_settings)
        *   [Kafka-Specific Settings](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_kafka_specific_settings)
    *   [Content Type and Transformation](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#contenttypemanagement)
        *   [MIME types](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#mime-types)
        *   [MIME types and Java types](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#mime-types-and-java-types)
        *   [`@StreamListener` and Message Conversion](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#__code_streamlistener_code_and_message_conversion)
    *   [Inter-Application Communication](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_inter_application_communication)
        *   [Connecting Multiple Application Instances](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_connecting_multiple_application_instances)
        *   [Instance Index and Instance Count](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_instance_index_and_instance_count)
        *   [Partitioning](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_partitioning)
    *   [Testing](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_testing)
    *   [Health Indicator](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_health_indicator_3)
    *   [Samples](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_samples)
    *   [Getting Started](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_getting_started)
*   [Spring Cloud Bus](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_bus)
    *   [Quick Start](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_quick_start_2)
    *   [Addressing an Instance](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_addressing_an_instance)
    *   [Addressing all instances of a service](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_addressing_all_instances_of_a_service)
    *   [Application Context ID must be unique](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_application_context_id_must_be_unique)
    *   [Customizing the Message Broker](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_customizing_the_message_broker)
    *   [Tracing Bus Events](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_tracing_bus_events)
    *   [Broadcasting Your Own Events](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_broadcasting_your_own_events)
*   [Spring Cloud Sleuth](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_sleuth)
    *   [Terminology](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_terminology)
    *   [Purpose](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_purpose)
    *   [Adding to the project](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_adding_to_the_project)
    *   [Additional resources](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_additional_resources)
    *   [Features](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_features_2)
    *   [Sampling](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_sampling)
    *   [Instrumentation](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_instrumentation)
    *   [Span lifecycle](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_span_lifecycle)
        *   [Creating and closing spans](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#creating-and-closing-spans)
        *   [Continuing spans](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#continuing-spans)
        *   [Creating spans with an explicit parent](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#creating-spans-with-explicit-parent)
    *   [Naming spans](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_naming_spans)
        *   [@SpanName annotation](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#__spanname_annotation)
        *   [toString() method](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_tostring_method)
    *   [Customizations](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_customizations)
        *   [Spring Integration](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_integration)
        *   [HTTP](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_http)
        *   [Example](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_example)
        *   [Custom SA tag in Zipkin](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_custom_sa_tag_in_zipkin)
        *   [Custom service name](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_custom_service_name)
    *   [Span Data as Messages](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_span_data_as_messages)
        *   [Zipkin Consumer](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_zipkin_consumer)
        *   [Custom Consumer](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_custom_consumer)
    *   [Metrics](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_metrics)
    *   [Integrations](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_integrations)
        *   [Runnable and Callable](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_runnable_and_callable)
        *   [Hystrix](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_hystrix)
        *   [RxJava](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_rxjava)
        *   [HTTP integration](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_http_integration)
        *   [HTTP client integration](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_http_client_integration)
        *   [Feign](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_feign)
        *   [Asynchronous communication](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_asynchronous_communication)
        *   [Messaging](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_messaging)
        *   [Zuul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_zuul)
    *   [Running examples](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_running_examples)
*   [Spring Cloud Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_consul)
    *   [Install Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-install)
    *   [Consul Agent](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-agent)
    *   [Service Discovery with Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-discovery)
        *   [Registering with Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_registering_with_consul)
        *   [HTTP Health Check](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_http_health_check)
        *   [Using the DiscoveryClient](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_the_discoveryclient)
    *   [Distributed Configuration with Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-config)
        *   [How to activate](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_how_to_activate)
        *   [Customizing](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_customizing)
    *   [YAML or Properties with Config](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-config-format)
    *   [git2consul with Config](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-config-git2consul)
    *   [Fail Fast](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-failfast)
    *   [Consul Retry](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-retry)
    *   [Spring Cloud Bus with Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-bus)
    *   [Circuit Breaker with Hystrix](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-hystrix)
    *   [Hystrix metrics aggregation with Turbine and Consul](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-turbine)
*   [Spring Cloud Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_zookeeper)
    *   [Install Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-zookeeper-install)
    *   [Service Discovery with Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-zookeeper-discovery)
        *   [How to activate](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_how_to_activate_2)
        *   [Registering with Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_registering_with_zookeeper)
        *   [Using the DiscoveryClient](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_the_discoveryclient_2)
    *   [Zookeeper Dependencies](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-zookeeper-dependencies)
        *   [Using the Zookeeper Dependencies](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_using_the_zookeeper_dependencies)
        *   [How to activate Zookeeper Dependencies](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_how_to_activate_zookeeper_dependencies)
        *   [Setting up Zookeeper Dependencies](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_setting_up_zookeeper_dependencies)
        *   [Configuring Spring Cloud Zookeeper Dependencies](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_configuring_spring_cloud_zookeeper_dependencies)
    *   [Spring Cloud Zookeeper Dependency Watcher](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-zookeeper-dependency-watcher)
        *   [How to activate](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_how_to_activate_3)
        *   [Registering a listener](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_registering_a_listener)
        *   [Presence Checker](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_presence_checker)
    *   [Distributed Configuration with Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-zookeeper-config)
        *   [How to activate](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_how_to_activate_4)
        *   [Customizing](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_customizing_2)
*   [Spring Boot Cloud CLI](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_boot_cloud_cli)
    *   [Installation](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_installation)
    *   [Running Spring Cloud Services in Development](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_running_spring_cloud_services_in_development)
        *   [Adding Additional Applications](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_adding_additional_applications)
    *   [Writing Groovy Scripts and Running Applications](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_writing_groovy_scripts_and_running_applications)
    *   [Encryption and Decryption](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_encryption_and_decryption_3)
*   [Spring Cloud Security](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_security)
    *   [Quickstart](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_quickstart)
        *   [OAuth2 Single Sign On](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_oauth2_single_sign_on)
        *   [OAuth2 Protected Resource](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_oauth2_protected_resource)
    *   [More Detail](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_more_detail)
        *   [Single Sign On](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_single_sign_on)
        *   [Token Relay](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_token_relay)
    *   [Configuring Authentication Downstream of a Zuul Proxy](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_configuring_authentication_downstream_of_a_zuul_proxy)
*   [Spring Cloud for Cloud Foundry](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_for_cloud_foundry)
    *   [Discovery](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_discovery)
    *   [Single Sign On](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_single_sign_on_2)
*   [Spring Cloud Cluster](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_spring_cloud_cluster)
    *   [Leader Election](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_leader_election)
        *   [Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-cluster-leaderelection-zookeeper)
        *   [Hazelcast](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-cluster-leaderelection-hazelcast)
        *   [Etcd](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-cluster-leaderelection-etcd)
*   [Appendix: Compendium of Configuration Properties](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_appendix_compendium_of_configuration_properties)



Spring Cloud는 개발자가 분산 시스템 (예 : 구성 관리, 서비스 발견, 회로 차단기, 지능형 라우팅, 마이크로 프록시, 제어 버스, 일회성 토큰, 글로벌 잠금, 리더십 선거, 분산 등)의 공통 패턴을 신속하게 구축 할 수있는 도구를 제공합니다. 세션, 클러스터 상태). 분산 시스템을 조정하면 보일러 플레이트 패턴이 생기고 Spring Cloud 개발자는 이러한 패턴을 구현하는 서비스와 애플리케이션을 신속하게 구현할 수 있습니다. 개발자의 자체 랩톱, 베어 메탈 (bare metal) 데이터 센터 및 Cloud Foundry와 같은 관리 플랫폼을 포함한 모든 분산 환경에서 잘 작동합니다.


버전 : Brixton.BUILD-SNAPSHOT


## Features


Spring Cloud는 전형적인 유스 케이스에 대해 좋은 아웃 오브 바운드 경험을 제공하고 다른 사람들을 포괄하는 확장 성 메커니즘에 중점을 둡니다.


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


[Cloud Native](https://pivotal.io/platform-as-a-service/migrating-to-cloud-native-application-architectures-ebook) 는 지속적인 개발 및 가치 중심 개발 분야에서 모범 사례를 쉽게 채택하도록 권장하는 애플리케이션 개발 스타일입니다. 이와 관련된 분야는 개발 관행이 전달 및 운영 목표 (예 : 선언적 프로그래밍 및 관리 및 모니터링 사용)와 연계 된 [12 개 요소의 Apps](http://12factor.net/) 구축에 있습니다. 스프링 클라우드는 여러 가지 방식으로 이러한 개발 스타일을 용이하게하며 출발점은 분산 시스템의 모든 구성 요소가 필요할 때 쉽게 액세스 할 수 있거나 필요로하는 기능 집합입니다.



이러한 기능 중 많은 부분 은 Spring Cloud에서 제공 하는 [Spring Boot](http://projects.spring.io/spring-boot) 에서 다룹니다 . Spring Cloud는 두 가지 라이브러리 인 Spring Cloud Context와 Spring Cloud Commons를 제공합니다. Spring Cloud Context는 `ApplicationContext`Spring Cloud 애플리케이션 (부트 스트랩 컨텍스트, 암호화, 화면 갱신 범위 및 환경 엔드 포인트)에 유틸리티와 특수 서비스를 제공한다 . Spring Cloud Commons는 다양한 Spring Cloud 구현 (예 : Spring Cloud Netflix 대 Spring Cloud Consul)에서 사용되는 추상화 및 공통 클래스 세트입니다.


"잘못된 키 크기"로 인해 예외가 발생하고 Sun의 JDK를 사용하는 경우 JCE (Java Cryptography Extension) 무제한 강도 관할 정책 파일을 설치해야합니다. 자세한 내용은 다음 링크를 참조하십시오.


*   [Java 6 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-6-download-429243.html)

*   [Java 7 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html)

*   [Java 8 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html)




JDK / jre / lib / security 폴더 (사용중인 JRE / JDK x64 / x86 버전)로 파일을 추출하십시오.













노트

Spring Cloud는 비 제한적 Apache 2.0 라이센스에 따라 출시되었습니다. 문서의이 섹션에 기여하고 싶거나 오류가 발견되면 [github](https://github.com/spring-cloud/spring-cloud-commons/tree/master/docs/src/main/asciidoc) 에서 프로젝트의 소스 코드와 이슈 트래커를 찾으십시오 .|















## Spring Cloud Context : 애플리케이션 컨텍스트 서비스





Spring Boot는 일반적인 구성 파일을위한 전통적인 위치와 일반적인 관리 및 모니터링 작업을위한 끝점을 가지고있는 Spring을 사용하여 응용 프로그램을 빌드하는 방법에 대한 의견이 많습니다. Spring Cloud는이를 기반으로 시스템의 모든 구성 요소가 사용하거나 필요로하는 기능을 추가합니다.





### 부트 스트랩 응용 프로그램 컨텍스트



Spring Cloud 애플리케이션은 메인 애플리케이션의 상위 컨텍스트 인 "부트 스트랩"컨텍스트를 작성하여 작동합니다. 기본적으로 외부 소스에서 구성 등록 정보를로드하고 로컬 외부 구성 파일의 등록 정보를 해독합니다. 이 두 컨텍스트 `Environment` 는 어떤 Spring 애플리케이션의 외부 속성 소스가 되는 것을 공유합니다 . 부트 스트랩 속성은 우선 순위가 높으므로 기본적으로 로컬 구성에 의해 재정의 될 수 없습니다.





부트 스트랩 컨텍스트는 주 응용 프로그램 컨텍스트가 아닌 외부 구성을 찾는 데 다른 규칙을 사용하므로 `application.yml`(또는 `.properties`) 대신 `bootstrap.yml`부트 스트랩 및 주 컨텍스트에 대한 외부 구성을 잘 분리하여 유지하십시오. 예:





bootstrap.yml


```
spring:
    application:
        name : foo
    cloud:
        config :
            uri : $ {SPRING_CONFIG_URI : http : // localhost : 8888}
```





응용 프로그램에 서버의 응용 프로그램 별 구성이 필요한 경우에는 `spring.application.name`in `bootstrap.yml`또는 `application.yml`) 을 설정하는 것이 좋습니다 .





설정 `spring.cloud.bootstrap.enabled=false`(예 : 시스템 속성)을 통해 부트 스트랩 프로세스를 완전히 비활성화 할 수 있습니다 .







### 응용 프로그램 컨텍스트 계층 구조



`SpringApplication`또는 에서 응용 프로그램 컨텍스트를 빌드하면 부트 `SpringApplicationBuilder`스트랩 컨텍스트가 해당 컨텍스트의 부모로 추가됩니다. 하위 컨텍스트가 부모로부터 속성 소스와 프로파일을 상속받는 것은 Spring의 기능이므로 "기본"애플리케이션 컨텍스트에는 Spring Cloud Config없이 동일한 컨텍스트를 빌드하는 것과 비교하여 추가 속성 소스가 포함됩니다. 추가 속성 소스는 다음과 같습니다.





*   "부트 스트랩": 부트 스트랩 컨텍스트에서 발견 되는 옵션 `CompositePropertySource`이 높은 우선 순위로 `PropertySourceLocators`나타나며 속성이 비어 있습니다. 한 예로 Spring Cloud Config Server의 특성이있다. 이 속성 소스의 내용을 사용자 정의하는 방법에 대한 지침 은 [아래](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#customizing-bootstrap-property-sources) 를 참조 [하십시오](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#customizing-bootstrap-property-sources) .

*   "applicationConfig : [classpath : bootstrap.yml]"(스프링 프로파일이 활성화 된 경우 친구). 속성이있는 경우 `bootstrap.yml`해당 속성은 부트 스트랩 컨텍스트를 구성하는 데 사용되며 부모가 설정된 경우 하위 컨텍스트에 추가됩니다. 그들은 `application.yml`(또는 속성) 및 Spring 부트 응용 프로그램을 만드는 과정의 정상적인 부분으로서 자식에 추가되는 다른 속성 소스 보다 우선 순위가 낮 습니다. 이러한 속성 소스의 내용을 사용자 정의하는 방법에 대한 지침 은 [아래](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#customizing-bootstrap-properties) 를 참조 [하십시오](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#customizing-bootstrap-properties) .





속성 소스의 순서 규칙 때문에 "부트 스트랩"항목이 우선적으로 적용되지만 이러한 항목에는 우선 순위 `bootstrap.yml`가 매우 낮지 만 기본값을 설정하는 데 사용할 수 있는 데이터가 포함되어 있지 않습니다 .





`ApplicationContext`자신 만의 인터페이스를 사용하거나 `SpringApplicationBuilder`편리한 메소드 ( `parent()`, `child()`및 `sibling()`) 를 사용하여 작성한 상위 컨텍스트를 설정하여 컨텍스트 계층 구조를 확장 할 수 있습니다 . 부트 스트랩 컨텍스트는 자신이 직접 생성 한 가장 상위의 조상의 부모가됩니다. 계층 구조의 모든 컨텍스트는 부모로부터 하위 노드로 부주의하게 값을 승격시키는 것을 피하기 위해 자체 "부트 스트랩"속성 소스 (비어 있음)를 갖습니다. 계층 구조의 모든 컨텍스트는 (원칙적으로) `spring.application.name`구성 서버가있는 경우 다른 원격 속성 소스를 가질 수 있습니다 . 일반 Spring 애플리케이션 컨텍스트 동작 규칙은 속성 확인에 적용된다. 자식 컨텍스트의 속성은 부모 컨텍스트의 속성보다 우선하며,





이 `SpringApplicationBuilder`옵션을 사용하면 `Environment`전체 계층 구조 를 공유 할 수 있지만 기본값은 아닙니다. 따라서 특히 형제 상황은 부모와 공통된 사항을 공유 할지라도 동일한 프로필이나 속성 소스를 가질 필요가 없습니다.







### 부트 스트랩 속성 위치 변경



`bootstrap.yml`(또는 `.properties`) 위치를 사용하여 지정할 수 있습니다 `spring.cloud.bootstrap.name`(기본 "부트 스트랩") 또는 `spring.cloud.bootstrap.location`시스템 등록 정보에서 예 (기본 빈을). 이러한 속성 `spring.config.*` 은 같은 이름을 가진 변형 처럼 동작합니다. 실제로 `ApplicationContext`해당 속성을 해당 속성 에 설정 하여 부트 스트랩 을 설정하는 데 사용됩니다 `Environment`. 활성 프로파일이 `spring.profiles.active`있거나 ( `Environment`빌드중인 컨텍스트 의 API를 통해 ) 프로파일의 속성은 일반 `bootstrap-development.properties`"Spring" 응용 프로그램 (예 : "개발"프로파일) 에서와 마찬가지로로드됩니다 .







### 원격 등록 정보 값 재 지정



부트 스트랩 컨텍스트에 의해 응용 프로그램에 추가되는 속성 소스는 종종 구성 서버와 같은 "원격"이며, 기본적으로 명령 줄을 제외하고는 로컬에서 재정의 할 수 없습니다. 응용 프로그램이 자신의 시스템 등록 정보 또는 구성 파일을 사용하여 원격 등록 정보를 대체 할 수있게하려면 원격 등록 정보 소스가 설정을 통해 권한을 부여해야합니다 `spring.cloud.config.allowOverride=true`(로컬로 설정하는 것이 효과가 없습니다). 플래그가 설정되면 시스템 등록 정보 및 응용 프로그램의 로컬 구성과 관련하여 원격 등록 정보의 위치를 ​​제어 할 수있는 세분화 된 설정이 있습니다. `spring.cloud.config.overrideNone=true`로컬 등록 정보 소스로 대체하고 `spring.cloud.config.overrideSystemProperties=false`시스템 등록 정보 및 환경 변수 만 원격 설정이지만 로컬 구성 파일은 제외합니다.







### 부트 스트랩 구성 사용자 정의



부트 스트랩 컨텍스트는 `/META-INF/spring.factories`키 아래 에 항목을 추가하여 원하는 모든 작업을하도록 교육받을 수 있습니다 `org.springframework.cloud.bootstrap.BootstrapConfiguration`. 이것은 `@Configuration`컨텍스트를 만드는 데 사용될 Spring 클래스 의 쉼표로 구분 된 목록입니다 . autowiring을 위해 기본 응용 프로그램 컨텍스트에서 사용 가능하게하려는 모든 bean을 여기에서 작성할 수 있으며 또한 `@Beans`유형 에 대한 특별 계약이 `ApplicationContextInitializer`있습니다. `@Order` 시작 순서를 제어하려는 경우 클래스를 표시 할 수 있습니다 (기본 순서는 "마지막"입니다).













경고

추가 `BootstrapConfiguration`하는 클래스가 `@ComponentScanned`실수로 "기본"응용 프로그램 컨텍스트 에 있지 않은 사용자 지정 을 추가 할 때주의해야 합니다. 필요하지 않을 수도 있습니다. 사용자 `@ComponentScan`또는 `@SpringBootApplication` 주석이 달린 구성 클래스에서 아직 다루지 않은 부팅 구성 클래스에는 별도의 패키지 이름을 사용하십시오 .|











부트 스트랩 프로세스는 초기화 프로세스를 주 `SpringApplication`인스턴스 (즉, 독립 실행 형 응용 프로그램으로 실행 중이거나 응용 프로그램 서버에 배포되어 있는지 여부와 상관없이 일반적인 스프링 부팅 시작 시퀀스)에 주입하여 종료됩니다. 먼저 부트 스트랩 컨텍스트가 발견 된 클래스에서 생성 된 `spring.factories`다음 모든 `@Beans`유형 이 시작되기 전에 `ApplicationContextInitializer`주에 추가됩니다 `SpringApplication`.







### 부트 스트랩 속성 소스 사용자 정의



부트 스트랩 프로세스에 의해 추가 된 외부 구성의 기본 속성 소스는 구성 서버이지만 `PropertySourceLocator`부트 스트랩 컨텍스트 (via `spring.factories`) 에 유형의 bean을 추가하여 추가 소스를 추가 할 수 있습니다 . 이 기능을 사용하여 다른 서버 또는 데이터베이스와 같은 추가 속성을 삽입 할 수 있습니다.





예를 들어, 다음과 같은 사소한 사용자 정의 위치 지정자를 고려하십시오.







    @Configuration
    public class CustomPropertySourceLocator implements PropertySourceLocator {

        @Override
        public PropertySource<?> locate(Environment environment) {
            return new MapPropertySource("customProperty",
                    Collections.<String, Object>singletonMap("property.from.sample.custom.source", "worked as intended"));
        }

    }







`Environment`전달되는이의 하나입니다 `ApplicationContext`우리가 추가 속성 소스를 공급하는 일, 즉 생성되는 약. 그것은 이미 Spring Boot가 제공하는 일반적인 속성 소스를 가지고있을 것이므로, 이것들을 사용하여 특정 속성 소스를 찾을 수 있습니다 `Environment`(예를 들어 `spring.application.name`기본 Config Server 속성 소스 위치 지정자에서와 같이).





이 클래스가 들어있는 jar 파일을 만든 다음 포함 파일을 추가하면 다음과 `META-INF/spring.factories`같습니다.







```org.springframework.cloud.bootstrap.BootstrapConfiguration = sample.custom.CustomPropertySourceLocator```







"customProperty" `PropertySource`는 해당 classpath에있는 jar를 포함하는 모든 응용 프로그램에 표시됩니다.







### 환경 변화



응용 프로그램은 `EnvironmentChangeEvent`표준 방식의 몇 가지 방법으로 변경 사항을 수신 하고 이에 대응합니다 ( 사용자가 정상적으로 `ApplicationListeners`추가 할 수 있음 `@Beans`). an `EnvironmentChangeEvent`이 관찰되면 변경된 키 값 목록을 가지게되며, 응용 프로그램은 키 값 목록을 사용하여 다음을 수행합니다.





*   `@ConfigurationProperties`컨텍스트에서 빈을 다시 바인드하십시오.

*   모든 속성에 대한 로거 수준 설정 `logging.level.*`





구성 클라이언트는 기본적으로 변경 사항을 폴링하지 않으며 `Environment`일반적으로 변경 사항을 감지하는 방법은 사용하지 않는 것이 좋습니다 (주석으로 설정할 수도 `@Scheduled`있음). 확장 된 클라이언트 응용 프로그램이 `EnvironmentChangeEvent`있는 경우 변경 사항을 폴링하는 대신 모든 인스턴스에 브로드 캐스팅하는 것이 좋습니다 (예 : [Spring Cloud Bus 사용](https://github.com/spring-cloud/spring-cloud-bus) ).





여기 `EnvironmentChangeEvent`에는 실제로 `Environment` 이벤트 를 변경 하고 이벤트를 게시 할 수있는 한 대규모 새로 고침 사용 사례 가 포함됩니다 (이러한 API는 공개이고 핵심 스프링의 일부 임). 엔드 포인트 `@ConfigurationProperties`를 방문 하여 변경 사항이 빈에 바인딩되어 있는지 확인할 수 있습니다 `/configprops`(일반적인 스프링 부트 액추에이터 기능). 예를 들어, a `DataSource`는 `maxPoolSize`런타임시 변경 될 수 있습니다 ( `DataSource`스프링 부트로 작성된 기본값 은 `@ConfigurationProperties`bean입니다). 그리고 동적으로 용량을 늘립니다. 리 바인딩 `@ConfigurationProperties`은 새로 고침을보다 세부적으로 제어해야하는 또 다른 대규모 클래스의 유스 케이스를 다루지 않으며 전체적으로 원자 단위로 변경해야하는 부분을 처리하지 않습니다 `ApplicationContext`. 우리가 그 문제를 해결합니다 `@RefreshScope`.







### 새로 고침 범위



설정 변경이있을 때 특별한 `@Bean`표시가있는 것으로 표시된 스프링 `@RefreshScope`. 이것은 초기화 될 때만 구성을 주입시키는 상태 보존빈의 문제점을 해결합니다. 예를 들어 , `DataSource`를 통해 데이터베이스 URL이 변경 될 때 연결에 열린 연결이있는 경우 해당 연결 `Environment`의 소유자가 수행중인 작업을 완료 할 수 있기를 바랍니다. 그런 다음 누군가 다음에 풀에서 연결을 빌리면 새 URL로 연결됩니다.





새로 고침 범위 Bean은 사용시 초기화되는 (즉, 메서드가 호출 될 때) 지연 프록시이며 범위는 초기화 된 값의 캐시 역할을합니다. 다음 메소드 호출시 빈을 강제로 다시 초기화하려면 캐시 엔트리를 무효화하면된다.





는 `RefreshScope`문맥에 콩이며 공개 방법이 `refreshAll()`대상 캐시를 삭제하여 범위에있는 모든 콩을 새로 고칠 수 있습니다. `refresh(String)`개별 bean을 이름별로 새로 고치는 메소드 도 있습니다 . 이 기능은 `/refresh`엔드 포인트 에서 공개됩니다 (HTTP 또는 JMX를 통해).













노트



`@RefreshScope``@Configuration` 수업에서 (기술적으로) 작동 하지만 놀라운 행동으로 이어질 수 있습니다. 즉 , 해당 클래스에 정의 된 모든 것이 자체 라는 것을 의미 하지는 **않습니다** . 특히, 빈에 의존하는 모든 것은 리프레시가 시작될 때 갱신되는 것에 의지 할 수 없습니다 (리프레시시 재 빌드되고 종속성을 다시 주입 할 경우) 새로 고침에서 초기화 됨 ). `@Beans``@RefreshScope``@RefreshScope``@Configuration`|













### 암호화 및 암호 해독



Spring Cloud에는 `Environment`속성 값을 로컬에서 해독하기위한 전처리 기가 있습니다. 구성 서버와 동일한 규칙을 따르며 동일한 외부 구성을 통해 `encrypt.*`합니다. 따라서 형식의 암호화 된 값을 사용할 수 `{cipher}*`있으며 유효한 키가있는 한 주 응용 프로그램 컨텍스트가 얻어지기 전에 암호가 해독 `Environment`됩니다. 애플리케이션에서 암호화 기능을 사용하려면 Classpath에 스프링 시큐리티 RSA (Maven이 "org.springframework.security : spring-security-rsa"를 조정)를 포함시켜야하며 JVM에서 강력한 JCE 확장 기능이 필요하다.





"잘못된 키 크기"로 인해 예외가 발생하고 Sun의 JDK를 사용하는 경우 JCE (Java Cryptography Extension) 무제한 강도 관할 정책 파일을 설치해야합니다. 자세한 내용은 다음 링크를 참조하십시오.





*   [Java 6 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-6-download-429243.html)

*   [Java 7 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html)

*   [Java 8 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html)





JDK / jre / lib / security 폴더 (사용중인 JRE / JDK x64 / x86 버전)로 파일을 추출하십시오.







### 종점



스프링 부트 액츄에이터 애플리케이션에는 몇 가지 추가 관리 엔드 포인트가 있습니다.





*   POST는 다음의 제품에 `/env`를 업데이트 `Environment`하고 바인딩 `@ConfigurationProperties`과 수준을 기록

*   `/refresh`부트 스트랩 컨텍스트를 다시로드하고 `@RefreshScope`콩 을 새로 고침

*   `/restart``ApplicationContext`그것을 닫고 다시 시작하기 위해 (기본적으로 비활성화 됨)

*   `/pause`및 `/resume`호출을위한 `Lifecycle`방법 ( `stop()`및 `start()`온 `ApplicationContext`)











## Spring Cloud Commons : 공통 추상화





서비스 발견,로드 밸런싱 및 회로 차단기와 같은 패턴은 모든 Spring Cloud 클라이언트가 구현과 독립적 (예 : Eureka 또는 Consul을 통한 검색) 할 수있는 공통적 인 추상화 계층에 적합합니다.





### @EnableDiscoveryClient



Commons은 `@EnableDiscoveryClient`주석을 제공합니다 . 이 `DiscoveryClient`인터페이스를 통해 인터페이스의 구현을 찾습니다 `META-INF/spring.factories`. Discovery Client의 구현 `spring.factories`은 `org.springframework.cloud.client.discovery.EnableDiscoveryClient`키 아래 에 구성 클래스를 추가합니다 . 구현 사례 `DiscoveryClient`: [Spring Cloud Netflix Eureka](http://cloud.spring.io/spring-cloud-netflix/) , [Spring Cloud Consul Discovery](http://cloud.spring.io/spring-cloud-consul/) 및 [Spring Cloud Zookeeper Discovery](http://cloud.spring.io/spring-cloud-zookeeper/) .





기본적으로 구현은 `DiscoveryClient`로컬 스프링 부트 서버를 원격 검색 서버에 자동 등록합니다. `autoRegister=false`에서 설정하여 비활성화 할 수 있습니다 `@EnableDiscoveryClient`.







### ServiceRegistry



풍경은 이제 제공 `ServiceRegistry`등의 방법을 제공하는 인터페이스 `register(Registration)`및 `deregister(Registration)`사용자 정의 등록 서비스를 제공 할 수 있습니다. `Registration`마커 인터페이스입니다.





#### Service Registry 액추에이터 엔드 포인트



`/service-registry`액추에이터 종점 가공에 의해 제공된다. 이 엔드 포인트 `Registration`는 Spring Application Context 의 빈에 의존한다. `/service-registry/instance-status`GET을 통해 전화하면 의 상태가 반환 `Registration`됩니다. `String`본문이 있는 동일한 끝점에 대한 POST 는 현재 상태를 `Registration`새 값으로 변경합니다. `ServiceRegistry`상태 업데이트를 위해 허용 된 값 및 상태 에 대해 보류 된 값에 대해 사용중인 구현 의 설명서를 참조하십시오 .









### 로드 밸런서 클라이언트로서의 Spring RestTemplate



`RestTemplate`자동으로 리본을 사용하도록 구성 할 수 있습니다. 균형 부하를 만들려면 `RestTemplate`를 생성 `RestTemplate` `@Bean`하고 사용 `@LoadBalanced`규정.













경고

`RestTemplate`빈은 더 이상 자동 구성을 통해 만들어집니다. 개별 응용 프로그램에서 만들어야합니다.|













    @Configuration
    public class MyConfiguration {

        @LoadBalanced
        @Bean
        RestTemplate restTemplate() {
            return new RestTemplate();
        }
    }

    public class MyClass {
        @Autowired
        private RestTemplate restTemplate;

        public String doOtherStuff() {
            String results = restTemplate.getForObject("http://stores/stores", String.class);
            return results;
        }
    }







URI는 가상 호스트 이름 (예 : 호스트 이름이 아닌 서비스 이름)을 사용해야합니다. 리본 클라이언트는 전체 실제 주소를 만드는 데 사용됩니다. 설정 방법에 대한 자세한 내용 은 [RibbonAutoConfiguration](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/ribbon/RibbonAutoConfiguration.java) 을 참조하십시오 `RestTemplate`.





#### 실패한 요청 다시 시도



로드 균형 조정 `RestTemplate`은 실패한 요청을 다시 시도하도록 구성 할 수 있습니다. 기본적으로이 논리는 비활성화되어 있으므로 설정을 통해 활성화 할 수 있습니다 `spring.cloud.loadbalancer.retry.enabled=true`. 로드 균형 조정 `RestTemplate`은 실패한 요청을 다시 시도하는 것과 관련된 일부 리본 구성 값을 사용합니다. 당신이 사용할 수있는 속성은 `client.ribbon.MaxAutoRetries`, `client.ribbon.MaxAutoRetriesNextServer`하고 `client.ribbon.OkToRetryOnAllOperations`. [속성의 용도](https://github.com/Netflix/ribbon/wiki/Getting-Started#the-properties-file-sample-clientproperties) 에 대한 설명은 [리본 설명서](https://github.com/Netflix/ribbon/wiki/Getting-Started#the-properties-file-sample-clientproperties) 를 참조하십시오 .













노트

`client` 위의 예에서 리본 클라이언트의 이름으로 바꿔야합니다.|















### 여러 RestTemplate 객체



`RestTemplate`로드 균형 조정 을 원하지 않으면, `RestTemplate` 빈을 작성하고 정상적으로 주입하십시오. 로드 균형 `RestTemplate use the `@LoadBalanced`조정자 를 액세스 할 때 `@Bean`.













중대한

통지 `@Primary`일반에 주석 `RestTemplate`규정되지 않은 명확하게하기 위해, 아래의 예에서 선언을 `@Autowired`주입.|













    @Configuration
    public class MyConfiguration {

        @LoadBalanced
        @Bean
        RestTemplate loadBalanced() {
            return new RestTemplate();
        }

        @Primary
        @Bean
        RestTemplate restTemplate() {
            return new RestTemplate();
        }
    }

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















팁

대신에 `java.lang.IllegalArgumentException: Can not set org.springframework.web.client.RestTemplate field com.my.app.Foo.restTemplate to com.sun.proxy.$Proxy89`주사 `RestOperations`하거나 설정을 시도하는 것과 같은 오류가 표시 됩니다 `spring.aop.proxyTargetClass=true`.|













### 네트워크 인터페이스 무시



때로는 특정 명명 된 네트워크 인터페이스를 무시하여 서비스 검색 등록 (예 : Docker 컨테이너에서 실행)에서 제외 할 수있는 경우가 있습니다. 원하는 네트워크 인터페이스가 무시되도록하는 정규식 목록을 설정할 수 있습니다. 다음 구성은 "docker0"인터페이스와 "veth"로 시작하는 모든 인터페이스를 무시합니다.





application.yml



```봄: 구름: inetutils : ignoredInterfaces : - 도커 0 - 베스. *```







또한 정규식 목록을 사용하여 지정된 네트워크 주소 만 사용하도록 할 수 있습니다.





application.yml



```봄: 구름: inetutils : preferredNetworks : - 192.168 - 10.0```







사이트 로컬 주소 만 사용하도록 할 수도 있습니다. 사이트 로컬 주소에 대한 자세한 내용 은 [Inet4Address.html.isSiteLocalAddress ()](https://docs.oracle.com/javase/8/docs/api/java/net/Inet4Address.html#isSiteLocalAddress--) 를 참조하십시오.





application.yml



```봄: 구름: inetutils : useOnlySiteLocalInterfaces : true```











# 스프링 클라우드 구성



Spring Cloud Config는 분산 시스템에서 외부화 된 구성을위한 서버 및 클라이언트 측 지원을 제공합니다. 구성 서버를 사용하면 모든 환경에서 응용 프로그램의 외부 속성을 중앙에서 관리 할 수 ​​있습니다. 클라이언트와 서버 모두에 대한 개념은 Spring `Environment`과 `PropertySource`추상화 와 동일하게 매핑되므로 Spring 애플리케이션에 매우 잘 맞지만 모든 언어로 실행되는 모든 애플리케이션에서 사용할 수 있습니다. 애플리케이션이 개발 파이프 라인을 통해 개발에서 테스트 및 프로덕션으로 이동하면 해당 환경 간의 구성을 관리 할 수 ​​있으며 마이그레이션 할 때 실행하는 데 필요한 모든 기능을 애플리케이션에 적용 할 수 있습니다. 서버 저장소 백엔드의 기본 구현은 git을 사용하므로 레이블이있는 구성 환경 버전을 쉽게 지원하므로, 뿐만 아니라 콘텐츠 관리를위한 다양한 툴링에 액세스 할 수 있습니다. 대체 구현을 추가하고 Spring 구성으로 플러그인을 쉽게 삽입 할 수 있습니다.





## 빠른 시작





서버를 시작하십시오.







```$ cd spring-cloud-config-server $ ../mvnw spring-boot : run```







서버는 스프링 부트 응용 프로그램이므로 원하는 경우 IDE에서 실행할 수 있습니다 (기본 클래스는 `ConfigServerApplication`). 그런 다음 클라이언트를 사용해보십시오.







```$ curl localhost : 8888 / foo / development { "name": "development", "label": "master", "propertySources": [ { "name": "https://github.com/scratches/config-repo/foo-development.properties", "source": { "bar": "spam"}} { "name": "https://github.com/scratches/config-repo/foo.properties", "source": { "foo": "bar"}} ]}```







속성 소스를 찾는 기본 전략은 git 저장소 (at `spring.cloud.config.server.git.uri`) 를 복제하고 이를 사용하여 mini를 초기화하는 것 `SpringApplication`입니다. 미니 응용 프로그램 `Environment`은 속성 소스를 열거하고 JSON 끝점을 통해 게시하는 데 사용됩니다.





HTTP 서비스에는 다음과 같은 형식의 자원이 있습니다.







```/ {application} / {profile} [/ {label}] /{application}-{profile}.yml /{label}/{application}-{profile}.yml /{application}-{profile}.properties /{label}/application}-{profile}.properties```







은 "응용 프로그램"으로 주입되는 곳 `spring.config.name`에서 `SpringApplication`(즉, 일반 봄 부팅 응용 프로그램에서 "응용 프로그램"일반적으로 어떤), "프로필"활성 프로필 (또는 쉼표로 구분 된 속성 목록) 및 "레이블"하는 선택적 git 레이블 (기본값은 "master"입니다.)





Spring Cloud Config Server는 git 저장소 (제공되어야 함)에서 원격 클라이언트에 대한 구성을 가져옵니다.







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo







### 클라이언트 측 사용



이러한 기능을 응용 프로그램에서 사용하려면 spring-cloud-config-client (예 : config-client 또는 샘플 응용 프로그램의 테스트 사례 참조)에 따라 달라지는 Spring Boot 응용 프로그램으로 빌드하면됩니다. 의존성을 추가하는 가장 편리한 방법은 스프링 부트 스타터를 이용하는 것 `org.springframework.cloud:spring-cloud-starter-config`입니다. 또한 `spring-cloud-starter-parent`Maven 사용자를위한 부모 pom과 BOM ( )과 Gradle 및 Spring CLI 사용자를위한 Spring IO 버전 관리 등록 정보 파일이 있습니다. Maven 구성 예 :





pom.xml



    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>1.3.5.RELEASE</version>
        <relativePath /> <!-- lookup parent from repository -->
    </parent>

    <dependencyManagement>
        <dependencies>
            <dependency>
                <groupId>org.springframework.cloud</groupId>
                <artifactId>spring-cloud-dependencies</artifactId>
                <version>Brixton.RELEASE</version>
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







그런 다음이 간단한 HTTP 서버와 같은 표준 스프링 부트 애플리케이션을 만들 수 있습니다.







```@SpringBootApplication @RestController public class Application {
 @RequestMapping ( "/") public String home () { return "Hello World!"; }
 공공 정적 무효 메인 (문자열 [] args) { SpringApplication.run (Application.class, args); }
 }```







실행될 때 포트 8888의 기본 로컬 구성 서버에서 외부 구성을 선택합니다 (실행중인 경우). 시작 동작을 수정하려면 `bootstrap.properties`( `application.properties`예 : 응용 프로그램 컨텍스트의 부트 스트랩 단계 와 마찬가지로) 구성 서버의 위치를 ​​변경할 수 있습니다 . 예 :







```spring.cloud.config.uri : http://myconfigserver.com```







부트 스트랩 `/env`속성은 우선 순위가 높은 속성 소스로 엔드 포인트에 표시됩니다 ( 예 :







```$ curl localhost : 8080 / env { "프로필": [], "configService : https : //github.com/spring-cloud-samples/config-repo/bar.properties": { "foo": "bar"}, "servletContextInitParams": {}, "systemProperties": {...}, ... }```







( "configService : <원격 저장소의 URL / <파일 이름>"이라는 속성 소스에는 "bar"값을 갖는 속성 "foo"가 포함되어 있으며 가장 우선 순위가 높음).













노트

속성 소스 이름의 URL은 config 서버 URL이 아닌 git 저장소입니다.|

















## 스프링 클라우드 구성 서버





서버는 외부 구성 (이름 - 값 쌍 또는 이와 동등한 YAML 내용)을위한 HTTP, 자원 기반 API를 제공합니다. 서버는 어노테이션을 사용하여 스프링 부트 애플리케이션에 쉽게 임베딩 할 수 있습니다 `@EnableConfigServer`. 그래서이 응용 프로그램은 설정 서버입니다 :





ConfigServer.java



    @SpringBootApplication
    @EnableConfigServer
    public class ConfigServer {
      public static void main(String[] args) {
        SpringApplication.run(ConfigServer.class, args);
      }
    }







모든 스프링 부트 응용 프로그램과 마찬가지로 기본적으로 포트 8080에서 실행되지만 다양한 방법으로 기존 포트 8888로 전환 할 수 있습니다. 기본 구성 저장소를 설정하는 가장 쉬운 방법 은 구성 서버 jar `spring.config.name=configserver`에 a `configserver.yml`를 사용하는 것입니다. 또 다른 방법은 자신의 것을 사용하는 것입니다 `application.properties`.





application.properties



    server.port: 8888
    spring.cloud.config.server.git.uri: file://${user.home}/config-repo







여기서는 `${user.home}/config-repo`YAML 및 특성 파일을 포함하는 git 저장소가 있습니다.













노트

Windows에서 드라이브 접두사가 절대적이면 파일 URL에 여분의 "/"가 필요합니다 (예 :) `[file:///${user.home}/config-repo](file:///$%7Buser.home%7D/config-repo)`.|



















팁





위의 예에서 git 저장소를 만드는 방법은 다음과 같습니다.







```$ cd $ HOME $ mkdir config-repo $ cd config-repo $ git init. $ echo info.foo : bar> application.properties $ git add -A. $ git commit -m "application.properties 추가"```























경고

git 저장소에 로컬 파일 시스템을 사용하는 것은 테스트 용입니다. 프로덕션 환경에서 서버를 사용하여 구성 저장소를 호스트하십시오.|



















경고

텍스트 파일 만 저장하면 구성 저장소의 초기 복제본이 빠르고 효율적입니다. 바이너리 파일, 특히 큰 파일을 저장하기 시작하면 서버의 구성 및 / 또는 메모리 부족 오류에 대한 첫 번째 요청이 지연 될 수 있습니다.|











### 환경 저장소



구성 서버의 구성 데이터를 어디에 저장 하시겠습니까? 이 동작을 제어하는 ​​전략은 `EnvironmentRepository`서빙 `Environment`객체입니다. 이것은 `Environment`Spring의 도메인의 얕은 복사본입니다 `Environment`( `propertySources`주요 기능 포함). `Environment`자원은 세 가지 변수에 의해 매개 변수화된다 :





*   `{application}` 클라이언트 쪽에서 "spring.application.name"에 매핑됩니다.

*   `{profile}`클라이언트의 "spring.profiles.active"에 매핑됩니다 (쉼표로 구분 된 목록). 과

*   `{label}` 이 파일은 "버전 관리"된 설정 파일의 레이블을 지정하는 서버 측 기능입니다.





저장소 구현은 일반적으로 "spring.config.name"에서 `{application}`매개 변수 와 동일한 구성 파일을로드하고 "spring.profiles.active"는 매개 변수 와 동일한 Spring Boot 응용 프로그램처럼 작동 `{profiles}`합니다. 프로필의 우선 순위 규칙은 일반 Boot 응용 프로그램과 동일합니다. 활성 프로필은 기본값보다 우선하며, 여러 프로필이있는 경우 마지막 항목이 우선합니다 (예 : a에 항목 추가 `Map`).





예 : 클라이언트 응용 프로그램에이 부트 스트랩 구성이 있습니다.





bootstrap.yml



    spring:
      application:
        name: foo
      profiles:
        active: dev,mysql







(보통 Spring Boot 애플리케이션에서 이러한 속성은 환경 변수 또는 명령 행 인자로 설정 될 수 있습니다).





저장소가 파일 기반 인 경우 서버는 `Environment`from `application.yml`(모든 클라이언트 간 공유) 및 `foo.yml`( `foo.yml`우선 순위를두고) 작성합니다. YAML 파일에 스프링 프로파일을 가리키는 문서가있는 경우, 프로파일 우선 순위 (나열된 프로파일 순서대로)로 적용되고, 프로파일 특정 YAML (또는 특성) 파일이있는 경우 YAML 파일보다 높은 우선 순위로 적용됩니다 기본값. 우선 순위가 높을수록 `PropertySource`앞부분에 나열된 것과 유사 합니다 `Environment`. (이것들은 독립 실행 형 Spring Boot 응용 프로그램과 동일한 규칙입니다.)





#### 힘내 백엔드



기본 구현은 `EnvironmentRepository`Git 백엔드 를 사용합니다. 이는 업그레이드 및 물리적 환경을 관리하고 변경 사항을 감사하는 데 매우 편리합니다. 저장소 위치를 변경하려면 구성 서버 (예 :)에서 "spring.cloud.config.server.git.uri"구성 등록 정보를 설정할 수 있습니다 `application.yml`. `file:`접두어 로 설정하면 로컬 저장소에서 작동하므로 서버없이 쉽고 빠르게 시작할 수 있지만이 경우 서버는 복제하지 않고 로컬 저장소에서 직접 작동합니다 (그렇지 않은 경우 중요하지 않습니다). Config Server가 "원격"저장소를 변경하지 않기 때문에 노출되지 않습니다. 구성 서버를 확장하여 가용성을 높이려면 서버의 모든 인스턴스를 동일한 리포지토리로 지정해야합니다. 따라서 공유 파일 시스템 만 작동합니다. `ssh:`이 경우에도 공유 파일 시스템 저장소에 프로토콜 을 사용하는 것이 더 좋으므로 서버가이를 복제하고 로컬 작업 사본을 캐시로 사용할 수 있습니다.





이 저장소 구현 `{label}`은 HTTP 자원 의 매개 변수를 git 레이블 (커밋 ID, 분기 이름 또는 태그)에 매핑합니다 . git 브랜치 또는 태그 이름에 슬래시 ( "/")가 포함되어 있으면 HTTP URL의 레이블을 (다른 URL 경로와 모호하지 않게) 특수 문자열 "(_)"로 지정해야합니다. curl과 같은 명령 행 클라이언트를 사용하는 경우 URL의 대괄호 (예 : 따옴표 ''가있는 쉘에서 이스케이프 처리)를 사용할 때주의하십시오.





##### Git URI의 자리 표시 자



봄 클라우드 구성 서버는 대한 자리 표시와 자식 저장소의 URL 지원 `{application}`과 `{profile}`(그리고 `{label}`당신이 그것을 필요로하지만 라벨이 어쨌든 자식 레이블로 적용되는 것을 기억 경우). 따라서 (예를 들어) 다음을 사용하여 "애플리케이션 당 하나의 저장소"정책을 쉽게 지원할 수 있습니다.







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/myorg/{application}







비슷한 패턴을 사용하지만 "프로필 당 하나의 repo"정책을 사용합니다 `{profile}`.







##### 패턴 일치 및 다중 저장소



또한 응용 프로그램 및 프로필 이름에 패턴 일치가있는보다 복잡한 요구 사항에 대한 지원이 있습니다. 패턴 형식은 `{application}/{profile}`와일드 카드 로 쉼표로 구분 된 이름 목록입니다 (와일드 카드로 시작하는 패턴을 따옴표로 묶어야 할 수도 있음). 예:







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







if `{application}/{profile}`패턴과 일치하지 않으면 "spring.cloud.config.server.git.uri"에 정의 된 기본 URI를 사용합니다. 위의 예에서 "단순한"저장소의 경우 패턴이 있습니다 `simple/*`(즉, 모든 프로파일에서 "simple"이라는 하나의 응용 프로그램과 만 일치합니다). "로컬"리포지토리는 모든 프로필에서 "local"로 시작하는 모든 응용 프로그램 이름을 찾습니다 ( `/*`접미어는 프로필 일치 프로그램이없는 모든 패턴에 자동으로 추가됩니다).













노트

위의 "간단한"예제에서 사용 된 "한 줄짜리"단축키는 설정할 유일한 속성이 URI 인 경우에만 사용할 수 있습니다. 다른 것을 설정해야하는 경우 (자격 증명, 패턴 등) 전체 양식을 사용해야합니다.|











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















노트

봄 클라우드에서 끝나지 않는 프로파일을 포함하는 패턴을 추측 할 것이다 `*`당신이 실제로이 패턴으로 시작하는 프로파일의 목록을 일치시킬 것을 의미한다 (그래서 `*/staging`에 대한 바로 가기입니다 `["*/staging", "*/staging,*"]`). 이는 "개발"프로필에서 로컬로 실행해야하는 응용 프로그램과 "클라우드"프로필을 원격으로 실행해야하는 경우에 일반적으로 사용됩니다.|











모든 저장소는 또한 하위 디렉토리에 구성 파일을 선택적으로 저장할 수 있으며 해당 디렉토리를 검색 할 패턴을로 지정할 수 있습니다 `searchPaths`. 예를 들어 최상위 레벨에서 :







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              searchPaths: foo,bar*







이 예제에서 서버는 최상위 레벨과 "foo /"하위 디렉토리 및 이름이 "bar"로 시작하는 하위 디렉토리에서 구성 파일을 검색합니다.





기본적으로 서버는 구성이 처음 요청 될 때 원격 저장소를 복제합니다. 시작할 때 저장소를 복제하도록 서버를 구성 할 수 있습니다. 예를 들어 최상위 레벨에서







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







이 예제에서 서버는 시작시 임의의 요청을 수락하기 전에 팀 -a의 config-repo를 복제합니다. 다른 모든 저장소는 저장소의 구성이 요청 될 때까지 복제되지 않습니다.





원격 저장소에서 HTTP 기본 인증을 사용하려면 "username"및 "password"속성을 URL에 별도로 추가하십시오 (예 :







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              username: trolley
              password: strongpassword







HTTPS와 사용자 자격 증명을 사용하지 않으면 기본 디렉토리 ( `~/.ssh`) 에 키를 저장할 때 SSH가 기본으로 작동 하고 uri는 SSH 위치 (예 : " [git@github.com](mailto:git@github.com) : configuration / cloud- 구성 ". 저장소는 JGit을 사용하여 액세스하므로 해당 문서를 찾을 수 있어야합니다. HTTPS 프록시 설정은 `~/.git/config`시스템 등록 정보 ( `-Dhttps.proxyHost`및 `-Dhttps.proxyPort`) 를 통해 다른 JVM 프로세스와 동일하게 설정 하거나 설정할 수 있습니다 .













팁

`~/.git`디렉토리가 어디 `git config --global`에서 설정을 조작하는지 알지 못하는 경우 (예 :) `git config --global http.sslVerify false`.|













##### Git 검색 경로의 자리 표시 자



Spring Cloud Config Server는 `{application}`및 에 대한 자리 표시자가있는 검색 경로도 지원합니다 `{profile}`( `{label}`필요한 경우). 예:







    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              searchPaths: '{application}'







디렉토리와 동일한 이름의 파일 (최상위 레벨)을 저장소에서 검색합니다. 와일드 카드는 자리 표시자가있는 검색 경로에서도 유효합니다 (일치하는 디렉토리가 검색에 포함됨).









#### 버전 제어 백엔드 파일 시스템 사용











경고

VCS 기반 백엔드 (자식, svn) 파일은 로컬 파일 시스템에 체크 아웃되거나 복제됩니다. 기본적으로 시스템 임시 디렉토리에 접두어 of를 붙입니다 `config-repo-`. 리눅스에서, 예를 들어 그것은 가능할 수 있습니다 `/tmp/config-repo-<randomid>`. 일부 운영 체제 [에서는 정기적으로](https://serverfault.com/questions/377348/when-does-tmp-get-cleared/377349#377349) 임시 디렉토리 [를](https://serverfault.com/questions/377348/when-does-tmp-get-cleared/377349#377349) 지 웁니다. 이로 인해 속성 누락과 같은 예기치 않은 동작이 발생할 수 있습니다. 이 문제를 피하려면 Config Temp가 사용 하는 디렉터리를 설정 `spring.cloud.config.server.git.basedir`하거나 `spring.cloud.config.server.svn.basedir`시스템 temp 구조에없는 디렉터리로 변경하십시오.|













#### 파일 시스템 백엔드



구성 서버에는 Git을 사용하지 않는 "기본"프로필이 있지만 로컬 클래스 경로 또는 파일 시스템 ( "spring.cloud.config.server"로 가리키는 모든 정적 URL)에서 구성 파일을로드합니다 .native.searchLocations "). 기본 프로필을 사용하려면 "spring.profiles.active = native"를 사용하여 구성 서버를 시작하십시오.













노트

`file:`파일 자원 에 접두사 를 사용하는 것을 잊지 마십시오 (접두사가없는 기본값은 일반적으로 클래스 경로입니다). 어떤 Spring Boot 환경 설정과 마찬가지로 `${}`스타일 환경 자리 표시자를 내장 할 수 있지만 Windows의 절대 경로에는 추가 "/"가 필요하다는 것을 기억하십시오.`[file:///${user.home}/config-repo](file:///$%7Buser.home%7D/config-repo)`|



















경고

the의 기본값 `searchLocations`은 로컬 스프링 부트 응용 프로그램 (so `[classpath:/, classpath:/config, file:./, file:./config]`)과 동일 합니다. 이렇게 `application.properties`하면 서버에있는 속성 소스가 클라이언트에 보내기 전에 제거되므로 서버에서 모든 클라이언트로 노출되지 않습니다 .|



















팁

파일 시스템 백엔드는 신속하게 시작하고 테스트하기에 좋습니다. 프로덕션 환경에서 사용하려면 파일 시스템이 안정적이어야하며 모든 구성 서버 인스턴스에서 공유해야합니다.|











검색 위치에 대한 자리 표시자를 포함 할 수 있습니다 `{application}`, `{profile}`하고 `{label}`. 이 방법으로 경로의 디렉토리를 분리하고 자신에게 맞는 전략 (예 : 응용 프로그램 별 하위 디렉토리 또는 프로필 당 하위 디렉토리)을 선택할 수 있습니다.





당신이 검색 위치에 자리 표시자를 사용하지 않는 경우,이 저장소는 추가 `{label}`속성 파일이 각 검색 위치에서로드되도록, 검색 경로에 접미사로 HTTP 자원의 매개 변수 **및** 레이블과 동일한 이름의 하위 디렉토리 ( 레이블이 지정된 속성은 Spring 환경에서 우선 순위를가집니다). 따라서 자리 표시자가없는 기본 동작은 다음으로 끝나는 검색 위치 추가 `/{label}/. For example `file:/tmp/config` 와 동일합니다.`file:/tmp/config,file:/tmp/config/{label}`







#### 모든 응용 프로그램과 구성 공유



파일 기반 (예 : 자식, svn 및 네이티브) 저장소의 경우 파일 이름이있는 `application*`자원이 모든 클라이언트 응용 프로그램간에 공유됩니다 ( `application.properties`예 `application.yml`: `application-*.properties`등). 이러한 파일 이름의 자원을 사용하여 전역 기본값을 구성하고 필요에 따라 응용 프로그램 특정 파일에 의해 대체 될 수 있습니다.


The #_property_overrides [속성 재정의] 기능은 전역 기본값을 설정하는 데 사용할 수도 있으며 자리 표시 자 응용 프로그램에서 로컬 우선 순위를 재정의 할 수 있습니다.



팁

"네이티브"프로파일 (로컬 파일 시스템 백엔드)을 사용하면 서버 자체 구성의 일부가 아닌 명시적인 검색 위치를 사용하는 것이 좋습니다. 그렇지 않으면 `application*` 기본 검색 위치의 리소스가 서버의 일부이기 때문에 제거됩니다.





#### 속성 재정의



구성 서버에는 정상적인 스프링 부트 훅을 사용하여 응용 프로그램이 실수로 변경할 수없는 모든 응용 프로그램에 구성 등록 정보를 제공 할 수있는 "재정의"기능이 있습니다. 재정의를 선언하려면 이름 - 값 쌍의지도를 추가하면됩니다 `spring.cloud.config.server.overrides`. 예를 들어







    spring:
      cloud:
        config:
          server:
            overrides:
              foo: bar







구성 클라이언트 인 모든 응용 프로그램이 `foo=bar` 자체 구성과 독립적 으로 읽을 수 있게합니다. 물론 응용 프로그램은 구성 서버의 데이터를 원하는 방식으로 사용할 수 있으므로 재정의는 적용 할 수 없지만 Spring Cloud 구성 클라이언트 인 경우 유용한 기본 동작을 제공합니다.













팁

백 슬래시 ( "\")를 사용하여 "$"또는 "{"를 이스케이프 처리하여 "$ {}"이있는 일반 환경의 스프링 환경 자리 표시자를 이스케이프 (및 클라이언트에서 `\${app.foo:bar}`해결할 수 있습니다. 자체 "app.foo"를 제공합니다. YAML에서는 백 슬래시 자체를 이스케이프 할 필요가 없지만 서버에서 재정의를 구성 할 때 수행하는 등록 정보 파일에서주의해야합니다.|











클라이언트의 모든 재정의 우선 순위를 기본값과 비슷하게 변경하여 응용 프로그램 `spring.cloud.config.overrideNone=true`이 원격 저장소에 플래그 (기본값은 false) 를 설정하여 환경 변수 또는 시스템 등록 정보에 자체 값을 제공 할 수 있습니다 .









### 건강 지표



구성 서버에는 구성 `EnvironmentRepository`이 작동 하는지 확인하는 상태 표시기가 함께 제공됩니다 . 디폴트 `EnvironmentRepository` 에서는, 어플리케이션에 의해 지정된 어플리케이션 `app`, `default`프로파일, 및 구현으로 제공되는 디폴트의 라벨을 `EnvironmentRepository`요구합니다.





사용자 정의 프로파일 및 사용자 정의 레이블과 함께 더 많은 응용 프로그램을 점검하도록 Health 표시기를 구성 할 수 있습니다 (예 :







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







설정을 통해 상태 표시기를 사용 불가능하게 할 수 있습니다 `spring.cloud.config.server.health.enabled=false`.







### 보안



물리적 인 네트워크 보안에서부터 OAuth2 베어러 토큰에 이르는 모든 방식으로 구성 서버를 자유롭게 보호 할 수 있으며 Spring Security와 Spring Boot를 사용하면 쉽게 모든 것을 할 수 있습니다.





기본 Spring Boot로 구성된 HTTP 기본 보안을 사용하려면 클래스 패스에 Spring Security를 ​​포함하기 만하면 `spring-boot-starter-security`된다. 기본값은 "사용자"사용자 이름과 무작위로 생성 된 암호입니다. 실제로는 그다지 유용하지 않을 수 있으므로 암호를 구성 `security.user.password`하고 (암호화하여) 암호 를 암호화하는 것이 좋습니다 (아래 참조). ).







### 암호화 및 암호 해독











중대한

**전제 조건 :** 암호화 및 암호 해독 기능을 사용하려면 JVM에 전체 강도의 JCE가 설치되어 있어야합니다 (기본값은 없습니다). Oracle에서 "Java Cryptography Extension (JCE) 무제한 강도 관할 정책 파일"을 다운로드하고 설치 지침을 따르십시오 (기본적으로 JRE lib / security 디렉토리에있는 2 개의 정책 파일을 다운로드 한 정책 파일로 대체하십시오).|











원격 속성 소스에 암호화 된 내용 (다음으로 시작하는 값 `{cipher}`)이 들어 있으면 HTTP를 통해 클라이언트에 보내기 전에 해독됩니다. 이 설정의 가장 큰 장점은 속성 값이 "휴식"(예 : 자식 저장소에서) 일 때 일반 텍스트 일 ​​필요가 없다는 것입니다. 값을 암호 해독 할 수 없으면이 값은 속성 소스에서 제거되고 추가 속성은 같은 키로 추가되지만 앞에 "invalid"가 붙습니다. "적용 할 수 없음"을 의미하는 값 (대개 "<n / a>"). 이것은 주로 암호문이 실수로 누설되거나 암호로 사용되는 것을 방지하기위한 것입니다.





config 클라이언트 응용 프로그램에 대한 원격 구성 저장소를 설정하는 경우 `application.yml`다음과 같이이를 포함 할 수 있습니다 .





application.yml



    spring:
      datasource:
        username: dbuser
        password: '{cipher}FKSAJDFGYOS8F7GLHAKERGFHLSAJ'







.properties 파일의 암호화 된 값은 따옴표로 묶어서는 안됩니다. 그렇지 않으면 값이 해독되지 않습니다.





application.properties



```spring.datasource.username : dbuser spring.datasource.password : {암호} FKSAJDFGYOS8F7GLHAKERGFHLSAJ```







이 일반 텍스트를 공유 git 저장소로 안전하게 푸시 할 수 있으며 비밀 암호가 보호됩니다.





서버는 또한 노출 `/encrypt`및 `/decrypt`엔드 포인트 를 공개합니다 (권한이 부여 된 에이전트 만 액세스 할 수 있다는 가정하에). 원격 구성 파일을 편집하는 경우 구성 서버를 사용하여 `/encrypt`엔드 포인트 에 게시하여 값을 암호화 할 수 있습니다 ( 예 :







```$ curl localhost : 8888 / encrypt -d mysecret 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda```







반대 연산은 via를 통해 사용할 수 있습니다 `/decrypt`(서버가 대칭 키 또는 전체 키 쌍으로 구성되어있는 경우).







```$ curl localhost : 8888 / decrypt -d 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda 나의 비밀```















팁

당신은 컬과 같이 테스트하는 경우, 사용 `--data-urlencode`(대신 `-d`명시 적)을 설정하거나 `Content-Type: text/plain`확인 컬 특수 문자가있는 경우 정확하게 데이터를 인코딩하기 위해 ( '+'는 특히 까다 롭다).|











암호화 된 값을 가져 와서 `{cipher}`접두어를 YAML 또는 특성 파일에 넣기 전에 그리고 커밋하고 원격의 잠재적으로 안전하지 않은 저장소로 밀어 넣기 전에 접두어를 추가하십시오 .





또한 엔드 포인트 `/encrypt`와 `/decrypt`엔드 포인트는 `/*/{name}/{profiles}`클라이언트가 기본 환경 자원을 호출 할 때 응용 프로그램 (이름) 및 프로파일마다 암호를 제어하는 ​​데 사용할 수 있는 양식 경로를 허용 합니다.













노트

이 세분화 된 방법으로 암호화를 제어하려면 이름과 프로필마다 다른 암호화 장치를 만드는 `@Bean`유형 도 제공해야합니다 `TextEncryptorLocator`. 기본적으로 제공되는 암호는이 작업을 수행하지 않으므로 모든 암호화가 동일한 키를 사용합니다.|











`spring`(설치 봄 구름 CLI 확장자) 명령 행 클라이언트는, 예를 암호화하고 해독하는 데 사용할 수 있습니다







```$ spring encrypt mysecret --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda $ spring decrypt --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda 나의 비밀```







파일 (예 : 암호화를위한 RSA 공개 키)에서 키를 사용하려면 키 값 앞에 "@"를 붙이고 파일 경로를 제공하십시오.







```$ spring encrypt mysecret --key @ $ {HOME} /. ssh / id_rsa.pub AQAjPgt3eFZQXwt8tsHAVv / QHiY5sI2dRcR + ...```







주요 인수는 필수 항목입니다 ( `--`접두사가 있음에도 불구하고 ).







### 키 관리



구성 서버는 대칭 (공유) 키 또는 비대칭 (RSA 키 쌍) 키를 사용할 수 있습니다. 비대칭 선택은 보안 측면에서 우수하지만 구성 할 단일 속성 값이기 때문에 대칭 키를 사용하는 것이 더 편리합니다.





대칭 키 `encrypt.key`를 구성하려면 비밀 문자열 로 설정 하거나 환경 변수 `ENCRYPT_KEY`를 사용하여 일반 텍스트 구성 파일에서 제외해야합니다.





비대칭 키를 구성하려면 키를 PEM으로 인코딩 된 텍스트 값 (in `encrypt.key`)으로 설정하거나 키 스토어 (예 : `keytool`JDK와 함께 제공 되는 유틸리티 로 작성)를 통해 설정할 수 있습니다 . 키 스토어의 프로퍼티은 다음 `encrypt.keyStore.*`과 `*`같습니다.





*   `location`( `Resource`위치),

*   `password` (키 스토어의 잠금을 해제하기 위해)

*   `alias` (상점의 어떤 키가 사용되는지 식별하기 위해).





암호화는 공개 키를 사용하여 수행되며 개인 키는 암호 해독에 필요합니다. 따라서 암호화를 원한다면 원칙적으로 서버의 공개 키 만 구성 할 수 있습니다 (개인 키로 로컬에서 값을 해독 할 준비가되어 있음). 실제로는 핵심 관리 프로세스가 서버에 집중되는 대신 모든 클라이언트를 중심으로 확산되므로이를 수행하고 싶지 않을 수 있습니다. 반면에 config 서버가 실제로 상대적으로 안전하지 않고 소수의 클라이언트 만 암호화 된 속성이 필요한 경우 유용한 옵션입니다.







### 테스트 용 키 저장소 만들기



테스트 용 키 저장소를 만들려면 다음과 같이하면됩니다.







```$ keytool -genkeypair -alias mytestkey -keyalg RSA \ -dname "CN = 웹 서버, OU = 단위, O = 조직, L = 도시, S = 상태, C = 미국" -keypass changeme -keystore server.jks -storepass letmein```







풋 `server.jks`(예를 들어) 클래스 경로에 파일을 한 다음에 `application.yml`는 config 서버 :







    encrypt:
      keyStore:
        location: classpath:/server.jks
        password: letmein
        alias: mytestkey
        secret: changeme









### 여러 키 및 키 회전 사용



`{cipher}`구성 서버는 암호화 된 등록 정보 값 의 접두어 이외에 `{name:value}`접두사 (0 또는 여러)를 (Base64로 인코딩 된) 암호 텍스트의 시작 전에 찾습니다 . 키는 a로 전달되어 cipher의 `TextEncryptorLocator`위치를 찾는 데 필요한 모든 논리를 수행 할 수 있습니다 `TextEncryptor`. 키 스토어 ( `encrypt.keystore.location`)를 설정 했다면 , 디폴트 로케이터는 "키"접두사에 의해 제공되는 것과 같은 별칭을 가진 저장소의 키를 찾는다.







    foo:
      bar: `{cipher}{key:testkey}...`







locator는 "testkey"라는 키를 찾을 것입니다. `{secret:…​}`접두사 의 값을 통해 비밀을 제공 할 수도 있지만 기본값이 아닌 경우 키 저장소 비밀번호를 사용하는 것입니다. 키 저장소를 만들 때 얻을 수있는 비밀 번호는 사용하지 않습니다. 당신이 경우에 **할** 비밀을 제공 당신은 또한 사용자 정의를 사용하여 비밀을 암호화하는 것이 좋습니다 `SecretLocator`.





키가 구성 데이터의 몇 바이트 만 암호화하는 데 사용되는 경우 (즉, 다른 곳에서 사용되지 않는 경우) 암호화 위반으로 키를 교체 할 필요는 거의 없지만 보안 위반이있는 경우 키를 변경해야 할 수도 있습니다. 예. 이 경우 모든 클라이언트는 소스 설정 파일 (예 : git)을 변경하고 `{key:…​}`모든 암호에서 새 접두어를 사용하여 미리 설정 서버 키 스토어에서 키 별칭을 사용할 수 있는지 확인해야합니다.













팁

구성 서버가 모든 암호화와 암호 해독을 처리하게 하려면 `{name:value}`접두어를 `/encrypt`엔드 포인트에 게시 된 일반 텍스트에 추가 할 수도 있습니다 .|













### 암호화 된 속성 제공



때로는 클라이언트가 서버에서 수행하는 대신 구성을 로컬에서 해독하기를 원할 수 있습니다. 이 경우 ( `encrypt.*` 키를 찾기 위해 구성을 제공하는 경우) 엔드 포인트를 / 암호화 및 / 암호 해독 할 수 있지만, 사용하여 나가는 등록 정보의 암호 해독 을 명시 적으로 해제해야합니다 `spring.cloud.config.server.encrypt.enabled=false`. 끝점을 신경 쓰지 않는다면 키 또는 활성화 된 플래그를 구성하지 않으면 작동합니다.











## 대체 형식 검색





환경 종점의 기본 JSON 형식은 추상화에 직접 매핑되기 때문에 Spring 응용 프로그램에서 사용하기에 `Environment`적합합니다. 원하는 경우 리소스 경로 ( ".yml", ".yaml"또는 ".properties")에 접미사를 추가하여 YAML 또는 Java 등록 정보와 동일한 데이터를 사용할 수 있습니다. 이는 JSON 끝점의 구조 나 그들이 제공하는 추가 메타 데이터를 신경 쓰지 않는 응용 프로그램에서 유용하게 사용할 수 있습니다. 예를 들어 Spring을 사용하지 않는 응용 프로그램은이 접근 방식의 단순함으로 이익을 얻을 수 있습니다.





YAML과 프라퍼티 표현은 `resolvePlaceholders`소스 문서의 자리 표시 자 (표준 Spring `${…​}`형식)가 렌더링 전에 가능한 출력에서 ​​확인되어야한다는 신호를 보내기 위해 추가 플래그 (부울 쿼리 매개 변수로 제공됨 ) 를가집니다. 이것은 Spring 개체 틀 규칙에 대해 잘 모르는 소비자에게 유용한 기능입니다.













노트

주로 메타 데이터의 손실과 관련하여 YAML 또는 속성 형식을 사용하는 데 제한이 있습니다. JSON은 속성 소스의 정렬 된 목록으로 구성됩니다 (예 : 소스와 상호 관련된 이름 포함). 값의 출처에 여러 원본이 있고 원래 원본 파일의 이름이 손실 된 경우에도 YAML 및 속성 양식은 단일 맵으로 병합됩니다. YAML 표현은 반드시 배킹 리포지토리의 YAML 소스를 충실하게 표현한 것은 아니며 플랫 속성 소스 목록으로 구성되며 키의 형식에 대한 가정을해야합니다.|















## 일반 텍스트 검색





`Environment`추상화 (또는 YAML 또는 속성 형식의 대체 표현 중 하나) 를 사용하는 대신 응용 프로그램에 환경에 맞게 일반 일반 텍스트 구성 파일이 필요할 수 있습니다. 구성 서버는 `/{name}/{profile}/{label}/{path}` "name", "profile"및 "label"이 일반 환경 엔드 포인트와 동일한 의미를 가지지 만 "path"는 파일 이름 (예 :) 인 추가 엔드 포인트를 통해이를 제공합니다 `log.xml`. 이 엔드 포인트의 소스 파일은 환경 엔드 포인트와 동일한 방식으로 위치합니다. 동일한 검색 경로가 특성 또는 YAML 파일에 사용되지만 일치하는 모든 자원을 모으는 대신 일치하는 첫 번째 파일 만 리턴됩니다.





리소스를 찾은 후 일반 형식 ( `${…​}`)의 자리 `Environment`표시자는 제공된 응용 프로그램 이름, 프로필 및 레이블에 대한 유효성 을 사용하여 확인 됩니다. 이 f}으로 자원 엔드 포인트는 환경 엔드 포인트와 긴밀하게 통합됩니다. 예를 들어, GIT (또는 SVN) 저장소에 대한 레이아웃이있는 경우 :







```application.yml nginx.conf```







위치는 `nginx.conf`다음과 같습니다 :







```서버 { 80을 듣는다. server_name $ {nginx.server.name}; }```







그리고 `application.yml`이렇게 :







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







```서버 { 80을 듣는다. server_name example.com; }```







그리고 `/foo/development/master/nginx.conf`이렇게 :







```서버 { 80을 듣는다. server_name develop.com; }```















노트

환경 설정을위한 소스 파일과 마찬가지로 "프로파일"을 사용하여 파일 이름을 분석하므로 프로파일 특정 파일을 원한다면 (선호하는 ) `/*/development/*/logback.xml`파일로 해석됩니다 . `logback-development.xml``logback.xml`|















## 구성 서버 포함





구성 서버는 독립 실행 형 응용 프로그램으로 가장 잘 실행되지만 필요한 경우 다른 응용 프로그램에 포함시킬 수 있습니다. `@EnableConfigServer`특수 효과 를 사용하면 됩니다. 이 경우에 유용 할 수있는 선택적 속성 `spring.cloud.config.server.bootstrap`은 서버가 자체 원격 저장소에서 자체를 구성해야 함을 나타내는 플래그입니다. 이 플래그는 시작을 지연시킬 수 있으므로 기본적으로 해제되어 있지만 다른 응용 프로그램에 포함 된 경우 다른 응용 프로그램과 같은 방법으로 초기화하는 것이 좋습니다.













노트

부트 스트랩 플래그를 사용하면 config 서버의 이름과 저장소 URI를 구성해야 `bootstrap.yml`합니다.|











서버 종점의 위치를 ​​변경하려면 `spring.cloud.config.server.prefix`"/ config"와 같이 설정할 수 있습니다 ( 예 : "/ config"). 접두사는 시작해야하지만 "/"로 끝나지 않아야합니다. 이것은 `@RequestMappings`구성 서버 (즉, Spring Boot 접두사 `server.servletPath`및 아래 `server.contextPath`)에 적용됩니다.





기본적으로 엔드 포인트가없는 임베디드 구성 서버 인 백엔드 저장소 (구성 서버가 아닌)에서 응용 프로그램의 구성을 직접 읽으려는 경우. 어노테이션을 사용하지 않는다면 `@EnableConfigServer` (단지 설정 `spring.cloud.config.server.bootstrap=true`됨) 엔드 포인트를 완전히 끌 수 있습니다 .









## 푸시 알림 및 스프링 클라우드 버스





많은 소스 코드 저장소 공급자 (예 : Github, Gitlab 또는 Bitbucket)는 웹 훅을 통해 저장소의 변경 사항을 알려줍니다. 제공자의 사용자 인터페이스를 통해 웹 훅을 URL 및 관심있는 이벤트 세트로 구성 할 수 있습니다. 예를 들어 [Github](https://developer.github.com/v3/activity/events/types/#pushevent) 은 커밋 목록이 들어있는 JSON 본문과 "push"와 같은 헤더 "X-Github-Event"를 사용하여 webhook에 POST합니다. `spring-cloud-config-monitor`라이브러리 에 종속성을 추가하고 구성 서버에서 Spring Cloud Bus를 활성화하면 "/ monitor"엔드 포인트가 사용 가능하게됩니다.





Webhook이 활성화되면 Config Server는 `RefreshRemoteApplicationEvent`변경된 것으로 생각되는 응용 프로그램을 대상으로 보냅니다 . 변경 감지는 전략적으로 수행 할 수 있지만 기본적으로 응용 프로그램 이름과 일치하는 파일의 변경 사항을 찾습니다 (예 : "foo.properties"는 "foo"응용 프로그램을 대상으로하고 "application.properties"는 모든 응용 프로그램을 대상으로 함) . 이 동작을 재정의하려는 경우 전략 `PropertyPathNotificationExtractor` 은 요청 헤더와 본문을 매개 변수로 받아들이고 변경된 파일 경로 목록을 반환하는 것입니다.





기본 구성은 Github, Gitlab 또는 Bitbucket과 함께 즉시 사용할 수 있습니다. Github, Gitlab 또는 Bitbucket의 JSON 알림 외에도 폼 인코딩 된 본문 매개 변수를 사용하여 "/ monitor"로 POST하여 변경 알림을 실행할 수 있습니다 `path={name}`. 이것은 "{name}"패턴 (와일드 카드를 포함 할 수 있음)과 일치하는 응용 프로그램으로 브로드 캐스팅됩니다.













노트

는 `RefreshRemoteApplicationEvent`가있는 경우에만 송신 될 것이다 `spring-cloud-bus`는 config 서버에 상기 클라이언트 어플리케이션이 활성화된다.|



















노트

기본 설정은 또한 로컬 자식 저장소에서 파일 시스템 변경을 감지합니다 (이 경우 webhook은 사용되지 않지만 설정 파일을 편집하자마자 새로 고침이 브로드 캐스트됩니다).|















## Spring Cloud 구성 클라이언트





Spring Boot 애플리케이션은 Spring Config Server (또는 애플리케이션 개발자가 제공 한 다른 외부 속성 소스)를 즉시 이용할 수 있으며 `Environment`변경 이벤트 와 관련된 몇 가지 유용한 기능을 추가로 제공 합니다.





### 첫 번째 부트 스트랩 구성



이는 클래스 경로에 Spring Cloud Config Client가있는 모든 애플리케이션의 기본 동작입니다. <font class="">설정 클라이언트가 시작되면 설정 서버에 (부트 스트랩 구성 등록 정보를 통해 `spring.cloud.config.uri`<font class="">) 바인드 `Environment`<font class="">하고 원격 등록 정보 소스로 <font class="">Spring <font class="">을 <font class="">초기화 <font class="">합니다.





이것의 최종 결과는 구성 서버를 사용하려는 모든 클라이언트 응용 프로그램이 `bootstrap.yml`서버 주소 가있는 (또는 `spring.cloud.config.uri`"http : // localhost : 8888") 기본값 (또는 환경 변수)이 필요하다는 것 입니다.







### 발견 첫 번째 부트 스트랩



Spring Cloud Netflix와 Eureka Service Discovery 또는 Spring Cloud Consul (Spring Cloud Zookeeper가 아직 이것을 지원하지 않음)과 같은 DiscoveryClient 구현을 사용하고 있다면 원하는 경우 Discovery Service에 등록 서버를 등록 할 수 있습니다. 그러나 기본 "구성 먼저"모드에서 클라이언트는 등록을 활용할 수 없습니다.





`DiscoveryClient`구성 서버의 위치를 ​​찾는 데 선호하는 경우 설정 `spring.cloud.config.discovery.enabled=true`(기본값 "false") 을 사용하여 구성 할 수 있습니다 . 결과적으로 클라이언트 응용 프로그램에는 모두 `bootstrap.yml`적절한 검색 구성이 필요한 환경 변수 가 필요합니다 . 예를 들어, Spring Cloud Netflix에서는 Eureka 서버 주소를 정의해야합니다 (예 :) `eureka.client.serviceUrl.defaultZone`. 이 옵션을 사용하는 가격은 서비스 등록을 찾기 위해 시작할 때 추가 네트워크 왕복입니다. 이점은 구성 서비스 서버가 고정 지점 인 경우 구성 서버가 해당 좌표를 변경할 수 있다는 것입니다. 기본 서비스 ID는 "configserver"이지만 클라이언트에서 `spring.cloud.config.discovery.serviceId`(및 설정에 의해 서비스와 같은 일반적인 방법으로 서버에서) 변경할 수 있습니다 `spring.application.name`.





검색 클라이언트 구현은 모든 종류의 메타 데이터 맵을 지원합니다 (예 : Eureka의 경우 `eureka.instance.metadataMap`). 클라이언트가 올바르게 연결할 수 있도록 구성 서버의 일부 추가 등록 정보를 서비스 등록 메타 데이터에 구성해야 할 수 있습니다. 구성 서버가 HTTP Basic으로 보안 설정되어 있으면 "사용자 이름"과 "암호"로 자격 증명을 구성 할 수 있습니다. 구성 서버에 컨텍스트 경로가있는 경우 "configPath"를 설정할 수 있습니다. 예를 들어, 유레카 클라이언트 인 구성 서버의 경우 :





bootstrap.yml



    eureka:
      instance:
        ...
        metadataMap:
          user: osufhalskjrtl
          password: lviuhlszvaorhvlo5847
          configPath: /config









### 구성 클라이언트 실패 빠른



경우에 따라 구성 서버에 연결할 수없는 경우 서비스 시작에 실패하는 것이 바람직 할 수 있습니다. 이것이 원하는 동작이면 bootstrap 구성 등록 정보 `spring.cloud.config.failFast=true`를 설정하면 클라이언트가 Exception으로 정지합니다.







### 구성 클라이언트 재시도



앱이 시작될 때 때때로 설정 서버를 사용할 수 없을 것으로 예상되면 오류가 발생한 후에도 계속 시도하도록 요청할 수 있습니다. 먼저 설정해야합니다 `spring.cloud.config.failFast=true`, 그리고 당신은 추가해야 `spring-retry`하고 `spring-boot-starter-aop`클래스 경로에. 기본 동작은 1000ms의 초기 백 오프 간격과 후속 백 오프의 지수 배율 1.1로 6 회 재 시도하는 것입니다. 구성 등록 정보를 사용하여 이러한 등록 정보 (및 기타 등록 정보)를 `spring.cloud.config.retry.*`구성 할 수 있습니다 .













팁

재 시도를 완전히 제어하려면 "configServerRetryInterceptor"id를 가진 `@Bean`유형 `RetryOperationsInterceptor`을 추가하십시오 . Spring Retry는 하나 `RetryInterceptorBuilder`를 쉽게 만들 수있게 해줍니다.|













### 원격 구성 리소스 찾기



구성 서비스는에서 속성 원본을 제공합니다 `/{name}/{profile}/{label}`. 여기서 클라이언트 응용 프로그램의 기본 바인딩은





*   "name"= `${spring.application.name}`

*   "프로필"= `${spring.profiles.active}`(실제로 `Environment.getActiveProfiles()`)

*   "label"= "master"





이들 모두는 설정 `spring.cloud.config.*` ( `*`"이름", "프로파일"또는 "레이블"은 어디에 ) 에 의해 무시 될 수 있습니다 . "레이블"은 이전 버전의 구성으로 롤백 할 때 유용합니다. 기본 구성 서버 구현에서는 git 레이블, 분기 이름 또는 커밋 ID가 될 수 있습니다. 레이블은 쉼표로 구분 된 목록으로 제공 될 수도 있습니다.이 경우 목록에있는 항목은 성공할 때까지 하나씩 시도됩니다. 이것은 기능 브랜치에서 작업 할 때 유용 할 수 있습니다. 예를 들어, 브랜치에 설정 라벨을 정렬하고 싶을 때 (예 :) 선택적으로 설정할 수 `spring.cloud.config.label=myfeature,develop`있습니다.







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





클라우드 파운드리에 앱을 배포하는 경우 암호를 제공하는 가장 좋은 방법은 서비스 자격 증명 (예 : URI)을 사용하는 것입니다. 이후로 구성 파일에있을 필요가 없기 때문입니다. "configserver"라는 Cloud Foundry에서 사용자가 제공하는 서비스와 로컬로 작동하는 예제 :





bootstrap.yml



    spring:
      cloud:
        config:
         uri: ${vcap.services.configserver.credentials.uri:http://user:password@localhost:8888}







다른 형태의 보안을 사용 `RestTemplate`하는 경우 `ConfigServicePropertySourceLocator`(예 : 부트 스트랩 컨텍스트에서이를 잡아서 주입하는 등)에를 제공해야 할 수도 있습니다 .









# 봄 구름 넷플 릭스



이 프로젝트는 자동 환경 설정과 스프링 환경 및 기타 스프링 프로그래밍 모델 관용구에 대한 바인딩을 통해 스프링 부트 애플리케이션을위한 Netflix OSS 통합을 제공합니다. 몇 가지 간단한 주석을 사용하면 애플리케이션 내부의 공통 패턴을 신속하게 활성화 및 구성하고 전투 테스트를 거친 Netflix 구성 요소로 대규모 분산 시스템을 구축 할 수 있습니다. 제공되는 패턴에는 서비스 발견 (Eureka), 회로 차단기 (Hystrix), 지능형 라우팅 (Zuul) 및 클라이언트 측로드 균형 조정 (리본)이 포함됩니다.





## 서비스 발견 : 유레카 클라이언트





서비스 검색은 마이크로 서비스 기반 아키텍처의 핵심 교리 중 하나입니다. 각 클라이언트 또는 일부 형식의 컨벤션을 손으로 구성하려는 것은 매우 어려울 수 있으며 매우 약해질 수 있습니다. 유레카는 Netflix 서비스 검색 서버 및 클라이언트입니다. 서버는 등록 된 서비스에 대한 상태를 다른 서버로 복제하여 각 서버가 고 가용성으로 구성 및 배치 될 수 있습니다.





### 유레카 등록



클라이언트가 유레카에 등록하면 호스트 및 포트, 상태 표시기 URL, 홈 페이지 등과 같은 메타 데이터를 제공합니다. 유레카는 서비스에 속한 각 인스턴스에서 하트 비트 메시지를 수신합니다. 하트 비트가 구성 가능한 시간표에 실패하면 인스턴스는 보통 레지스트리에서 제거됩니다.





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







(즉, 완전히 정상적인 스프링 부트 응용 프로그램). 이 예에서는 `@EnableEurekaClient`명시 적으로 사용 하지만 유레카 만 사용하면 사용할 수도 있습니다 `@EnableDiscoveryClient`. Eureka 서버를 찾으려면 구성이 필요합니다. 예:





application.yml



```유레카: 고객: serviceUrl : defaultZone : http : // localhost : 8761 / eureka /```







여기서 "defaultZone"은 기본 설정을 나타내지 않는 클라이언트 (즉 유용한 기본값)에 대한 서비스 URL을 제공하는 마법 문자열 대체 값입니다.





기본 프로그램 이름 (서비스 ID)는 가상 호스트와 비보안 포트는 상기에서 촬영 `Environment`하고, `${spring.application.name}`, `${spring.application.name}`및 `${server.port}`는 각각.





`@EnableEurekaClient`응용 프로그램을 유레카 "인스턴스"(예 : 자체 등록)와 "클라이언트"(즉, 다른 서비스를 찾기 위해 레지스트리에 쿼리 할 수 ​​있음)로 만듭니다. 인스턴스 동작은 구성 `eureka.instance.*`키로 인해 이루어 지지만 응용 프로그램에 a `spring.application.name`(유레카 서비스 ID 또는 VIP 의 기본값)가 있는지 확인하는 경우 기본값이 잘됩니다 .





구성 가능한 옵션에 대한 자세한 내용 은 [EurekaInstanceConfigBean](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-eureka-client/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java) 및 [EurekaClientConfigBean](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-eureka-client/src/main/java/org/springframework/cloud/netflix/eureka/EurekaClientConfigBean.java) 을 참조하십시오.







### 유레카 서버 인증



`eureka.client.serviceUrl.defaultZone`URL 중 하나에 자격 증명이 삽입 된 경우 (예 : 컬 스타일 `[http://user:password@localhost:8761/eureka](http://user:password@localhost:8761/eureka)`) HTTP 기본 인증이 자동으로 유레카 클라이언트에 추가됩니다 . 더 복잡한 요구를 들어, 당신은 만들 수 있습니다 `@Bean`유형의를 `DiscoveryClientOptionalArgs`하고 주입 `ClientFilter`모두는 클라이언트에서 서버로 호출에 적용됩니다, 그것으로 인스턴스.













노트

유레카의 한계로 인해 서버 당 기본 인증 자격 증명을 지원할 수 없으므로 발견 된 첫 번째 세트 만 사용됩니다.|













### 상태 페이지 및 상태 표시기



Eureka 인스턴스의 상태 페이지 및 상태 표시기는 각각 Spring Boot Actuator 응용 프로그램의 유용한 끝점의 기본 위치 인 "/ info"및 "/ health"로 기본 설정됩니다. 기본값이 아닌 컨텍스트 경로 나 서블릿 경로 (예 `server.servletPath=/foo`:) 또는 관리 끝점 경로 (예 :) 를 사용하는 경우 액추에이터 응용 프로그램의 경우에도 이러한 내용을 변경해야합니다 `management.contextPath=/admin`. 예:





application.yml



```유레카: 예: statusPageUrlPath : $ {management.context-path} / info healthCheckUrlPath : $ {management.context-path} / 건강```







이러한 링크는 클라이언트가 사용하는 메타 데이터에 표시되며 일부 시나리오에서는 응용 프로그램에 요청을 보낼지 여부를 결정하는 데 사용되므로 정확하면 유용합니다.







### 보안 응용 프로그램 등록



앱이 HTTPS를 통해 연락을 원하는 경우에 당신은 두 개의 플래그를 설정할 수 있습니다 `EurekaInstanceConfig`, _즉_ `eureka.instance.[nonSecurePortEnabled,securePortEnabled]=[false,true]` 각각. 이렇게하면 Eureka가 보안 통신에 대한 명시적인 선호를 보여주는 인스턴스 정보를 게시하게됩니다. 스프링 클라우드 `DiscoveryClient`는 `[https://…​](https://%E2%80%A6%E2%80%8B/);`이런 방식으로 구성된 서비스에 대한 URI를 항상 리턴 하고 유레카 (네이티브) 인스턴스 정보는 보안 상태 확인 URL을 갖게된다.





Eureka가 내부적으로 작동하는 방식 때문에 명시 적으로 덮어 쓰지 않는 한 상태 및 홈 페이지에 대해 보안되지 않은 URL을 게시합니다. 자리 표시자를 사용하여 eureka 인스턴스 URL을 구성 할 수 있습니다 (예 :





application.yml



```유레카: 예: statusPageUrl : https : // $ {eureka.hostname} / info healthCheckUrl : https : // $ {eureka.hostname} / 건강 homePageUrl : https : // $ {eureka.hostname} /```







( `${eureka.hostname}`유레카의 최신 버전에서만 사용 가능한 네이티브 자리 표시 자입니다. 예를 들어, 스프링 자리 표시자를 사용하여 동일한 결과를 얻을 수 `${eureka.instance.hostName}`있습니다.)













노트

앱이 프록시 뒤에 있고 SSL 종료가 프록시에있는 경우 (예 : Cloud Foundry 또는 다른 플랫폼에서 서비스로 실행하는 경우) 프록시 "전달 된"헤더가 가로 채어지고 처리되는지 확인해야합니다. 응용 프로그램. 'X-Forwarded - \ *'헤더를 명시 적으로 설정하면 Spring Boot 애플리케이션의 임베디드 Tomcat 컨테이너가 자동으로이 기능을 수행한다. 틀린 표시는 앱이 자체적으로 렌더링 한 링크가 잘못된 호스트 (잘못된 호스트, 포트 또는 프로토콜)가 될 것입니다.|













### 유레카 건강 검사



기본적으로 Eureka는 클라이언트 하트 비트를 사용하여 클라이언트가 작동 중인지 확인합니다. 별도로 명시하지 않는 한 Discovery Client는 Spring Boot Actuator 당 응용 프로그램의 현재 상태 확인 상태를 전파하지 않습니다. 즉, 성공적으로 등록한 후에 유레카는 응용 프로그램이 항상 'UP'상태임을 발표합니다. 이 동작은 유레카 상태 검사를 사용하도록 설정하여 응용 프로그램 상태를 유레카로 전파함으로써 변경 될 수 있습니다. 결과적으로 다른 모든 응용 프로그램은 'UP'이외의 상태에서 응용 프로그램에 트래픽을 보내지 않습니다.





application.yml



```유레카: 고객: 건강 체크: enabled : true```







건강 검진에 대한 더 많은 통제가 필요하다면, 자신의 건강 검진을 시행 할 것을 고려할 수 있습니다 `com.netflix.appinfo.HealthCheckHandler`.







### 인스턴스 및 클라이언트에 대한 유레카 메타 데이터



It’s worth spending a bit of time understanding how the Eureka metadata works, so you can use it in a way that makes sense in your platform. There is standard metadata for things like hostname, IP address, port numbers, status page and health check. These are published in the service registry and used by clients to contact the services in a straightforward way. Additional metadata can be added to the instance registration in the `eureka.instance.metadataMap`, and this will be accessible in the remote clients, but in general will not change the behaviour of the client, unless it is made aware of the meaning of the metadata. There are a couple of special cases described below where Spring Cloud already assigns meaning to the metadata map.





#### Using Eureka on Cloudfoundry


Cloudfoundry has a global router so that all instances of the same app have the same hostname (it’s the same in other PaaS solutions with a similar architecture). This isn’t necessarily a barrier to using Eureka, but if you use the router (recommended, or even mandatory depending on the way your platform was set up), you need to explicitly set the hostname and port numbers (secure or non-secure) so that they use the router. You might also want to use instance metadata so you can distinguish between the instances on the client (e.g. in a custom load balancer). By default, the `eureka.instance.instanceId` is `vcap.application.instance_id`. For example:





application.yml

    eureka:
      instance:
        hostname: ${vcap.application.uris[0]}
        nonSecurePort: 80


Cloudfoundry 인스턴스에서 보안 규칙을 설정하는 방법에 따라 직접 서비스 간 호출에 호스트 VM의 IP 주소를 등록하고 사용할 수 있습니다. 이 기능은 Pivotal Web Services ( [PWS](https://run.pivotal.io/) ) 에서 아직 사용할 수 없습니다 .



#### AWS에서 Eureka 사용



응용 프로그램이 AWS 클라우드에 배포되도록 계획된 경우 Eureka 인스턴스는 Amazon을 인식하도록 구성되어야하며 다음과 같은 방식으로 [EurekaInstanceConfigBean](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-eureka-client/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java) 을 사용자 정의하여 수행 할 수 있습니다 .







    @Bean
    @Profile("!default")
    public EurekaInstanceConfigBean eurekaInstanceConfig() {
      EurekaInstanceConfigBean b = new EurekaInstanceConfigBean();
      AmazonInfo info = AmazonInfo.Builder.newBuilder().autoBuild("eureka");
      b.setDataCenterInfo(info);
      return b;
    }









#### 유레카 인스턴스 ID 변경



바닐라 넷플 릭스 유레카 인스턴스는 호스트 이름과 동일한 ID로 등록됩니다 (예 : 호스트 당 하나의 서비스 만). Spring Cloud Eureka는 다음과 같은 현명한 기본값을 제공합니다 `${spring.cloud.client.hostname}:${spring.application.name}:${spring.application.instance_id:${server.port}}}`. 예를 들면 `myhost:myappname:8080`.





Spring Cloud를 사용하면에서 고유 한 식별자를 제공함으로써 이것을 덮어 쓸 수있다 `eureka.instance.instanceId`. 예 :





application.yml



```유레카: 예: instanceId : $ {spring.application.name} : $ {spring.application.instance_id : $ {random.value}}```







이 메타 데이터와 localhost에 배포 된 여러 서비스 인스턴스를 사용하면 무작위 값이 인스턴스를 고유하게 만듭니다. Cloudfoundry에서는 `spring.application.instance_id`Spring Boot Actuator 응용 프로그램에 자동으로 채워 지므로 무작위 값은 필요하지 않습니다.









### EurekaClient 사용



[유레카 서버](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-eureka-server) 에서 서비스 인스턴스를 발견하는 데 사용할 수 있는 앱이 있으면 `@EnableDiscoveryClient`(또는 `@EnableEurekaClient`) 사용할 수 있습니다 . 이를 수행하는 한 가지 방법은 네이티브를 사용하는 것입니다 ( 예 : Spring Cloud와 반대 ).[](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-eureka-server)`com.netflix.discovery.EurekaClient``DiscoveryClient`







```@Autowired 개인 EurekaClient discoveryClient;
 public String serviceUrl () { InstanceInfo 인스턴스 = discoveryClient.getNextServerFromEureka ( "저장", 거짓); return instance.getHomePageUrl (); }```















팁





`EurekaClient`in `@PostConstruct`메소드 또는 `@Scheduled`메소드 (또는 `ApplicationContext`아직 시작되지 않았을 수있는 모든 위치)를 사용하지 마십시오 . 그것은 `SmartLifecycle`(with `phase=0`) 로 초기화되어 가장 초기에 당신이 사용할 수있는 것이 `SmartLifecycle`더 높은 단계의 다른 것에 존재할 수 있습니다 .

















### 기본 Netflix EurekaClient의 대안



원시 Netflix를 사용할 필요가 없으며 `EurekaClient`일반적으로 일종의 래퍼 뒤에 사용하는 것이 더 편리합니다. Spring Cloud는 물리적 URL 대신 논리적 Eureka 서비스 식별자 (VIP)를 사용하여 [Feign](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign) (REST 클라이언트 빌더) 및 [Spring`RestTemplate`](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon) 을 지원합니다. 물리적 서버의 고정 목록으로 리본을 구성하려면 `<client>.ribbon.listOfServers`쉼표로 구분 된 실제 주소 (또는 호스트 이름) 목록을 설정 `<client>`하면됩니다. 여기서는 클라이언트의 ID입니다.





또한 `org.springframework.cloud.client.discovery.DiscoveryClient` Netflix와 관련이없는 검색 클라이언트를위한 간단한 API를 제공하는을 사용할 수도 있습니다.







```@Autowired 개인용 DiscoveryClient discoveryClient;
 public String serviceUrl () { List <ServiceInstance> list = discoveryClient.getInstances ( "STORES"); if (list! = null && list.size ()> 0) { return list.get (0) .getUri (); } null를 돌려 준다. }```









### 서비스 등록이 너무 느린 이유는 무엇입니까?



인스턴스가되는 것은 또한 `serviceUrl`기본 지속 시간이 30 초인 (클라이언트를 통해) 레지스트리에주기적인 하트 비트를 포함합니다 . 인스턴스, 서버 및 클라이언트가 모두 로컬 캐시에 동일한 메타 데이터를 가지고 있기 때문에 (3 개의 하트 비트가 필요할 수 있음) 클라이언트가 서비스를 검색 할 수 없습니다. 이를 사용하여 기간을 변경할 수 `eureka.instance.leaseRenewalIntervalInSeconds`있으며 이로 인해 클라이언트가 다른 서비스에 연결되는 프로세스가 빨라집니다. 프로덕션 환경에서는 임대 갱신 기간에 대한 가정을 서버에서 내부적으로 계산하기 때문에 기본값을 사용하는 것이 좋습니다.











## 서비스 발견 : 유레카 서버





유레카 서버의 예 (예 : spring-cloud-starter-eureka-server를 사용하여 클래스 경로 설정)







    @SpringBootApplication
    @EnableEurekaServer
    public class Application {

        public static void main(String[] args) {
            new SpringApplicationBuilder(Application.class).web(true).run(args);
        }

    }







서버에는 UI가있는 홈 페이지와 일반적인 Eureka 기능 당 HTTP API 끝 점이 `/eureka/*`있습니다.





유레카 배경 읽기 : [플럭스 커패시터](https://github.com/cfregly/fluxcapacitor/wiki/NetflixOSS-FAQ#eureka-service-discovery-load-balancer) 및 [Google 그룹 토론을](https://groups.google.com/forum/?fromgroups#!topic/eureka_netflix/g3p2r7gHnN0) 참조하십시오 .













팁





Gradle의 의존성 해결 규칙과 부모 bom 기능의 부족으로 인해 spring-cloud-starter-eureka-server에 의존하기 만하면 응용 프로그램 시작시 오류가 발생할 수 있습니다. 이 문제를 해결하려면 Spring Boot Gradle 플러그인을 추가해야하며 Spring 클라우드 스타터 상위 BOM을 다음과 같이 가져와야합니다.





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



Eureka 서버에는 백엔드 저장소가 없지만 레지스트리의 서비스 인스턴스는 등록을 최신 상태로 유지하기 위해 하트 비트를 보내야합니다 (메모리에서이 작업을 수행 할 수 있습니다). 또한 클라이언트는 메모리에 유레카 등록 캐시를 가지고 있기 때문에 (서비스에 대한 모든 단일 요청에 대해 레지스트리에 갈 필요가 없습니다).





기본적으로 모든 유레카 서버는 유레카 클라이언트이기도하며 피어를 찾기 위해 (적어도 하나의) 서비스 URL이 필요합니다. 제공하지 않으면 서비스가 실행되고 작동하지만 피어와 함께 등록 할 수 없다는 것에 대한 많은 소음이 로그에 기록됩니다.





영역 및 영역에 대한 클라이언트 측 [의 리본 지원](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon) 에 [대한 자세한](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon) 내용은 [아래를 참조하십시오](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon) .







### 독립 실행 형 모드



두 개의 캐시 (클라이언트 및 서버)와 하트 비트의 결합으로 독립 실행 형 유레카 서버가 모니터 또는 탄력적 인 런타임 (예 : Cloud Foundry)을 유지하는 한 실패에 상당히 탄력적입니다. 독립 실행 형 모드에서는 클라이언트 측 동작을 중단하여 동료에게 도달하지 못하고 계속 시도하지 않는 것을 선호 할 수 있습니다. 예:





application.yml (독립 실행 형 유레카 서버)



```섬기는 사람: 포트 : 8761
 유레카: 예: 호스트 이름 : localhost 고객: registerWithEureka : false fetchRegistry : 거짓 serviceUrl : defaultZone : http : // $ {eureka.instance.hostname} : $ {server.port} / eureka /```







(가) 알 `serviceUrl`로컬 인스턴스와 동일한 호스트를 가리키고 있습니다.







### 또래 인식



유레카는 여러 인스턴스를 실행하고 서로 등록하도록 요청함으로써 훨씬 더 탄력적으로 사용할 수 있습니다. 사실 이것은 기본 동작이므로 `serviceUrl`피어 에 유효한 값 을 추가하는 것만으로도 작동하게 만들면됩니다.





application.yml (두 개의 피어 인식 유레카 서버)



```--- 봄: 프로필 : peer1 유레카: 예: 호스트 이름 : peer1 고객: serviceUrl : defaultZone : http : // peer2 / eureka /
 --- 봄: 프로필 : peer2 유레카: 예: 호스트 이름 : peer2 고객: serviceUrl : defaultZone : http : // peer1 / eureka /```







이 예제에서는 두 개의 호스트 (peer1 및 peer2)에서 동일한 서버를 실행하고 다른 Spring 프로파일에서 실행함으로써 YAML 파일을 사용할 수 있습니다. 이 구성을 사용하여 단일 호스트에 대한 피어 인식을 테스트 할 수 있습니다 (프로덕션 환경에서 수행 할 때 그다지 가치가 없음) `/etc/hosts`. 호스트 이름을 해결하기 위해 조작 합니다. 사실, `eureka.instance.hostname`자신의 호스트 이름을 알고있는 머신에서 실행중인 경우에는이 옵션이 필요하지 않습니다 ( `java.net.InetAddress`기본적으로 사용 됩니다).





시스템에 여러 피어를 추가 할 수 있으며 서로가 모두 직접 연결되어있는 한 서로간에 피어를 등록 할 수 있습니다.





application.yml (세 개의 피어 인식 유레카 서버)



```유레카: 고객: serviceUrl : defaultZone : http : // peer1 / eureka /, http : // peer2 / eureka /, http : // peer3 / eureka /
 --- 봄: 프로필 : peer1 유레카: 예: 호스트 이름 : peer1
 --- 봄: 프로필 : peer2 유레카: 예: 호스트 이름 : peer2
 --- 봄: 프로필 : peer3 유레카: 예: 호스트 이름 : peer3```









### IP 주소 선호



어떤 경우에는 유레카가 호스트 이름이 아닌 서비스의 IP 주소를 광고하는 것이 바람직합니다. 집합 `eureka.instance.preferIpAddress` 을 `true`응용 프로그램 유레카에 등록 할 때, 호스트 이름 대신 IP 주소를 사용한다.











## 회로 차단기 : Hystrix 클라이언트





Netflix는 [회로 차단기 패턴](http://martinfowler.com/bliki/CircuitBreaker.html) 을 구현하는 [Hystrix](https://github.com/Netflix/Hystrix) 라는 라이브러리를 만들었습니다 . 마이크로 서비스 아키텍처에서는 서비스 호출의 다중 레이어를 갖는 것이 일반적입니다.[](http://martinfowler.com/bliki/CircuitBreaker.html)





![HystrixGraph](./spring-cloud-doc-resources/HystrixGraph.png)

그림 1\. 마이크로 서비스 그래프





서비스 수준이 낮 으면 서비스가 실패 할 수 있으므로 계단식 오류가 발생할 수 있습니다. 특정 서비스에 대한 통화가 특정 임계 값에 도달하면 (Hystrix에서는 기본값 인 5 초 동안 20 개의 실패가 발생 함) 회선이 열리고 통화가 이루어지지 않습니다. 오류 및 개방 회로의 경우 폴백은 개발자가 제공 할 수 있습니다.





![HystrixFallback](./spring-cloud-doc-resources/HystrixFallback.png)

그림 2\. Hystrix 폴백으로 계단식 오류 방지





개방 회로가 있으면 계단식 오류가 발생하지 않으므로 압도되거나 실패한 서비스를 치료할 수 있습니다. 폴백은 또 다른 Hystrix 보호 호출, 정적 데이터 또는 빈 값입니다. 폴백은 체인으로 연결되어 첫 번째 폴백이 다른 비즈니스 호출을 만들어 정적 데이터로 다시 폴백 할 수 있습니다.





부팅 앱의 예 :







```@SpringBootApplication @EnableCircuitBreaker public class Application {
 공공 정적 무효 메인 (문자열 [] args) { 새로운 SpringApplicationBuilder (Application.class) .web (true) .run (args); }
 }
 @구성 요소 공용 클래스 StoreIntegration {
 @HystrixCommand (fallbackMethod = "defaultStores") 공용 객체 getStores (Map <String, Object> 매개 변수) { // 실패 할 수있는 일을하십시오. }
 공용 객체 defaultStores (Map <String, Object> 매개 변수) { return / * 유용한 정보 * /; } }```







이 파일 `@HystrixCommand`은 ["javanica"](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica) 라는 Netflix contrib 라이브러리에서 제공 합니다. 스프링 클라우드는 Hystrix 회로 차단기에 연결된 프록시에서 해당 주석이있는 스프링 빈을 자동으로 래핑합니다. 회로 차단기는 회로를 열거 나 닫을시기와 고장이 발생할 경우 수행 할 작업을 계산합니다.





이를 구성하려면 어노테이션 목록과 함께 속성을 `@HystrixCommand`사용할 수 있습니다 . 자세한 내용은 [여기](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica#configuration) 를 참조하십시오. 사용 가능한 속성에 대한 자세한 내용은 [Hystrix 위키](https://github.com/Netflix/Hystrix/wiki/Configuration) 를 참조하십시오.`commandProperties``@HystrixProperty`[](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica#configuration)[](https://github.com/Netflix/Hystrix/wiki/Configuration)





### 보안 컨텍스트 전파 또는 스프링 스코프 사용



일부 스레드 로컬 컨텍스트를 `@HystrixCommand`기본 선언에 전파하려면 스레드 풀에서 명령을 실행하기 때문에 (시간 초과의 경우) 기본 선언이 작동하지 않습니다. 일부 구성을 사용하여 발신자와 동일한 스레드를 사용하거나 주석에서 다른 "격리 전략"을 사용하도록 요청하여 Hystrix를 전환 할 수 있습니다. 예 :







    @HystrixCommand(fallbackMethod = "stubMyService",
        commandProperties = {
          @HystrixProperty(name="execution.isolation.strategy", value="SEMAPHORE")
        }
    )
    ...







`@SessionScope`또는 을 사용하는 경우에도 마찬가지입니다 `@RequestScope`. 범위가 지정된 컨텍스트를 찾을 수 없다는 런타임 예외로 인해이를 수행해야 할 때를 알 수 있습니다.







### 건강 지표



연결된 회로 차단기의 상태 `/health`는 호출 응용 프로그램 의 끝점 에서도 노출됩니다 .







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



Hystrix 메트릭 스트림을 사용하려면에 종속성을 포함시킵니다 `spring-boot-starter-actuator`. 이렇게하면 `/hystrix.stream`관리 엔드 포인트로 표시됩니다.







        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-actuator</artifactId>
        </dependency>













## 회로 차단기 : Hystrix 대시 보드





Hystrix의 주요 이점 중 하나는 각 HystrixCommand에 대해 수집 한 일련의 메트릭입니다. Hystrix Dashboard는 각 회로 차단기의 상태를 효율적으로 표시합니다.





![Hystrix](./spring-cloud-doc-resources/Hystrix.png)

그림 3\. Hystrix 대시 보드





Hystrix 대시 보드를 실행하려면 Spring Boot 메인 클래스에 주석을 달아 라 `@EnableHystrixDashboard`. 그런 다음 `/hystrix`대시 보드를 방문 `/hystrix.stream`하여 Hystrix 클라이언트 애플리케이션 의 개별 인스턴스 엔드 포인트로 지정합니다.





### 터빈



개별 인스턴스를 보면 Hystrix 데이터는 시스템의 전반적인 상태와 관련하여별로 유용하지 않습니다. [터빈](https://github.com/Netflix/Turbine) 은 Hystrix 대시 보드에서 사용하기 위해 모든 관련 `/hystrix.stream`엔드 포인트를 결합한 `/turbine.stream`어플리케이션입니다. 개별 인스턴스는 Eureka를 통해 위치합니다. Running Turbine은 메인 클래스에 주석을 달아주는 것처럼 간단합니다 `@EnableTurbine`(예 : 스프링 - 클라우드 - 스타터 - 터빈을 사용하여 클래스 경로 설정). [터빈 1 위키의](https://github.com/Netflix/Turbine/wiki/Configuration-(1.x)) 모든 문서화 된 구성 속성이 적용됩니다. 유일한 차이점은 `turbine.instanceUrlSuffix`port가 prepended 할 필요가 없다는 것 `turbine.instanceInsertPort=false`입니다.





구성 키 `turbine.appConfig`는 터빈이 인스턴스를 검색하는 데 사용할 eureka serviceIds 목록입니다. 터빈 스트림은 다음과 같은 URL을 사용하여 Hystrix 대시 보드에서 사용됩니다. `[http://my.turbine.sever:8080/turbine.stream?cluster=<CLUSTERNAME>](http://my.turbine.sever:8080/turbine.stream?cluster=%3CCLUSTERNAME%3E);`(클러스터 매개 변수는 이름이 "default"인 경우 생략 할 수 있습니다). `cluster`매개 변수의 항목과 일치해야합니다 `turbine.aggregator.clusterConfig`. eureka에서 반환 된 값은 대문자이므로 Eureka에 등록 된 앱이 "고객"이라면이 예제가 작동 할 것으로 기대합니다.







```터빈: 어 그리 게이터 : clusterConfig : 고객 appConfig : 고객```







은 `clusterName`에 SPEL 표현하여 사용자 정의 할 수 있습니다 `turbine.clusterNameExpression`루트의 인스턴스 `InstanceInfo`. 기본값 `appName`은 Eureka serviceId가 클러스터 키로 끝나는 것을 의미합니다 (즉 `InstanceInfo`고객에게 `appName`"고객"이 있음). 다른 예가 `turbine.clusterNameExpression=aSGName`AWS ASG 이름에서 클러스터 이름을 가져옵니다. 다른 예 :







```터빈: 어 그리 게이터 : clusterConfig : SYSTEM, USER appConfig : 고객, 상점, UI, 관리자 clusterNameExpression : 메타 데이터 [ 'cluster']```







이 경우 네 가지 서비스의 클러스터 이름은 메타 데이터 맵에서 가져오고 "SYSTEM"및 "USER"가 포함 된 값이 있어야합니다.





모든 응용 프로그램에 대해 "기본"클러스터를 사용하려면 문자열 리터럴식이 필요합니다 (작은 따옴표로 묶고 YAML에있는 경우 큰 따옴표로 이스케이프 처리).







```터빈: appConfig : 고객, 상점 clusterNameExpression : " ''기본값 '"```







Spring Cloud는 `spring-cloud-starter-turbine`터빈 서버를 실행하는 데 필요한 모든 종속성을 가진 것을 제공합니다 . 그냥 봄 부팅 응용 프로그램을 만들고 주석을 달아주세요 `@EnableTurbine`.













노트

기본적으로 Turbine에 내장 된 기본 Netflix 동작 은 클러스터 당 호스트 당 여러 프로세스를 허용 하지 _않습니다_ (인스턴스 ID의 키는 호스트 이름 임). Spring Cloud는 이것을 약간 일반화하여 호스트와 포트를 키로 사용할 수있게하지만 속성을 설정 한 경우에만 가능합니다.`turbine.combineHostPort=true`|













### 터빈 스트림



In some environments (e.g. in a PaaS setting), the classic Turbine model of pulling metrics from all the distributed Hystrix commands doesn’t work. In that case you might want to have your Hystrix commands push metrics to Turbine, and Spring Cloud enables that with messaging. All you need to do on the client is add a dependency to `spring-cloud-netflix-hystrix-stream` and the `spring-cloud-starter-stream-*` of your choice (see Spring Cloud Stream documentation for details on the brokers, and how to configure the client credentials, but it should work out of the box for a local broker).





On the server side Just create a Spring Boot application and annotate it with `@EnableTurbineStream` and by default it will come up on port 8989 (point your Hystrix dashboard to that port, any path). You can customize the port using either `server.port` or `turbine.stream.port`. If you have `spring-boot-starter-web` and `spring-boot-starter-actuator` on the classpath as well, then you can open up the Actuator endpoints on a separate port (with Tomcat by default) by providing a `management.port` which is different.





You can then point the Hystrix Dashboard to the Turbine Stream Server instead of individual Hystrix streams. If Turbine Stream is running on port 8989 on myhost, then put `[http://myhost:8989](http://myhost:8989/)` in the stream input field in the Hystrix Dashboard. Circuits will be prefixed by their respective serviceId, followed by a dot, then the circuit name.





Spring Cloud는 `spring-cloud-starter-turbine-stream`Turbine Stream 서버를 실행하는 데 필요한 모든 의존성을 제공하는 것을 제공합니다 `spring-cloud-starter-stream-rabbit`. 예를 들어, 원하는 Stream 바인더 만 추가하면 됩니다. Netty 기반이기 때문에 Java 8이 필요합니다.











## 클라이언트 측로드 밸런서 : 리본





리본은 HTTP 및 TCP 클라이언트의 동작을 제어 할 수있는 클라이언트 측로드 밸런서입니다. Feign은 이미 리본을 사용하므로이 `@FeignClient`섹션 을 사용하는 경우에도이 섹션이 적용됩니다.





리본의 중심 개념은 명명 된 클라이언트의 개념입니다. 각로드 밸런서는 필요에 따라 원격 서버에 연결하기 위해 함께 작동하는 구성 요소 앙상블의 일부이며 앙상블은 애플리케이션 개발자 (예 : `@FeignClient` 주석 사용)로 지정한 이름을가집니다. Spring Cloud는 `ApplicationContext`각 명명 된 클라이언트를 사용하여 필요할 때마다 새로운 앙상블을 생성합니다 `RibbonClientConfiguration`. 여기에는 an `ILoadBalancer`, a `RestClient`및 a가 포함 `ServerListFilter`됩니다.





### 리본 클라이언트 사용자 정의



외부 속성을 사용하여 리본 클라이언트의 일부 비트를 구성 할 수 있습니다 `<client>.ribbon.*`. Netflix API를 기본적으로 사용하는 것 외에는 Spring 부트 구성 파일을 사용할 수 있다는 점만 다릅니다. 기본 옵션은 `CommonClientConfigKey`(리본 코어의 일부인) 정적 필드로 검사 할 수 있습니다 .





봄 구름은 또한 당신 (의 위에 추가 구성을 선언하여 클라이언트의 모든 권한 걸릴 수 있습니다 `RibbonClientConfiguration`사용) `@RibbonClient`. 예:







    @Configuration
    @RibbonClient(name = "foo", configuration = FooConfiguration.class)
    public class TestConfiguration {
    }







이 경우 클라이언트는 `RibbonClientConfiguration`모든 in과 함께 이미있는 구성 요소로 구성 됩니다 `FooConfiguration` (일반적으로 후자가 이전을 대체합니다).













경고

이 `FooConfiguration`있어야한다 `@Configuration`하지만이 아닌 관리 걸릴 `@ComponentScan`그렇지 않으면 모두에 의해 공유됩니다, 기본 응용 프로그램 컨텍스트를 `@RibbonClients`. `@ComponentScan`(또는 `@SpringBootApplication`) 을 사용하는 경우 포함되지 않도록 조치를 취해야합니다 (예 : 별도의 중복되지 않는 패키지에 넣거나 명시 적으로 스캔 할 패키지를 지정하는 경우 `@ComponentScan`).|











Spring Cloud Netflix는 기본적으로 리본 ( `BeanType`beanName :)에 대해 다음과 같은 빈을 제공합니다 `ClassName`.





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



유레카는 리본 상기와 함께 사용하는 경우 `ribbonServerList` 의 확장으로 오버라이드 (override) `DiscoveryEnabledNIWSServerList` 유레카에서 서버 목록을 채 웁니다있다. 또한 대체 `IPing`와 인터페이스 `NIWSDiscoveryPing`서버가있는 경우 유레카 명 규모가 결정되는합니다. `ServerList`기본적으로 설치되는이 인 `DomainExtractingServerList`이의 목적은 (넷플 릭스에 의존하는 것입니다) AWS AMI 메타 데이터를 사용하지 않고 부하 분산 장치에 대한 물리적 메타 데이터를 사용할 수 있도록하는 것입니다. 기본적으로 서버 목록은 인스턴스 메타 데이터에 제공된대로 "영역"정보로 구성되며 (원격 클라이언트 집합에서 제공됨 `eureka.instance.metadataMap.zone`) 서버가없는 경우 영역의 프록시로 서버 호스트 이름의 도메인 이름을 사용할 수 있습니다 (if 플래그 `approximateZoneFromHostname`가 설정됩니다). 영역 정보를 사용할 수있게되면 a `ServerListFilter`. 에서 사용할 수 있습니다 . `ZonePreferenceServerListFilter`기본적으로 클라이언트는 클라이언트와 동일한 영역에 서버를 배치하는 데 사용됩니다 . 클라이언트 영역은 기본적으로 원격 인스턴스와 동일한 방식으로 결정됩니다 (예 : via) `eureka.instance.metadataMap.zone`.













노트

클라이언트 영역을 설정하는 "archaius"방식은 "@zone"이라는 구성 속성을 통해 이루어지며, Spring Cloud는 사용 가능한 경우 다른 모든 설정보다 우선적으로 사용합니다 (키는 YAML에서 인용해야합니다 구성).|



















노트

영역 데이터의 다른 소스가없는 경우 클라이언트 구성 (인스턴스 구성과 반대 됨)을 기반으로 추측이 이루어집니다. 우리는 걸릴 `eureka.client.availabilityZones`영역 목록에 지역 이름에서지도를하다, 그리고 인스턴스의 자신의 지역의 제 1 영역을 당겨 (즉 `eureka.client.region`, 이는 기본적으로 "우리 동쪽-1"기본 넷플릭스와 comatibility)입니다.|













### 예 : 유레카가없는 리본 사용법



Eureka는 원격 서버의 발견을 추상화하는 편리한 방법이므로 클라이언트에 URL을 하드 코딩 할 필요가 없지만 사용하지 않으려는 경우에도 Ribbon 및 Feign은 여전히 ​​사용하기 쉽습니다. `@RibbonClient`"상점" 을 선언했다고 가정 하고, 유레카는 사용 중이 지 않습니다 (그리고 클래스 패스조차도 아닙니다). 리본 클라이언트는 기본적으로 구성된 서버 목록으로 구성되며 다음과 같은 구성을 제공 할 수 있습니다





application.yml



```백화점: 리본: listOfServers : example.com, google.com```









### 예 : 리본에서 유레카 사용을 비활성화합니다.



속성 `ribbon.eureka.enabled = false`을 설정하면 명시 적으로 리본에서 유레카의 사용을 비활성화합니다.





application.yml



```리본: 유레카: enabled : false```









### 리본 API를 직접 사용



`LoadBalancerClient`직접 사용할 수도 있습니다. 예:







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





[Feign](https://github.com/Netflix/feign) 은 선언적 웹 서비스 클라이언트입니다. 따라서 웹 서비스 클라이언트를 쉽게 작성할 수 있습니다. Feign을 사용하려면 인터페이스를 만들고 주석을 달아 라. Feign 주석과 JAX-RS 주석을 포함하여 플러그 가능 주석 주석 지원을 제공합니다. Feign은 또한 플러그 형 인코더와 디코더를 지원합니다. Spring Cloud는 Spring MVC 주석을 지원 `HttpMessageConverters`하고 Spring Web에서 기본적으로 사용되는 주석을 사용한다 . Spring Cloud는 Ribbon과 Eureka를 통합하여 Feign을 사용할 때로드 밸런싱 된 HTTP 클라이언트를 제공합니다.





봄 부팅 응용 프로그램의 예







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







에서 `@FeignClient`주석 문자열 값 ( "저장"위)는 리본로드 밸런서 (참조 만드는 데 사용되는 임의의 클라이언트 이름입니다 [리본 지원 자세한 내용은 아래를](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon) ). `url`속성 (절대 값 또는 호스트 이름)을 사용하여 URL을 지정할 수도 있습니다 . 응용 프로그램 컨텍스트에서 Bean의 이름은 인터페이스의 완전한 이름입니다. 'name'속성과 'FeignClient'가 추가 된 별칭도 생성됩니다. 위의 예제 `@Qualifier("storesFeignClient")`에서 bean을 참조하는 데 사용될 수 있습니다.





위의 리본 클라이언트는 "상점"서비스의 실제 주소를 검색하려고합니다. 응용 프로그램이 유레카 클라이언트 인 경우 유레카 서비스 레지스트리의 서비스가 해결됩니다. 유레카 (Eureka)를 사용하지 않으려는 경우 외부 구성에서 서버 목록을 구성하기 만하면됩니다 ( [위의 예](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon-without-eureka) 참조).





### 기본 기본값 재정의



Spring Cloud의 Feign 지원의 핵심 개념은 명명 된 클라이언트의 개념입니다. 각 클라이언트는 필요에 따라 원격 서버에 연결하기 위해 함께 작동하는 구성 요소의 앙상블의 일부이며, 앙상블에는 주석을 사용하여 `@FeignClient`응용 프로그램 개발자로 제공하는 이름이 있습니다 . Spring Cloud는 `ApplicationContext`각 명명 된 클라이언트를 사용하여 필요할 때마다 새로운 앙상블을 생성합니다 `FeignClientsConfiguration`. 여기에는 an `feign.Decoder`, a `feign.Encoder`및 a가 포함 `feign.Contract`됩니다.





봄 클라우드는 (의 위에 추가 구성 선언함으로써 꾀병 클라이언트의 전체 제어 할 수 있습니다 `FeignClientsConfiguration`) 사용하여 `@FeignClient`. 예:







    @FeignClient(name = "stores", configuration = FooConfiguration.class)
    public interface StoreClient {
        //..
    }







이 경우 클라이언트는 이미 in `FeignClientsConfiguration`과 함께있는 구성 요소로 구성 됩니다 `FooConfiguration`(후자는 이전을 대체합니다).













경고

이 `FooConfiguration`있어야한다 `@Configuration`하지만이 아닌 관리 걸릴 `@ComponentScan`그렇지 않으면 모든 사용됩니다, 기본 응용 프로그램 컨텍스트를 `@FeignClient`. `@ComponentScan`(또는 `@SpringBootApplication`) 을 사용하는 경우 포함되지 않도록 조치를 취해야합니다 (예 : 별도의 중복되지 않는 패키지에 넣거나 명시 적으로 스캔 할 패키지를 지정하는 경우 `@ComponentScan`).|



















노트

`serviceId`속성은 이제 찬성되지 않습니다 `name`속성.|



















경고

이전에는 속성을 사용하여 `url`속성을 요구하지 않았습니다 `name`. 사용 `name`은 이제 필요합니다.|











자리 표시자는 `name`및에서 `url`지원됩니다.







    @FeignClient(name = "${feign.name}", url = "${feign.url}")
    public interface StoreClient {
        //..
    }







Spring Cloud Netflix는 기본적으로 feign ( `BeanType`beanName :)에 대해 다음 bean을 제공합니다 `ClassName`.





*   `Decoder`feignDecoder : `ResponseEntityDecoder`(a를 감싸는 `SpringDecoder`)

*   `Encoder` feignEncoder : `SpringEncoder`

*   `Logger` feignLogger : `Slf4jLogger`

*   `Contract` feignContract : `SpringMvcContract`

*   `Feign.Builder` feignBuilder : `HystrixFeign.Builder`





Spring Cloud Netflix _는_ 기본적으로 feign에 대해 다음과 같은 bean을 제공 _하지 않지만_ , 어플리케이션 컨텍스트에서 이러한 유형의 bean을 검색하여 feign 클라이언트를 작성합니다.





*   `Logger.Level`

*   `Retryer`

*   `ErrorDecoder`

*   `Request.Options`

*   `Collection<RequestInterceptor>`





그 유형 중 하나의 콩 만들기 및에 배치 `@FeignClient`구성하면 (예 : `FooConfiguration`위)가 설명 된 콩의 각각을 대체 할 수 있습니다. 예:







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







이것은 `SpringMvcContract`with `feign.Contract.Default`를 대체하고 `RequestInterceptor`Collection을에 추가합니다 `RequestInterceptor`.





기본 구성이 지정 될 수있는 `@EnableFeignClients`특성을 `defaultConfiguration`상술 한 바와 같이 유사한 방식. 차이점은이 구성이 _모든_ 클라이언트에 적용된다는 것 입니다.







### Hystrix 지원 지원



Hystrix가 classpath 상에 있다면, 기본적으로 Feign은 모든 메소드를 회로 차단기로 감쌀 것이다. 돌아 오는 `com.netflix.hystrix.HystrixCommand`것도 가능합니다. 이를 통해 반응 패턴을 사용할 수 있습니다 ( `.toObservable()`또는 `.observe()`에 대한 호출과 함께 또는 비동기 사용 `.queue()`).





Feyst에 대한 Hystrix 지원을 사용하지 않으려면 설정 `feign.hystrix.enabled=false`하십시오.





클라이언트별로 Hystrix 지원을 비활성화하려면 `Feign.Builder`"프로토 타입"범위 의 바닐라 를 만드십시오 . 예 :







    @Configuration
    public class FooConfiguration {
        @Bean
        @Scope("prototype")
        public Feign.Builder feignBuilder() {
            return Feign.builder();
        }
    }









### Hystrix Fallbacks를 기쁘게합니다.



Hystrix는 회로가 열려 있거나 오류가있을 때 실행되는 기본 코드 경로 인 폴백의 개념을 지원합니다. 주어진 `@FeignClient`세트에 `fallback`대해 대체를 사용하려면 대체를 구현하는 클래스 이름에 속성을 설정합니다.







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















경고

Feign의 대체 기능 구현과 Hystrix 대체 기능의 작동 방식에는 제한이 있습니다. fallback은 현재 `com.netflix.hystrix.HystrixCommand`와 를 반환하는 메소드에서 지원되지 않습니다 `rx.Observable`.|













### 기꺼이 상속 지원



Feign은 단일 상속 인터페이스를 통해 상용구 API를 지원합니다. 이를 통해 공통 작업을 편리한 기본 인터페이스로 그룹화 할 수 있습니다.





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

일반적으로 서버와 클라이언트간에 인터페이스를 공유하는 것은 바람직하지 않습니다. 이것은 tight coupling을 소개하고 실제로는 현재의 형태로 Spring MVC에서 작동하지 않습니다 (메소드 매개 변수 매핑은 상속되지 않습니다).|













### 희망 요청 / 응답 압축



귀하는 귀하의 Feign 요청에 대해 요청 또는 응답 GZIP 압축을 활성화하는 것을 고려할 수 있습니다. 다음 중 하나의 속성을 활성화하여이 작업을 수행 할 수 있습니다.







    feign.compression.request.enabled=true
    feign.compression.response.enabled=true







긴급 요청 압축을 사용하면 웹 서버에 설정할 수있는 것과 비슷한 설정을 사용할 수 있습니다.







    feign.compression.request.enabled=true
    feign.compression.request.mime-types=text/xml,application/xml,application/json
    feign.compression.request.min-request-size=2048







이 등록 정보를 사용하면 압축 된 미디어 유형과 최소 요청 임계 값 길이에 대한 선택을 할 수 있습니다.







### 벌채 로깅



작성된 각 Feign 클라이언트에 대해 로거가 작성됩니다. 기본적으로 로거 이름은 Feign 클라이언트를 만드는 데 사용 된 인터페이스의 전체 클래스 이름입니다. 깃발 기록은 `DEBUG`레벨 에만 응답합니다 .





application.yml



    logging.level.project.user.UserClient: DEBUG







`Logger.Level`클라이언트별로 구성 할 수 있는 객체는 Feign에게 얼마나 많은 양을 기록할지 알려줍니다. 선택 사항은 다음과 같습니다.





*   `NONE`, No logging ( **DEFAULT** ).

*   `BASIC`, 요청 방법과 URL 및 응답 상태 코드와 실행 시간 만 로깅합니다.

*   `HEADERS`, 요청 및 응답 헤더와 함께 기본 정보를 기록하십시오.

*   `FULL`, 요청과 응답에 대한 헤더, 본문 및 메타 데이터를 기록합니다.





예를 들어, 다음은 `Logger.Level`to를 `FULL`다음과 같이 설정합니다 .







    @Configuration
    public class FooConfiguration {
        @Bean
        Logger.Level feignLoggerLevel() {
            return Logger.Level.FULL;
        }
    }













## 외부 구성 : Archaius





[Archaius](https://github.com/Netflix/archaius) 는 Netflix 클라이언트 측 구성 라이브러리입니다. 모든 Netflix OSS 구성 요소가 구성에 사용하는 라이브러리입니다. Archaius는 [Apache Commons Configuration](https://commons.apache.org/proper/commons-configuration) 프로젝트의 [확장판](https://commons.apache.org/proper/commons-configuration) 입니다. 소스를 폴링하여 변경 사항을 보거나 소스가 변경 사항을 클라이언트에 푸시하여 구성을 갱신 할 수 있습니다. Archaius는 동적 <Type> 속성 클래스를 속성의 핸들로 사용합니다.





아키아우스 예



    class ArchaiusTest {
        DynamicStringProperty myprop = DynamicPropertyFactory
                .getInstance()
                .getStringProperty("my.prop");

        void doSomething() {
            OtherClass.someMethod(myprop.get());
        }
    }







Archaius는 고유의 구성 파일 세트 및로드 우선 순위를 가지고 있습니다. 스프링 애플리케이션은 일반적으로 Archaius를 직접 사용하지 않아야하지만 넷플 릭스 도구를 기본적으로 구성 할 필요가 있습니다. Spring Cloud는 Spring Environment Bridge를 가지고있어서 Archaius는 Spring Environment로부터 속성을 읽을 수 있습니다. 이를 통해 스프링 부트 프로젝트는 일반적인 구성 툴 체인을 사용하면서 문서화 된대로 Netflix 도구를 구성 할 수 있습니다.









## 라우터 및 필터 : Zuul





마이크로 서비스 아키텍처의 핵심 부분에서 라우팅. 예를 들어 `/`웹 응용 프로그램 `/api/users`에 매핑되고 사용자 서비스 `/api/shop`에 매핑되며 쇼핑 서비스에 매핑 될 수 있습니다. [Zuul](https://github.com/Netflix/zuul) 은 Netflix의 JVM 기반 라우터 및 서버 측로드 밸런서입니다.





[Netflix는 Zuul](http://www.slideshare.net/MikeyCohen1/edge-architecture-ieee-international-conference-on-cloud-engineering-32240146/27) 을 [사용하여 다음과 같은 작업](http://www.slideshare.net/MikeyCohen1/edge-architecture-ieee-international-conference-on-cloud-engineering-32240146/27) 을 수행합니다.





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

구성 속성은 `zuul.max.host.connections`두 가지 새로운 속성으로 대체되었습니다 `zuul.host.maxTotalConnections`및 `zuul.host.maxPerRouteConnections`각각 200과 20에있는 기본.|











### 임베디드 Zuul 역방향 프록시



Spring Cloud는 UI 애플리케이션이 하나 이상의 백엔드 서비스에 대한 호출을 프록시하고자하는 매우 일반적인 사용 사례의 개발을 용이하게하기 위해 임베디드 Zuul 프록시를 만들었습니다. 이 기능은 필요한 모든 백엔드에 대해 CORS 및 인증 문제를 독립적으로 관리 할 필요가 없도록 사용자 인터페이스가 필요한 백엔드 서비스로 프록시하는 데 유용합니다.





이를 가능하게하려면 Spring Boot 메인 클래스에 주석을 달아 `@EnableZuulProxy`라. 그러면 이것은 로컬 호출을 적절한 서비스에 전달한다. 규약에 따라 ID가 "users"인 서비스는 `/users`(앞에 접두사가 붙은) 위치에있는 프록시로부터 요청을받습니다 . 프록시는 발견을 통해 전달할 인스턴스를 찾기 위해 리본을 사용하고 모든 요청은 hystrix 명령으로 실행되므로 Hystrix 메트릭에 실패가 표시되고 일단 회로가 열리면 프록시는 서비스에 접속하려고 시도하지 않습니다.













노트

Zuul 스타터에는 검색 클라이언트가 포함되어 있지 않으므로 서비스 ID를 기반으로하는 경로의 경우 클래스 패스에있는 경로 중 하나를 제공해야합니다 (예 : Eureka는 하나의 선택 사항입니다).|











서비스가 자동으로 추가되는 것을 건너 뛰려면 `zuul.ignored-services`서비스 ID 패턴 목록을 설정 하십시오. 서비스가 무시되고 명시 적으로 구성된 라우트 맵에 포함 된 패턴과 일치하면 무시되지 않습니다. 예:





application.yml



     zuul:
      ignoredServices: '*'
      routes:
        users: /myusers/**







이 예에서는 "users"를 **제외한** 모든 서비스가 무시됩니다 .





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







이것은 "/ myusers"에 대한 http 호출이 "users_service"서비스로 전달됨을 의미합니다. 경로는 개미 스타일 패턴으로 지정할 수있는 "경로"를 가져야하므로 "/ myusers / *"는 한 레벨에만 일치하지만 "/ myusers / **"는 계층 적으로 일치합니다.





백엔드의 위치는 "serviceId"(발견 된 서비스의 경우) 또는 "url"(물리적 위치의 경우)으로 지정할 수 있습니다.





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          url: http://example.com/users_service







이러한 간단한 URL 경로는 URL로 실행 `HystrixCommand`되지 않으며 여러 URL을 리본으로로드 밸런싱 할 수도 없습니다. 이를 위해 service-route를 지정하고 serviceId에 대한 리본 클라이언트를 구성하십시오 (현재 리본에서 Eureka 지원을 비활성화해야합니다. 자세한 내용은 [위](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-ribbon-without-eureka) 참조 ).





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







regexmapper를 사용하여 serviceId와 route 사이에 규칙을 제공 할 수 있습니다. 그룹이라는 정규 표현식을 사용하여 serviceId에서 변수를 추출하여 경로 패턴에 주입합니다.





ApplicationConfiguration.java



    @Bean
    public PatternServiceRouteMapper serviceRouteMapper() {
        return new PatternServiceRouteMapper(
            "(?<name>^.+)-(?<version>v.+$)",
            "${version}/${name}");
    }







즉, serviceId "myusers-v1"은 "/ v1 / myusers / **"경로에 매핑됩니다. 모든 정규식이 허용되지만 모든 명명 된 그룹은 servicePattern과 routePattern에 모두 있어야합니다. servicePattern이 serviceId와 일치하지 않으면 기본 비헤이비어가 사용됩니다. 위의 예에서 serviceId "myusers"는 "/ myusers / **"경로에 매핑됩니다 (버전이 없음).이 기능은 기본적으로 비활성화되어 있으며 발견 된 서비스에만 적용됩니다.





모든 매핑에 접두어를 추가하려면와 `zuul.prefix`같은 값으로 설정 `/api`하십시오. 프록시 접두사는 요청이 기본적으로 전달되기 전에 요청에서 제거됩니다 (이 동작을 해제 `zuul.stripPrefix=false`). 개별 경로에서 서비스 별 접두어를 제거 할 수도 있습니다 (예 :





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          stripPrefix: false







이 예에서 "/ myusers / 101"에 대한 요청은 "users"서비스의 "/ myusers / 101"로 전달됩니다.





`zuul.routes`항목은 실제로 유형의 개체에 바인딩 `ZuulProperties`. 해당 객체의 속성을 보면 "재시도 가능"플래그가 있음을 알 수 있습니다. 해당 플래그를 "true"로 설정하면 리본 클라이언트가 실패한 요청을 자동으로 다시 시도합니다 (리본 클라이언트 구성을 사용하여 재시도 작업의 매개 변수를 수정할 수 있어야하는 경우).





`X-Forwarded-Host`헤더는 기본적으로 전달 요청에 추가됩니다. 그것을 끄려면 설정 `zuul.addProxyHeaders = false`하십시오. 접두어 경로는 기본적으로 제거되고 백엔드에 대한 요청은 헤더 "X-Forwarded-Prefix"(위의 예에서 "/ myusers")를 선택합니다.





응용 프로그램 `@EnableZuulProxy`은 기본 경로 ( "/")를 설정하면 독립 실행 형 서버로 작동 할 수 있습니다. 예를 들어 `zuul.route.home: /`모든 트래픽 (예 : "/ **")을 "홈"서비스로 라우팅합니다.





보다 세분화 된 무시가 필요할 경우 무시할 특정 패턴을 지정할 수 있습니다. 이러한 패턴은 라우트 위치 지정 프로세스의 시작에서 평가됩니다. 즉, 일치를 보장하기 위해 접두어가 패턴에 포함되어야 함을 의미합니다. 무시 된 패턴은 모든 서비스에 적용되며 다른 경로 사양보다 우선합니다.





application.yml



     zuul:
      ignoredPatterns: /**/admin/**
      routes:
        users: /myusers/**







즉, "/ myusers / 101"과 같은 모든 호출은 "users"서비스에서 "/ 101"로 전달됩니다. 그러나 "/ admin /"을 포함한 전화는 해결되지 않습니다.







### 쿠키 및 민감한 헤더



동일한 시스템에서 서비스간에 헤더를 공유해도 괜찮지 만, 민감한 헤더가 외부 서버로 다운 스트림으로 유출되는 것을 원하지 않을 것입니다. 무시 된 헤더 목록을 라우트 구성의 일부로 지정할 수 있습니다. 쿠키는 브라우저에서 잘 정의 된 의미 체계를 가지고 있기 때문에 특별한 역할을하며 항상 민감한 것으로 취급됩니다. 프록시 사용자가 브라우저 인 경우 다운 스트림 서비스에 대한 쿠키도 모두 혼란 스럽기 때문에 문제가됩니다 (다운 스트림 서비스는 모두 같은 장소에서 온 것처럼 보입니다).





예를 들어 다운 스트림 서비스 중 하나에서만 쿠키를 설정하는 경우와 같이 서비스 설계에주의를 기울이면 백엔드에서 발신자까지 모든 흐름을 전달할 수 있습니다. 또한 프록시가 쿠키를 설정하고 모든 백엔드 서비스가 동일한 시스템의 일부인 경우 간단하게 공유하는 것이 자연 스럽습니다 (예를 들어 Spring 세션을 사용하여 일부 공유 상태로 연결). 그 이외에 다운 스트림 서비스에 의해 설정된 쿠키는 호출자에게별로 유용하지 않을 수 있으므로 "Set-Cookie"및 "Cookie"를 중요한 헤더에 사용하는 것이 좋습니다. 도메인의 일부가 아닙니다. 심지어 경로에 대한 **있습니다** 도메인의 일부,





민감한 헤더는 경로별로 쉼표로 구분 된 목록으로 구성 할 수 있습니다 (예 :





application.yml



     zuul:
      routes:
        users:
          path: /myusers/**
          sensitiveHeaders: Cookie,Set-Cookie,Authorization
          url: https://downstream







민감한 헤더는 설정을 통해 전체적으로 설정할 수도 있습니다 `zuul.sensitiveHeaders`. 경우 `sensitiveHeaders`경로에 설정이 글로벌 우선합니다 `sensitiveHeaders`설정.













노트

이 값은 기본 값 `sensitiveHeaders`이므로 다른 값을 원한다면 설정하지 않아도됩니다. NB 이것은 Spring Cloud Netflix 1.1에서 새로 추가되었습니다 (1.0에서는 사용자가 헤더를 제어 할 수없고 모든 쿠키가 양방향으로 흐른다).|











경로 별 구분 헤더 `zuul.ignoredHeaders`외에도 다운 스트림 서비스와의 상호 작용 중에 폐기해야하는 값 (요청 및 응답 모두) 에 대한 전역 값을 설정할 수 있습니다 . Spring 보안이 클래스 패스에 없다면, 디폴트 값은 비어 있습니다. 그렇지 않으면 Spring Security에 지정된대로 잘 알려진 "보안"헤더 세트 (예 : 캐싱 포함)로 초기화됩니다. 이 경우의 가정은 다운 스트림 서비스가이 헤더를 추가 할 수도 있고 프록시의 값을 원한다는 것입니다.







### 경로 종점



`@EnableZuulProxy`스프링 부트 액츄에이터와 함께 사용 하는 경우 HTTP를 통해 추가 엔드 포인트를 사용할 수있게됩니다 (기본적으로) `/routes`. 이 엔드 포인트에 대한 GET은 맵핑 된 라우트 목록을 리턴합니다. POST는 기존 경로를 강제로 새로 고칩니다 (예 : 서비스 카탈로그가 변경된 경우).













노트

경로는 서비스 카탈로그의 변경 사항에 자동으로 응답해야하지만 / routes에 대한 POST는 변경 사항을 즉시 적용하도록하는 방법입니다.|













### 교살 패턴과 로컬 전달



기존 애플리케이션이나 API를 마이그레이션 할 때 일반적인 패턴은 이전 엔드 포인트를 "교살하여 다른 구현으로 천천히 대체하는 것"입니다. Zuul 프록시는 이전 엔드 포인트의 클라이언트로부터의 모든 트래픽을 처리하는 데 사용할 수 있기 때문에이 기능에 유용한 도구이지만 일부 요청은 새로운 엔드 포인트로 리디렉션합니다.





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







이 예에서는 다른 패턴 중 하나와 일치하지 않는 모든 요청에 ​​매핑되는 '기존'앱을 차단하고 있습니다. 에있는 경로 `/first/**`가 외부 URL이있는 새 서비스로 추출되었습니다. 그리고 경로 `/second/**`는 forware되기 때문에 정상적인 Spring과 같이 로컬에서 처리 할 수 ​​있습니다 `@RequestMapping`. `/third/**`또한 경로 는 전달되지만 다른 접두어 `/third/foo`로 전달됩니다 (예 : 전달됨 `/3rd/foo`).













노트

무시 된 패턴은 완전히 무시되지 않고 프록시에 의해 처리되지 않습니다 (따라서 효과적으로 로컬로 전달됩니다).|













### Zuul을 통한 파일 업로드



당신이 경우 `@EnableZuulProxy`당신은 파일을 업로드 할 프록시 경로를 사용할 수 있습니다 그리고 그것은 단지 한 파일이 작으로 작동합니다. 대용량 파일의 경우 `DispatcherServlet`"/ zuul / *"에서 Spring을 우회하는 다른 경로가 있습니다 (다중 처리를 피하기 위해). 즉, `zuul.routes.customers=/customers/**`큰 파일을 "/ zuul / customers / *"에 POST 할 수 있습니다. 서블릿 경로는를 통해 외부화됩니다 `zuul.servletPath`. 대용량 파일은 프록시 경로가 리본로드 밸런서를 통해 이동하는 경우 시간 초과 설정을 높여야합니다 (예 :





application.yml



    hystrix.command.default.execution.isolation.thread.timeoutInMilliseconds: 60000
    ribbon:
      ConnectTimeout: 3000
      ReadTimeout: 60000







스트리밍을 대용량 파일로 작업하려면 요청에서 청크 분할 인코딩을 사용해야합니다 (일부 브라우저에서는 기본적으로 수행하지 않음). 예 : 명령 줄에서 :







```$ curl -v -H "전송 인코딩 : 청크 분할"\ -F "file=@mylarge.iso"localhost : 9999 / zuul / simple / file```









### 일반 내장 Zuul



프록시를 사용하지 않고 Zuul 서버를 실행할 수도 있고 `@EnableZuulServer`(대신 `@EnableZuulProxy`) 프록시 서버의 일부를 선택적으로 사용할 수도 있습니다 . 만약 유형의 애플리케이션에 추가하는 콩 `ZuulFilter` 들이 함께 한, 자동적으로 설치된다 `@EnableZuulProxy`하지만 않고 프록시 필터 중 하나가 자동으로 추가된다.





이 경우 Zuul 서버에 대한 경로는 "zuul.routes. *"를 구성하여 계속 지정되지만 서비스 발견 및 프록시가 없으므로 "serviceId"및 "url"설정은 무시됩니다. 예 :





application.yml



     zuul:
      routes:
        api: /api/**







"/ api / **"의 모든 경로를 Zuul 필터 체인에 매핑합니다.







### 주울 필터 사용 안 함



Spring Cloud 용 Zuul은 `ZuulFilter`기본적으로 프록시 모드와 서버 모드에서 사용할 수있는 많은 Bean을 제공 합니다. 사용 가능한 필터에 [대해서는 zuul 필터 패키지](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/zuul/filters) 를 참조하십시오 . 사용하지 않으려면 간단히 설정 `zuul.<SimpleClassName>.<filterType>.disable=true`하십시오. 규칙에 따라, 패키지 `filters`는 Zuul 필터 유형입니다. 예를 들어 `org.springframework.cloud.netflix.zuul.filters.post.SendResponseFilter`설정 을 사용 중지 합니다 `zuul.SendResponseFilter.post.disable=true`.







### 사이드카로 다국어 지원



Eureka, Ribbon 및 Config Server를 활용하고자하는 jvm이 아닌 언어를 사용합니까? Spring Cloud Netflix Sidecar는 [Netflix Prana](https://github.com/Netflix/Prana) 에서 영감을 얻었 습니다. 여기에는 특정 서비스에 대한 모든 인스턴스 (예 : 호스트 및 포트)를 가져 오는 간단한 http API가 포함되어 있습니다. Eureka에서 경로 항목을 가져온 Zuul 프록시를 통해 서비스 호출을 프록시 처리 할 수도 있습니다. Spring Cloud Config Server는 호스트 조회를 통해 또는 Zuul 프록시를 통해 직접 액세스 할 수 있습니다. 비 jvm 앱은 헬스 체크를 구현하여 사이드카가 앱이 위 또는 아래로 움직일 때 사이드카가 유레카에게 신고 할 수 있도록해야합니다.





사이드카를 사용하려면 Spring Boot 응용 프로그램을 `@EnableSidecar`만듭니다. 이 주석은 포함 `@EnableCircuitBreaker`, `@EnableDiscoveryClient`하고 `@EnableZuulProxy`. 비 -JVM 응용 프로그램과 동일한 호스트에서 결과 응용 프로그램을 실행하십시오.





측면 차 추가 구성하려면 다음 `sidecar.port`과 `sidecar.health-uri`에를 `application.yml`. 이 `sidecar.port`속성은 비 jvm 응용 프로그램이 수신 대기하는 포트입니다. 이것은 사이드카가 앱을 유레카에 제대로 등록 할 수있게 해줍니다. The `sidecar.health-uri` 는 스프링 부트 (Spring Boot) 상태 표시기를 흉내내는 non-jvm 앱에서 액세스 할 수있는 uri입니다. 다음과 같은 json 문서를 반환해야합니다.





건강 - 우리 - 문서



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







`DiscoveryClient.getInstances()`메서드에 대한 API 가 `/hosts/{serviceId}`있습니다. 다음은 `/hosts/customers`다른 호스트에 두 개의 인스턴스를 반환 하는 예제 응답입니다 . 이 api는 비 jvm 앱 (사이드카가 포트 5678에있는 경우)에서 액세스 할 수 `[http://localhost:5678/hosts/{serviceId}](http://localhost:5678/hosts/%7BserviceId%7D)`있습니다.





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







Zuul 프록시는 eureka에 알려진 각 서비스에 대한 경로를 자동으로 추가 `/<serviceId>`하므로 고객 서비스는에서 사용할 수 `/customers`있습니다. 비 jvm 앱은 `[http://localhost:5678/customers](http://localhost:5678/customers)` (사이드카가 포트 5678에서 수신 중이라고 가정 할 때 )를 통해 고객 서비스에 액세스 할 수 있습니다 .





구성 서버가 Eureka에 등록 된 경우 비 jvm 응용 프로그램은 Zuul 프록시를 통해 액세스 할 수 있습니다. ConfigServer의 serviceId가 `configserver` 있고 사이드카가 포트 5678에 있으면 [http : // localhost : 5678 / configserver](http://localhost:5678/configserver) 에서 액세스 할 수 있습니다[](http://localhost:5678/configserver)





비 jvm 앱은 YAML 문서를 반환하는 구성 서버의 기능을 이용할 수 있습니다. 예를 들어 [http://sidecar.local.spring.io:5678/configserver/default-master.yml을](http://sidecar.local.spring.io:5678/configserver/default-master.yml) 호출하면 [다음](http://sidecar.local.spring.io:5678/configserver/default-master.yml) 과 같은 YAML 문서가 생성 될 수 있습니다.







    eureka:
      client:
        serviceUrl:
          defaultZone: http://localhost:8761/eureka/
      password: password
    info:
      description: Spring Cloud Samples
      url: https://github.com/spring-cloud-samples













## 스프링 MVC가있는 RxJava





Spring Cloud Netflix에는 [RxJava가](https://github.com/ReactiveX/RxJava) 포함되어 있습니다.





>
>
> RxJava는 [Reactive Extensions](http://reactivex.io/) 의 Java VM 구현입니다 . 관찰 가능한 순서를 사용하여 비동기 및 이벤트 기반 프로그램을 작성하기위한 라이브러리입니다.
>
>





Spring Cloud Netflix는 `rx.Single`Spring MVC 컨트롤러에서 객체 를 반환 할 수 있도록 지원 합니다. 또한 [SSE (Server-sent events)](https://en.wikipedia.org/wiki/Server-sent_events)`rx.Observable` 에 대한 객체 사용도 지원합니다 . 내부 API가 이미 RxJava를 사용하여 작성된 경우 매우 유용 할 수 있습니다 ( 예제는 [Hystrix 지원](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-hystrix) 페이지 [참조](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-hystrix) ).[](https://en.wikipedia.org/wiki/Server-sent_events)[](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-feign-hystrix)





다음은 몇 가지 사용 예입니다 `rx.Single`.







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







당신이있는 경우 `Observable`, 오히려 하나보다, 당신이 사용할 수있는 `.toSingle()`나 `.toList().toSingle()`. 여기 몇 가지 예가 있어요.







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







스트리밍 엔드 포인트와 클라이언트가있는 경우 SSE가 옵션 일 수 있습니다. `rx.Observable`Spring `SseEmitter`용도 로 변환 하기 `RxResponse.sse()`. 여기 몇 가지 예가 있어요.







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
        return RxResponse.sse(APPLICATION_JSON_UTF8, Observable.just(
                new EventDto("Spring io", getDate(2016, 5, 19)),
                new EventDto("SpringOnePlatform", getDate(2016, 8, 1))
        ));
    }











## 통계 : Spectator, Servo 및 Atlas





Spectator / Servo와 Atlas를 함께 사용하면 거의 실시간 운영 통찰력을 얻을 수 있습니다.





Spectator 및 Servo는 Netflix의 메트릭 컬렉션 라이브러리입니다. Atlas는 차원 시계열 데이터를 관리하기위한 Netflix 메트릭 백엔드입니다.





Servo는 Netflix를 수년간 사용했으며 여전히 사용할 수 있지만 점차적으로 Java 8에서만 작동하도록 설계된 Spectator를 단계적으로 단계적으로 제거하고 있습니다. Spring Cloud Netflix는 둘 다 지원하지만 Java 8 기반 응용 프로그램은 Spectator .





### 차원 대 계층 적 메트릭 비교



스프링 부트 액츄에이터 메트릭은 계층 적이며 메트릭은 이름으로 만 구분됩니다. 이러한 이름은 종종 마침표로 구분 된 이름에 키 / 값 속성 쌍 (차원)을 포함하는 명명 규칙을 따릅니다. root와 star-star라는 두 개의 끝점에 대해 다음과 같은 측정 항목을 고려하십시오.







    {
        "counter.status.200.root": 20,
        "counter.status.400.root": 3,
        "counter.status.200.star-star": 5,
    }







첫 번째 메트릭은 단위 시간당 루트 엔드 포인트에 대한 정상적인 요청 성공 횟수를 제공합니다. 그러나 시스템에 20 개의 엔드 포인트가 있고 모든 엔드 포인트에 대한 성공적인 요청 수가 필요한 경우에는 어떻게해야합니까? 일부 계층 적 메트릭 백엔드를 사용하면 **20 개의 모든 메트릭을 읽고 결과를 집계하는** 것과 같은 와일드 카드를 지정할 **수 있습니다. ****또는 ****엔드 포인트와 상관없이 모든 성공적인 요청 ****과 같은 메트릭을 가로 채고 기록 ****할 수 ****있지만 이제는 20 + 1 개의 다른 메트릭을 작성해야합니다. ****마찬가지로 서비스의 모든 엔드 포인트에 대한 성공한 요청의 총 수를 알고 싶으면 와일드 카드를 지정할 수 있습니다** .`counter.status.200.`**`HandlerInterceptorAdapter``counter.status.200.all``counter.status.2`**`.*`





계층 적 메트릭 백엔드에서 와일드 카드 지원이 있더라도 명명 일관성은 어려울 수 있습니다. 특히 이름 문자열에서 이러한 태그의 위치는 시간이지나면서 질의를 위반할 수 있습니다. 예를 들어 위의 계층 적 메트릭에 HTTP 메서드에 대해 추가 차원을 추가한다고 가정합니다. 그런 다음 `counter.status.200.root`이된다 없습니다 `counter.status.200.method.get.root`등 우리는 `counter.status.200.*`갑자기 더 이상 같은 의미 론적 의미를 가지고있다. 또한 새로운 차원이 코드베이스 전체에 균일하게 적용되지 않으면 특정 쿼리가 불가능해질 수 있습니다. 이것은 빨리 빠져 나올 수 있습니다.





Netflix 측정 항목에는 일괄 적으로 태그가 지정됩니다. 각 메트릭에는 이름이 있지만이 단일 메트릭에는 더 많은 쿼리 유연성을 허용하는 여러 통계 및 '태그'키 / 값 쌍이 포함될 수 있습니다. 실제로 통계 자체는 특수 태그에 기록됩니다.





Netflix Servo 또는 Spectator로 기록 된 위에 설명 된 루트 끝점의 타이머에는 상태 코드 당 4 개의 통계가 포함됩니다. 여기서 카운트 통계는 Spring Boot Actuator의 카운터와 동일합니다. 지금까지 HTTP 200 및 400이 발생했다면 사용 가능한 데이터 포인트는 8 개가됩니다.







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



추가적인 의존성이나 설정없이 Spring Cloud 기반 서비스는 Servo를 자동 구성 `MonitorRegistry`하고 모든 Spring MVC 요청에 대한 메트릭 수집을 시작합니다. 기본적으로 이름 `rest`이 포함 된 서보 타이머 는 태그가있는 각 MVC 요청에 대해 기록됩니다.





1.  HTTP 메소드

2.  HTTP 상태 (예 : 200, 400, 500)

3.  URI (URI가 비어 있으면 "root"), Atlas에 대해 살균 됨

4.  요청 처리기가 예외를 던진 경우 예외 클래스 이름

5.  키 일치 `netflix.metrics.rest.callerHeader`가 있는 요청 헤더가 요청 에 설정된 경우 호출자 . 에 대한 기본 키가 없습니다 `netflix.metrics.rest.callerHeader`. 발신자 정보를 수집하려면 응용 프로그램 속성에 추가해야합니다.





`netflix.metrics.rest.metricName`메트릭 `rest`의 이름을 제공 한 이름 으로 변경 하는 속성을 설정하십시오 .





Spring AOP가 활성화되어 있고 `org.aspectj:aspectjweaver`런타임 클래스 패스에 존재한다면, Spring Cloud는 또한 모든 클라이언트 호출에서 메트릭을 수집 할 것이다 `RestTemplate`. 이름이있는 Servo 타이머 `restclient`는 태그가있는 각 MVC 요청에 대해 기록됩니다.





1.  HTTP 메소드

2.  HTTP 상태 (예 : 200, 400, 500), 응답이 null을 반환하면 "CLIENT_ERROR" `IOException`, `RestTemplate`메서드 실행 중에 "IO_ERROR" 가 발생한 경우

3.  Atlas에 대해 살생 된 URI

4.  고객 이름







### 통계 수집 : 관중



Spectator 메트릭을 사용하려면 다음에 대한 종속성을 포함시킵니다 `spring-boot-starter-spectator`.







        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-spectator</artifactId>
        </dependency>







스펙 테이터 용어에서 미터는 이름이 지정된, 유형이 지정된 및 태그가 지정된 구성이며 메트릭은 특정 시점의 주어진 미터의 값을 나타냅니다. 관측기 미터는 현재 여러 가지 구현이있는 레지스트리에 의해 생성되고 제어됩니다. Spectator는 4 미터 유형을 제공합니다 : 카운터, 타이머, 게이지 및 분배 요약.





Spring Cloud Spectator 통합 `com.netflix.spectator.api.Registry`은 당신을 위해 주사 가능한 인스턴스를 구성합니다. 특히, `ServoRegistry`단일 서보 API 하에서 REST 메트릭 콜렉션 및 Metrics를 Atlas 백엔드로 통합하기 위해 인스턴스를 구성합니다. 실질적으로 이것은 코드가 서보 모니터와 스펙 테이터 미터를 혼합하여 사용할 수 있으며 둘 다 스프링 부트 액츄에이터 `MetricReader`인스턴스 에 의해 스쿠프 되고 둘 다 아틀라스 백엔드로 배송된다는 것을 의미합니다.





#### 관중 카운터



카운터는 일부 이벤트가 발생하는 비율을 측정하는 데 사용됩니다.







    // create a counter with a name and a set of tags
    Counter counter = registry.counter("counterName", "tagKey1", "tagValue1", ...);
    counter.increment(); // increment when an event occurs
    counter.increment(10); // increment by a discrete amount







카운터는 단일 시간 정규화 통계를 기록합니다.







#### 관중 타이머



타이머는 일부 이벤트가 얼마나 오래 걸리는지 측정하는 데 사용됩니다. Spring Cloud는 스프링 MVC 요청 및 조건부 `RestTemplate`요청 을위한 타이머를 자동으로 기록 하며, 나중에 대기 시간과 같은 요청 관련 메트릭에 대한 대시 보드를 만드는 데 사용할 수있다.





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







타이머는 count, max, totalOfSquares 및 totalTime의 4 가지 통계를 동시에 기록합니다. 카운트 통계는 사용자가 `increment()`타이밍을 기록 할 때마다 카운터에서 한 번 호출 한 경우 카운터가 제공 한 단일 표준화 된 값과 항상 일치하므로 단일 작업 에 대해 별도로 계산하고 시간을 측정 할 필요는 거의 없습니다.





들어 [장기 실행 작업](https://github.com/Netflix/spectator/wiki/Timer-Usage#longtasktimer) , 관객은 특별한을 제공합니다 `LongTaskTimer`.







#### 스펙 테이터 게이지



게이지는 실행중인 상태의 대기열 또는 스레드 수와 같은 현재 값을 결정하는 데 사용됩니다. 게이지는 샘플링되므로 샘플간에 이러한 값이 변동하는 방식에 대한 정보는 제공하지 않습니다.





게이지의 정상적인 사용에는 초기화시 id, 샘플링 할 객체에 대한 참조, 객체를 기반으로 숫자 값을 가져 오거나 계산하는 함수를 사용하여 게이지를 등록하는 작업이 포함됩니다. 객체에 대한 참조는 별도로 전달되며 Spectator 레지스트리는 객체에 대한 약한 참조를 유지합니다. 개체가 가비지 수집 된 경우 관람자는 자동으로 등록을 취소합니다. 참조 [노트](https://github.com/Netflix/spectator/wiki/Gauge-Usage#using-lambda) 이 API가 잘못 사용되는 경우 잠재적 메모리 누수에 대한 관객의 문서를.







    // the registry will automatically sample this gauge periodically
    registry.gauge("gaugeName", pool, Pool::numberOfRunningThreads);

    // manually sample a value in code at periodic intervals -- last resort!
    registry.gauge("gaugeName", Arrays.asList("tagKey1", "tagValue1", ...), 1000);









#### 관람객 분포 요약



분배 요약은 이벤트 분배를 추적하는 데 사용됩니다. 그것은 타이머와 유사하지만 크기가 일정 시간 일 필요는 없다는 점에서보다 일반적입니다. 예를 들어, 분배 요약은 서버에 도달하는 요청의 페이로드 크기를 측정하는 데 사용될 수 있습니다.







    // the registry will automatically sample this gauge periodically
    DistributionSummary ds = registry.distributionSummary("dsName", "tagKey1", "tagValue1", ...);
    ds.record(request.sizeInBytes());











### 통계 수집 : 서보











경고

코드가 Java 8에서 컴파일 된 경우, 관측자로 서보 대신 관객을 사용하여 장기적으로 서보를 완전히 대체 할 예정입니다.|











서보 사용법에서 모니터는 명명 된, 입력 된 및 태그가 지정된 구성이고 메트릭은 특정 시점의 주어진 모니터 값을 나타냅니다. 서보 모니터는 관측기 미터와 논리적으로 동일합니다. 서보 모니터는에 의해 생성되고 제어됩니다 `MonitorRegistry`. 위의 경고에도 불구하고, Servo는 Spectator에 미터보다 [광범위한](https://github.com/Netflix/servo/wiki/Getting-Started) 모니터 옵션을 제공합니다.





Spring Cloud 통합 `com.netflix.servo.MonitorRegistry`은 당신을 위해 주사 가능한 인스턴스를 구성한다. `Monitor`Servo 에서 적절한 유형을 작성하면 데이터 기록 프로세스가 Spectator와 완전히 유사합니다.





#### 서보 모니터 만들기



`MonitorRegistry`Spring Cloud에서 제공 하는 Servo 인스턴스 (특히 인스턴스 `DefaultMonitorRegistry`)를 사용하는 경우 Servo는 [카운터](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamiccounter) 및 [타이머 검색](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamictimer) 을위한 편리한 클래스를 제공합니다 . 이 편리한 클래스 `Monitor`는 이름과 태그의 고유 한 조합마다 하나만 등록되도록합니다 .





서보에서 모니터 유형을 수동으로 작성하려면, 특히 편리한 메소드가 제공되지 않는 이국적인 모니터 유형의 `MonitorConfig`경우 , 인스턴스를 제공하여 적절한 유형을 인스턴스화하십시오 .







    MonitorConfig config = MonitorConfig.builder("timerName").withTag("tagKey1", "tagValue1").build();

    // somewhere we should cache this Monitor by MonitorConfig
    Timer timer = new BasicTimer(config);
    monitorRegistry.register(timer);











### Metrics Backend : Atlas



Atlas는 Netflix에서 거의 실시간 운영 통찰력을위한 차원 시계열 데이터를 관리하기 위해 개발되었습니다. Atlas는 메모리 내 데이터 스토리지를 특징으로하며 매우 많은 수의 메트릭을 매우 빨리 수집하고보고 할 수 있습니다.





Atlas는 운영 정보를 캡처합니다. 비즈니스 인텔리전스는 추세 분석을 위해 수집 된 데이터이지만 운영 인텔리전스는 시스템 내에서 현재 일어나고있는 상황을 보여줍니다.





Spring Cloud는 `spring-cloud-starter-atlas`필요한 모든 의존성을 가진 것을 제공한다 . 그런 다음 스프링 부트 애플리케이션에 주석을 달고 `@EnableAtlas`실행중인 Atlas 서버의 위치를 `netflix.atlas.uri`속성 과 함께 제공 하십시오.





#### 전역 태그



Spring Cloud를 사용하면 Atlas 백엔드에 전송 된 모든 메트릭에 태그를 추가 할 수 있습니다. 전역 태그를 사용하여 애플리케이션 이름, 환경, 지역 등으로 측정 항목을 분리 할 수 ​​있습니다.





구현하는 각 bean `AtlasTagProvider`은 전역 태그 목록에 기여합니다.







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

r3.2xlarge (61GB RAM)에서 실행되는 Atlas 독립형 노드는 주어진 6 시간 동안 분당 약 2 백만 개의 메트릭을 처리 할 수 ​​있습니다.|











일단 실행하고 몇 가지 메트릭을 수집했으면 Atlas 서버에 태그를 나열하여 설정이 올바른지 확인하십시오.







    $ curl http://ATLAS/api/v1/tags















팁

서비스에 대한 여러 요청을 실행 한 후 브라우저에 다음 URL을 붙여 넣어 요청의 대기 시간에 대한 몇 가지 기본적인 정보를 수집 할 수 있습니다. `[http://ATLAS/api/v1/graph?q=name,rest,:eq,:avg](http://atlas/api/v1/graph?q=name,rest,:eq,:avg)`|











Atlas wiki에는 다양한 시나리오에 대한 [샘플 쿼리](https://github.com/Netflix/atlas/wiki/Single-Line) 가 포함되어 있습니다 .





[경고 지수](https://github.com/Netflix/atlas/wiki/Alerting-Philosophy) 및 동적 경고 임계 [값](https://github.com/Netflix/atlas/wiki/DES) 을 생성하기 위해 [이중 지수 평활화](https://github.com/Netflix/atlas/wiki/DES) 사용에 대한 문서를 확인하십시오 .











# 스프링 클라우드 스트림







이 섹션에서는 Spring Cloud Stream을 사용하여 작업하는 방법에 대해 자세히 설명합니다. 스트림 응용 프로그램 작성 및 실행과 같은 주제를 다룹니다.









## Spring Cloud Stream 소개





Spring Cloud Stream은 메시지 기반 마이크로 서비스 애플리케이션을 구현하기위한 프레임 워크입니다. Spring Cloud Stream은 Spring Boot를 기반으로 독립형의 프로덕션 급 Spring 애플리케이션을 만들고 Spring Integration을 사용하여 메시지 브로커에 연결을 제공합니다. 여러 벤더의 미들웨어 구성에 대해 독창적 인 퍼블리시 - 서브 스크립 션 의미론, 소비자 그룹 및 파티션의 개념을 도입하여 독창적 인 구성을 제공합니다.





`@EnableBinding`주석을 응용 프로그램에 추가하여 메시지 브로커에 즉시 연결 `@StreamListener`하고 메소드에 추가 하여 스트림 처리를위한 이벤트를 수신하게 할 수 있습니다. 다음은 외부 메시지를받는 간단한 싱크 응용 프로그램입니다.







    @SpringBootApplication
    public class StreamApplication {

      public static void main(String[] args) {
        SpringApplication.run(StreamApplication.class, args);
      }
    }

    @EnableBinding(Sink.class)
    public class TimerSource {

      ...

      @StreamListener(Sink.INPUT)
      public void processVote(Vote vote) {
          votingService.recordVote(vote);
      }
    }







`@EnableBinding`주석 파라미터와 같은 하나 이상의 인터페이스 (이 경우, 파라미터는 싱글 얻어 `Sink`인터페이스). 인터페이스는 입력 및 / 또는 출력 채널을 선언합니다. Spring Cloud Stream은 인터페이스 `Source`를 제공하며 `Sink`, `Processor`; 자신 만의 인터페이스를 정의 할 수도 있습니다.





다음은 인터페이스의 정의입니다 `Source`.







    public interface Sink {
      String INPUT = "input";

      @Input(Sink.INPUT)
      SubscribableChannel input();
    }







`@Input`주석는 식별 _입력 채널_ 메시지 응용 프로그램을 입력받은 통해를; `@Output`애노테이션은 식별 _출력 채널_ 메시지 애플리케이션을두고 발행되는이. the `@Input`및 `@Output`주석은 채널 이름을 매개 변수로 사용할 수 있습니다. 이름이 제공되지 않으면 주석이 달린 메소드의 이름이 사용됩니다.





Spring Cloud Stream은 당신을위한 인터페이스 구현을 생성 할 것이다. 다음 테스트 사례의 예에서와 같이 자동 와이어 링을 사용하여 애플리케이션에서이를 사용할 수 있습니다.







    @RunWith(SpringJUnit4ClassRunner.class)
    @SpringApplicationConfiguration(classes = StreamApplication.class)
    @WebAppConfiguration
    @DirtiesContext
    public class StreamApplicationTests {

      @Autowired
      private Sink sink;

      @Test
      public void contextLoads() {
        assertNotNull(this.sink.input());
      }
    }











## 주요 개념





Spring Cloud Stream은 메시지 기반 마이크로 서비스 애플리케이션 작성을 단순화하는 많은 추상화 및 기본 기능을 제공합니다. 이 절에서는 다음을 개괄적으로 설명합니다.





*   Spring Cloud Stream의 애플리케이션 모델

*   바인더 추상화

*   지속적인 게시 - 구독 지원

*   소비자 그룹 지원

*   파티셔닝 지원

*   플러그 가능한 바인더 API





### 애플리케이션 모델



Spring Cloud Stream 애플리케이션은 미들웨어 중립적 인 코어로 구성된다. 응용 프로그램은 Spring Cloud Stream에 의해 입력 및 출력 _채널_ 을 통해 외부 세계와 통신합니다 . 채널은 미들웨어 관련 바인더 구현을 통해 외부 브로커에 연결됩니다.





![바인더가있는 SCSt](./spring-cloud-doc-resources/SCSt-with-binder.png)

그림 4\. Spring Cloud Stream 애플리케이션





#### 팻 항아리



Spring Cloud Stream 애플리케이션은 테스트를 위해 IDE에서 독립 실행 형 모드로 실행할 수 있습니다. 프로덕션 환경에서 Spring Cloud Stream 애플리케이션을 실행하려면 Maven 또는 Gradle 용으로 제공되는 표준 스프링 부트 도구를 사용하여 실행 파일 (또는 "fat") JAR을 작성할 수 있습니다.









### 바인더 추상화



Spring Cloud Stream은 [Kafka](https://github.com/spring-cloud/spring-cloud-stream/tree/master/spring-cloud-stream-binders/spring-cloud-stream-binder-kafka) , [Rabbit MQ](https://github.com/spring-cloud/spring-cloud-stream/tree/master/spring-cloud-stream-binders/spring-cloud-stream-binder-rabbit) , [Redis](https://github.com/spring-cloud/spring-cloud-stream-binder-redis) 및 [Gemfire](https://github.com/spring-cloud/spring-cloud-stream-binder-gemfire) 에 대한 바인더 구현을 제공합니다 . 또한 Spring Cloud Stream은 [TestSupportBinder](https://github.com/spring-cloud/spring-cloud-stream/blob/master/spring-cloud-stream-test-support/src/main/java/org/springframework/cloud/stream/test/binder/TestSupportBinder.java) 를 포함하고 있습니다. [TestSupportBinder](https://github.com/spring-cloud/spring-cloud-stream/blob/master/spring-cloud-stream-test-support/src/main/java/org/springframework/cloud/stream/test/binder/TestSupportBinder.java) 는 테스트가 직접 채널과 상호 작용할 수 있도록 채널을 변경하지 않고 수신 된 내용을 신뢰할 수있게 주장합니다. 확장 가능한 API를 사용하여 고유 한 바인더를 작성할 수 있습니다.





Spring Cloud Stream은 컨피규레이션을 위해 Spring Boot를 사용하고, Binder 추상화를 통해 Spring Cloud Stream 애플리케이션은 미들웨어에 유연하게 연결될 수있다. 예를 들어 배포자는 런타임에 채널이 연결되는 대상 (예 : Kafka 주제 또는 RabbitMQ 교환)을 동적으로 선택할 수 있습니다. 이러한 구성은 외부 구성 속성을 통해 (응용 인자 환경 변수 등을 포함하는 스프링 부트 지원하는 형태로 제공 될 수 `application.yml`또는 `application.properties`파일). [Introducing Spring Cloud Stream](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#_introducing_spring_cloud_stream) 섹션 의 싱크 예제에서 애플리케이션 속성 `spring.cloud.stream.bindings.input.destination`을 설정 `raw-sensor-data`하면 `raw-sensor-data`Kafka 주제 또는 `raw-sensor-data`RabbitMQ 교환에 바인드 된 대기열에서 읽게된다 .





Spring Cloud Stream은 클래스 패스에있는 바인더를 자동으로 감지하여 사용한다. 동일한 코드로 다른 유형의 미들웨어를 쉽게 사용할 수 있습니다. 빌드시 다른 바인더 만 포함하면됩니다. 보다 복잡한 사용 사례의 경우, 응용 프로그램에 여러 바인더를 패키지로 묶어 바인더를 선택하거나 런타임에 다른 채널에 다른 바인더를 사용할 지 여부도 결정할 수 있습니다.







### 영구 게시 - 구독 지원



응용 프로그램 간의 통신은 공유 주제를 통해 데이터가 브로드 캐스팅되는 게시 - 구독 모델을 따릅니다. 다음 그림은 상호 작용하는 Spring Cloud Stream 애플리케이션 세트의 일반적인 배치를 보여줍니다.





![SCSt 센서](./spring-cloud-doc-resources/SCSt-sensors.png)

그림 5\. Spring Cloud Stream 게시 - 구독





센서가 HTTP 끝점에보고 한 데이터는 이름이 지정된 공통 대상으로 전송됩니다 `raw-sensor-data`. 대상에서 시간 창 평균을 계산하는 마이크로 서비스 응용 프로그램과 원시 데이터를 HDFS로 가져 오는 다른 마이크로 서비스 응용 프로그램에 의해 독립적으로 처리됩니다. 데이터를 처리하기 위해 두 응용 프로그램은 런타임시 해당 주제를 입력으로 선언합니다.





게시 - 구독 통신 모델은 제작자와 소비자 모두의 복잡성을 줄여 주므로 기존 흐름을 방해하지 않으면 서 새로운 응용 프로그램을 토폴로지에 추가 할 수 있습니다. 예를 들어, 평균 계산 어플리케이션의 다운 스트림에서 디스플레이 및 모니터링을위한 최고 온도 값을 계산하는 어플리케이션을 추가 할 수 있습니다. 그런 다음 오류 감지를 위해 동일한 평균 평균 흐름을 해석하는 다른 애플리케이션을 추가 할 수 있습니다. 포인트 투 포인트 큐가 아닌 공유 토픽을 통해 모든 통신을 수행하면 마이크로 서비스 간의 커플 링이 감소합니다.





publish-subscribe 메시징의 개념은 새로운 것이 아니지만, Spring Cloud Stream은 애플리케이션 모델에 대해 독창적 인 선택으로 만드는 추가 단계를 필요로합니다. 네이티브 미들웨어 지원을 사용함으로써 Spring Cloud Stream은 다른 플랫폼에서 publish-subscribe 모델의 사용을 단순화합니다.







### 소비자 그룹



publish-subscribe 모델을 사용하면 공유 주제를 통해 응용 프로그램을 쉽게 연결할 수 있지만 주어진 응용 프로그램의 여러 인스턴스를 만들어 확장하는 기능도 똑같이 중요합니다. 이렇게하면 응용 프로그램의 다른 인스턴스가 경쟁 소비자 관계에 배치되며 인스턴스 중 하나만 주어진 메시지를 처리 ​​할 것으로 예상됩니다.





Spring Cloud Stream은 _소비자 그룹_ 의 개념을 통해 이러한 행동을 모델링 한다. (Spring Cloud Stream 소비자 그룹은 Kafka 소비자 그룹과 유사하고 영감을 받는다.) 각 소비자 바인딩은이 `spring.cloud.stream.bindings.input.group`속성을 사용하여 그룹 이름을 지정할 수있다. 다음 그림에 표시된 소비자의 경우이 속성은 `spring.cloud.stream.bindings.input.group=hdfsWrite`또는 으로 설정됩니다 `spring.cloud.stream.bindings.input.group=average`.





![SCSt 그룹](./spring-cloud-doc-resources/SCSt-groups.png)

그림 6\. Spring Cloud Stream Consumer Groups





주어진 대상에 가입 한 모든 그룹은 게시 된 데이터 사본을 받지만 각 그룹의 한 구성원 만 해당 대상에서 주어진 메시지를받습니다. 기본적으로 그룹을 지정하지 않으면 Spring Cloud Stream은 다른 모든 소비자 그룹과 게시 - 가입 관계에있는 익명의 독립적 인 단일 멤버 소비자 그룹에 애플리케이션을 할당한다.





#### 내구성



Spring Cloud Stream의 독창적 인 애플리케이션 모델과 일관되게, 소비자 그룹 가입은 _내구성이_ 있습니다. 즉, 바인더를 구현하면 그룹 가입이 영구적으로 유지되고 그룹에 대한 하나 이상의 가입이 생성되면 그룹의 모든 응용 프로그램이 중지되어있는 동안 그룹이 전송 되어도 메시지가 수신됩니다.













노트





익명 구독은 본질적으로 내구성이 없습니다. 일부 바인더 구현 (예 : RabbitMQ)의 경우 비 영구적 인 그룹 가입이 가능합니다.













일반적으로 응용 프로그램을 지정된 대상에 바인딩 할 때는 항상 소비자 그룹을 지정하는 것이 좋습니다. Spring Cloud Stream 애플리케이션을 확장 할 때, 각 입력 바인딩에 대한 소비자 그룹을 지정해야한다. 이렇게하면 응용 프로그램의 인스턴스가 중복 된 메시지를받지 않게됩니다 (예외적 인 경우는 예외입니다).









### 파티셔닝 지원



Spring Cloud Stream은 주어진 애플리케이션의 여러 인스턴스간에 데이터 를 _파티셔닝_ 하는 기능을 제공한다 . 분할 된 시나리오에서 물리적 통신 매체 (예 : 브로커 주제)는 여러 개의 파티션으로 구조화 된 것으로 간주됩니다. 하나 이상의 제작자 응용 프로그램 인스턴스가 여러 소비자 응용 프로그램 인스턴스에 데이터를 보내고 공통 특성으로 식별 된 데이터가 동일한 소비자 인스턴스에서 처리되도록합니다.





Spring Cloud Stream은 파티셔닝 된 프로세싱 유스 케이스를 일관된 방식으로 구현하기위한 공통된 추상화를 제공합니다. 따라서 브로커 자체가 자연스럽게 분할되었는지 (예 : Kafka) 또는 분할되지 않은 경우 (예 : RabbitMQ) 분할을 사용할 수 있습니다.





![SCSt 파티셔닝](./spring-cloud-doc-resources/SCSt-partitioning.png)

그림 7\. Spring Cloud Stream Partitioning





파티셔닝은 성능 또는 일관성을 이유로 모든 관련 데이터가 함께 처리되도록하는 비판적인 상태 보존 처리의 중요한 개념입니다. 예를 들어, 시간 창으로 표시된 평균 계산 예에서 주어진 센서의 모든 측정이 동일한 어플리케이션 인스턴스에 의해 처리되는 것이 중요합니다.













노트





파티션 된 처리 시나리오를 설정하려면 데이터 생성 및 데이터 소비 끝을 구성해야합니다.



















## 프로그래밍 모델





이 섹션에서는 Spring Cloud Stream의 프로그래밍 모델에 대해 설명한다. Spring Cloud Stream은 바인딩 된 입력 및 출력 채널을 선언하고 채널을 청취하는 방법에 대해 미리 정의 된 여러 주석을 제공합니다.





### 채널 선언 및 바인딩



#### 바인딩을 통해 트리거링 `@EnableBinding`



`@EnableBinding`애노테이션을 애플리케이션의 구성 클래스 중 하나 에 적용함으로써 Spring 애플리케이션을 Spring Cloud Stream 애플리케이션으로 바꿀 수있다. `@EnableBinding`주석 자체가 메타 주석 함께 `@Configuration`봄 클라우드 스트림 인프라의 구성을 트리거 :







    ...
    @Import(...)
    @Configuration
    @EnableIntegration
    public @interface EnableBinding {
        ...
        Class<?>[] value() default {};
    }







`@EnableBinding`바인딩 구성 요소 (일반적으로 메시지 채널)를 나타내는 방법을 포함하는 하나 이상의 인터페이스 클래스를 매개 변수로 주석이 걸릴 수 있습니다.













노트





Spring Cloud Stream 1.0에서 유일하게 지원되는 바인드 가능 구성 요소는 Spring Messaging `MessageChannel`과 그 확장 `SubscribableChannel`과 확장 `PollableChannel`이다. 이후 버전에서는 동일한 메커니즘을 사용하여이 지원을 다른 유형의 구성 요소로 확장해야합니다. 이 문서에서는 채널을 계속 참고할 것입니다.















#### `@Input` 과 `@Output`



Spring Cloud Stream 애플리케이션은 다음 `@Input`과 같이 인터페이스에 정의 된 임의의 수의 입력 및 출력 채널을 가질 수 있습니다 `@Output`.







    public interface Barista {

        @Input
        SubscribableChannel orders();

        @Output
        MessageChannel hotDrinks();

        @Output
        MessageChannel coldDrinks();
    }







매개 변수로이 인터페이스를 사용하기 `@EnableBinding`라는 세 가지 결합 채널의 생성을 트리거 `orders`, `hotDrinks`그리고 `coldDrinks`각각.







    @EnableBinding(Barista.class)
    public class CafeConfiguration {

       ...
    }







##### 채널 이름 사용자 정의



`@Input`and `@Output`주석을 사용하여 다음 예제와 같이 채널에 대해 사용자 정의 된 채널 이름을 지정할 수 있습니다.







    public interface Barista {
        ...
        @Input("inboundOrders")
        SubscribableChannel orders();
    }







이 예제에서 생성 된 바운드 채널의 이름이 지정 `inboundOrders`됩니다.







##### `Source`, `Sink`및`Processor`



입력 채널, 출력 채널 또는 둘 다를 포함하는 가장 일반적인 사용 사례를 쉽게 해결하기 위해 Spring Cloud Stream은 미리 정의 된 세 가지 인터페이스를 제공합니다.





`Source` 단일 아웃 바운드 채널이있는 응용 프로그램에 사용될 수 있습니다.







    public interface Source {

      String OUTPUT = "output";

      @Output(Source.OUTPUT)
      MessageChannel output();

    }







`Sink` 단일 인바운드 채널이있는 응용 프로그램에 사용할 수 있습니다.







    public interface Sink {

      String INPUT = "input";

      @Input(Sink.INPUT)
      SubscribableChannel input();

    }







`Processor` 인바운드 채널과 아웃 바운드 채널이 모두있는 응용 프로그램에 사용할 수 있습니다.







    public interface Processor extends Source, Sink {
    }







Spring Cloud Stream은 이러한 인터페이스를 특별히 처리하지 않는다. 그들은 단지 상자에서 제공됩니다.









#### 바운딩 된 채널 액세스



##### 바운딩 된 인터페이스 삽입하기



바인드 된 각 인터페이스에 대해 Spring Cloud Stream은 인터페이스를 구현하는 빈을 생성한다. 이 Bean들 중 하나의 주석 이 `@Input`달린 또는 `@Output`주석이 달린 메소드를 호출하면 관련 바운드 채널이 리턴됩니다.





다음 예제의 Bean은 `hello`메소드가 호출 될 때 출력 채널에서 메시지를 보냅니다 . `output()`주입 된 `Source`빈을 호출 하여 대상 채널을 검색합니다.







    @Component
    public class SendingBean {

        private Source source;

        @Autowired
        public SendingBean(Source source) {
            this.source = source;
        }

        public void sayHello(String name) {
             source.output().send(MessageBuilder.withPayload(body).build());
        }
    }









##### 직접 채널 주입



바운드 채널을 직접 주입 할 수도 있습니다.







    @Component
    public class SendingBean {

        private MessageChannel output;

        @Autowired
        public SendingBean(MessageChannel output) {
            this.output = output;
        }

        public void sayHello(String name) {
             output.send(MessageBuilder.withPayload(body).build());
        }
    }







채널의 이름이 선언 어노테이션에서 사용자 정의 된 경우 메소드 이름 대신 해당 이름을 사용해야합니다. 주어진 다음과 같은 선언 :







    public interface CustomSource {
        ...
        @Output("customOutput")
        MessageChannel output();
    }







다음 예제와 같이 채널이 주입됩니다.







    @Component
    public class SendingBean {

        @Autowired
        private MessageChannel output;

        @Autowired @Qualifier("customOutput")
        public SendingBean(MessageChannel output) {
            this.output = output;
        }

        public void sayHello(String name) {
             customOutput.send(MessageBuilder.withPayload(body).build());
        }
    }











#### 메시지 생성 및 사용



Spring Integration annotation이나 Spring Cloud Stream의 `@StreamListener`annotation을 사용하여 Spring Cloud Stream 애플리케이션을 작성할 수있다. `@StreamListener`주석은 다른 봄 메시징 주석을 모델로 (예입니다 `@MessageMapping`, `@JmsListener`, `@RabbitListener`, 등)하지만, 콘텐츠 형식 관리를 추가하고 강제 기능을 입력합니다.





##### 기본 스프링 통합 지원



Spring Cloud Stream은 Spring Integration을 기반으로하기 때문에 Stream은 Integration의 기초와 인프라는 물론 컴포넌트 자체를 완전히 상속받습니다. 예를 들어 a의 출력 채널을 a `Source`에 연결할 수 있습니다 `MessageSource`.







    @EnableBinding(Source.class)
    public class TimerSource {

      @Value("${format}")
      private String format;

      @Bean
      @InboundChannelAdapter(value = Source.OUTPUT, poller = @Poller(fixedDelay = "${fixedDelay}", maxMessagesPerPoll = "1"))
      public MessageSource<String> timerMessageSource() {
        return () -> new GenericMessage<>(new SimpleDateFormat(format).format(new Date()));
      }
    }







또는 변압기에서 프로세서 채널을 사용할 수 있습니다.







    @EnableBinding(Processor.class)
    public class TransformProcessor {
      @Transformer(inputChannel = Processor.INPUT, outputChannel = Processor.OUTPUT)
      public Object transform(String message) {
        return message.toUpper();
      }
    }









##### 자동 컨텐츠 유형 처리를 위해 @StreamListener 사용



그 봄의 통합 지원에 대한 보완, 봄 클라우드 스트림은 자체 제공하는 `@StreamListener`다른 봄 메시징 주석 (예를 모델로 주석을, `@MessageMapping`, `@JmsListener`, `@RabbitListener`, 등). 이 `@StreamListener`주석은 인바운드 메시지를 처리하기위한보다 단순한 모델을 제공합니다 . 특히 콘텐츠 형식 관리 및 유형 강제 변환과 관련된 사용 사례를 처리 할 때 더욱 그렇습니다.





Spring Cloud Stream은 `MessageConverter`바운드 채널에 의한 데이터 변환을 처리 할 수 있는 확장 가능한 메커니즘을 제공하며 ,이 경우에 주석이 달린 메소드로 디스 패칭한다 `@StreamListener`. 다음은 외부 `Vote`이벤트 를 처리하는 응용 프로그램의 예입니다 .







    @EnableBinding(Sink.class)
    public class VoteHandler {

      @Autowired
      VotingService votingService;

      @StreamListener(Sink.INPUT)
      public void handle(Vote vote) {
        votingService.record(vote);
      }
    }







구별 `@StreamListener`과 봄 통합 `@ServiceActivator`인바운드 고려할 때 볼 수 `Message`이 `String`페이로드와 `contentType`의 헤더를 `application/json`. 의 경우 `@StreamListener`, `MessageConverter`메커니즘은 `contentType`헤더를 사용 하여 `String`페이로드를 `Vote`오브젝트 로 구문 분석 합니다.





다른 Spring Messaging 메쏘드와 마찬가지로 메쏘드 인자는 `@Payload`, `@Headers`및로 주석 될 수 있습니다 `@Header`.













노트





데이터를 반환하는 메서드의 경우 `@SendTo`주석을 사용하여 메서드에서 반환 한 데이터의 출력 바인딩 대상을 지정 해야합니다 .







    @EnableBinding(Processor.class)
    public class TransformProcessor {

      @Autowired
      VotingService votingService;

      @StreamListener(Processor.INPUT)
      @SendTo(Processor.OUTPUT)
      public VoteResult handle(Vote vote) {
        return votingService.record(vote);
      }
    }























노트





RabbitMQ의 경우, 외부 응용 프로그램에서 컨텐트 유형 헤더를 설정할 수 있습니다. Spring Cloud Stream은 모든 유형의 전송 (일반적으로 헤더를 지원하지 않는 Kafka와 같은 전송 포함)에 사용되는 확장 된 내부 프로토콜의 일부로이를 지원합니다.

















#### 집합



Spring Cloud Stream은 여러 애플리케이션을 함께 결합하여 입력 및 출력 채널을 직접 연결하고 브로커를 통해 메시지를 교환하는 추가 비용을 피하는 기능을 제공합니다. Spring Cloud Stream 버전 1.0부터는 다음 유형의 애플리케이션에 대해서만 집계가 지원된다.





*   _sources_ - 이름이 지정된 단일 출력 채널이있는 응용 프로그램으로 `output`, 일반적으로 단일 유형의 바인딩이 있습니다.`org.springframework.cloud.stream.messaging.Source`

*   _싱크 (sinks)_ - 이름이 지정된 단일 입력 채널 `input`을 갖는 응용 프로그램으로서 일반적으로 유형의 단일 바인딩을 가짐`org.springframework.cloud.stream.messaging.Sink`

*   _프로세서_ - 명명 된 단일 입력 채널과 이름이 지정된 `input`단일 출력 채널 ( `output`일반적으로 단일 유형의 바인딩을 가짐)이있는 응용 프로그램 `org.springframework.cloud.stream.messaging.Processor`.





일련의 요소의 출력 채널이있는 경우 다음 요소의 입력 채널에 연결되는 일련의 상호 연결된 응용 프로그램을 만들어서 함께 집계 할 수 있습니다. 시퀀스는 하나 시작할 수 있습니다 _소스_ 또는 _프로세서_ , 그것은 임의의 수를 포함 할 수있는 _프로세서_ 와 하나로 끝나야합니다 _프로세서_ 또는 _싱크_ .





시작 및 끝 요소의 특성에 따라 시퀀스에는 다음과 같이 하나 이상의 바인딩 가능한 채널이있을 수 있습니다.





*   시퀀스가 소스로 시작하여 싱크로 끝나면 응용 프로그램 간의 모든 통신이 직접적이며 채널이 바인딩되지 않습니다.

*   시퀀스가 프로세서로 시작하면 입력 채널이 `input`집계 의 채널이되어 이에 따라 바인딩됩니다.

*   시퀀스가 프로세서로 끝나면 출력 채널은 집계의 채널이되고 이에 따라 `output`바인딩됩니다.





집계는 다음 `AggregateApplicationBuilder`예제와 같이 유틸리티 클래스 를 사용하여 수행 됩니다. 소스, 프로세서 및 싱크가 프로젝트에 정의되어 있거나 프로젝트 종속성 중 하나에 포함되어있는 프로젝트를 생각해 봅시다.







    @SpringBootApplication
    @EnableBinding(Sink.class)
    public class SinkApplication {

        private static Logger logger = LoggerFactory.getLogger(SinkModuleDefinition.class);

        @ServiceActivator(inputChannel=Sink.INPUT)
        public void loggerSink(Object payload) {
            logger.info("Received: " + payload);
        }
    }









    @SpringBootApplication
    @EnableBinding(Processor.class)
    public class ProcessorApplication {

        @Transformer
        public String loggerSink(String payload) {
            return payload.toUpperCase();
        }
    }









    @SpringBootApplication
    @EnableBinding(Source.class)
    public class SourceApplication {

        @Bean
        @InboundChannelAdapter(value = Source.OUTPUT)
        public String timerMessageSource() {
            return new SimpleDateFormat().format(new Date());
        }
    }







각 구성은 별도의 구성 요소를 실행하는 데 사용할 수 있지만이 경우 다음과 같이 함께 집계 할 수 있습니다.







    @SpringBootApplication
    public class SampleAggregateApplication {

        public static void main(String[] args) {
            new AggregateApplicationBuilder()
                .from(SourceApplication.class).args("--fixedDelay=5000")
                .via(ProcessorApplication.class)
                .to(SinkApplication.class).args("--debug=true").run(args);
        }
    }







시퀀스의 시작 구성 요소는 `from()`메소드의 인수로 제공됩니다 . 시퀀스의 끝 구성 요소는 `to()`메소드의 인수로 제공됩니다 . `via()`메소드의 인수로 중간 프로세서가 제공됩니다 . 동일한 유형의 여러 프로세서를 함께 연결할 수 있습니다 (예 : 다른 구성으로 파이프 라인 변환). 각 구성 요소에 대해 빌더는 스프링 부트 구성에 런타임 매개 변수를 제공 할 수 있습니다.







#### RxJava 지원



봄 클라우드 스트림은 통해 RxJava 기반 프로세서에 대한 지원 제공 `RxJavaProcessor`에서 사용할 수를 `spring-cloud-stream-rxjava`.







    public interface RxJavaProcessor<I, O> {
        Observable<O> process(Observable<I> input);
    }







의 구현 `RxJavaProcessor`받을 것입니다 `Observable`인바운드 메시지 페이로드의 흐름을 나타내는 입력으로. 이 `process`메소드는 시작시 데이터 흐름을 설정하기 위해 한 번 호출됩니다.





RxJava 기반 프로세서를 사용하도록 설정하고 주석을 사용하여 `@EnableRxJavaProcessor`프로세서 응용 프로그램에서 사용할 수 있습니다. `@EnableRxJavaProcessor`메타 주석이 첨부되어 `@EnableBinding(Processor.class)`있으며 `Processor`바인딩 이 만들어집니다 . 다음은 RxJava 기반 프로세서의 예입니다.







    @EnableRxJavaProcessor
    public class RxJavaTransformer {

        private static Logger logger = LoggerFactory.getLogger(RxJavaTransformer.class);

        @Bean
        public RxJavaProcessor<String,String> processor() {
            return inputStream -> inputStream.map(data -> {
                logger.info("Got data = " + data);
                return data;
            })
            .buffer(5)
            .map(data -> String.valueOf(avg(data)));
        }

        private static Double avg(List<String> data) {
            double sum = 0;
            double count = 0;
            for(String d : data) {
                count++;
                sum += Double.valueOf(d);
            }
            return sum/count;
        }
    }















노트





RxJava 프로세서를 구현할 때는 처리 흐름의 일부로 예외를 처리하는 것이 중요합니다. 잡히지 않은 예외는 RxJava에 의해 오류로 간주되어 처리 `Observable`를 완료하고 흐름을 방해합니다.





















## 바인더





Spring Cloud Stream은 외부 미들웨어의 물리적 대상에 연결하는 데 사용할 바인더 추상화를 제공합니다. 이 절에서는 바인더 SPI의 기본 개념, 주요 구성 요소 및 구현 관련 세부 정보에 대한 정보를 제공합니다.





### 생산자와 소비자



![생산자 소비자](./spring-cloud-doc-resources/producers-consumers.png)

도표 8\. 생산자와 소비자





_생산자는_ 채널에 메시지를 보내는 모든 구성 요소입니다. 채널은 해당 브로커에 대한 바인더 구현을 통해 외부 메시지 브로커에 바인딩 될 수 있습니다. 이 `bindProducer()`메소드 를 호출 할 때 첫 번째 매개 변수는 브로커 내의 대상 이름이고 두 번째 매개 변수는 생성자가 메시지를 보내는 로컬 채널 인스턴스이며 세 번째 매개 변수는 할 수있는 (예 : 파티션 키 표현식) 등록 정보를 포함합니다 해당 채널 용으로 작성된 어댑터 내에서 사용됩니다.





_소비자_ 채널에서 메시지를 수신하는 구성 요소입니다. 생산자와 마찬가지로 소비자의 채널은 외부 메시지 브로커에 바인딩 될 수 있습니다. `bindConsumer()`메서드 를 호출 할 때 첫 번째 매개 변수는 대상 이름이고 두 번째 매개 변수는 소비자의 논리 그룹 이름을 제공합니다. 주어진 목적지에 대한 소비자 바인딩에 의해 표현되는 각 그룹은 생산자가 그 목적지로 보내는 각 메시지의 복사본을받습니다 (즉, 발행 - 구독 의미론). 동일한 그룹 이름을 사용하여 바인딩 된 여러 소비자 인스턴스가있는 경우 메시지는 해당 소비자 인스턴스에서로드 균형 조정되므로 제작자가 보낸 각 메시지는 각 그룹 내의 단일 소비자 인스턴스 (즉, 큐잉 의미)에 의해 소비됩니다.







### 바인더 SPI



바인더 SPI는 다양한 인터페이스, 기본 제공 유틸리티 클래스 및 외부 미들웨어에 연결하기위한 플러그 가능한 메커니즘을 제공하는 검색 전략으로 구성됩니다.





SPI의 요점은 `Binder`입출력을 외부 미들웨어에 연결하는 전략 인 인터페이스입니다.







    public interface Binder<T, C extends ConsumerProperties, P extends ProducerProperties> {
        Binding<T> bindConsumer(String name, String group, T inboundBindTarget, C consumerProperties);

        Binding<T> bindProducer(String name, T outboundBindTarget, P producerProperties);
    }







인터페이스는 매개 변수화되어 여러 가지 확장 점을 제공합니다.





*   입력 및 출력 바인드 대상 - 버전 1.0부터 지원 `MessageChannel`되지만 이것은 향후 확장 점으로 사용하기위한 것입니다.

*   확장 된 소비자 및 프로듀서 속성 - 특정 Binder 구현이 유형 안전 방식으로 지원 될 수있는 보충 속성을 추가 할 수 있도록합니다.





일반적인 바인더 구현은 다음과 같이 구성됩니다.





*   인터페이스를 구현하는 클래스 `Binder`.

*   `@Configuration`미들웨어 연결 인프라와 함께 위 유형의 bean을 생성 하는 Spring 클래스.

*   `META-INF/spring.binders`하나 이상의 결합제 정의 등을 포함하는 클래스 경로에 찾은 파일







    kafka:\
    org.springframework.cloud.stream.binder.kafka.config.KafkaBinderConfiguration









### 바인더 감지



Spring Cloud Stream은 채널을 메시지 브로커에 연결하는 작업을 수행하기 위해 Binder SPI의 구현에 의존한다. 각 Binder 구현은 일반적으로 한 가지 유형의 메시징 시스템에 연결합니다. Spring Cloud Stream은 Kafka, RabbitMQ 및 Redis 용 바인더를 제공합니다.





#### 클래스 패스 감지



기본적으로 Spring Cloud Stream은 Spring Boot의 자동 설정에 의존하여 바인딩 프로세스를 구성합니다. 하나의 바인더 구현이 클래스 경로에서 발견되면 Spring Cloud Stream은 클래스 패스를 자동으로 사용합니다. 예를 들어 RabbitMQ에만 바인딩하려는 Spring Cloud Stream 프로젝트는 다음과 같은 종속성을 추가 할 수 있습니다.







    <dependency>
      <groupId>org.springframework.cloud</groupId>
      <artifactId>spring-cloud-stream-binder-rabbit</artifactId>
    </dependency>











### 클래스 패스의 다중 바인더



클래스 패스에 여러 바인더가있는 경우 응용 프로그램은 각 채널 바인딩에 사용할 바인더를 표시해야합니다. 각 바인더 구성에는 `META-INF/spring.binders`간단한 특성 파일 인 a 가 들어 있습니다 .







    rabbit:\
    org.springframework.cloud.stream.binder.rabbit.config.RabbitServiceAutoConfiguration







제공된 다른 바인더 구현 (예 : Kafka)에 대해서도 비슷한 파일이 존재하며, 사용자 정의 바인더 구현도이를 제공 할 것으로 예상됩니다. 키는 바인더 구현의 식별 이름을 나타내지 만 값은 쉼표로 구분 된 구성 클래스 목록입니다. 각 구성 클래스는 하나의 유형의 bean 정의 만 포함합니다 `org.springframework.cloud.stream.binder.Binder`.





바인더 선택은 각 채널 바인딩에 바인더를 구성 하여 `spring.cloud.stream.defaultBinder`속성 (예 `spring.cloud.stream.defaultBinder=rabbit`:) 또는 개별적으로 전역 적으로 수행 할 수 있습니다 . 예를 들어, Kafka에서 읽고 RabbitMQ에 쓰는 프로세서 응용 프로그램은 다음 구성을 지정할 수 있습니다.







```spring.cloud.stream.bindings.input.binder = kafka spring.cloud.stream.bindings.output.binder = 토끼```









### 여러 시스템에 연결



기본적으로 바인더는 응용 프로그램의 스프링 부트 자동 구성을 공유하므로 클래스 경로에있는 각 바인더의 인스턴스 하나가 만들어집니다. 응용 프로그램이 동일한 유형의 둘 이상의 브로커에 연결해야하는 경우 서로 다른 환경 설정을 갖는 여러 바인더 구성을 지정할 수 있습니다.













노트





명시 적 바인더 구성을 사용하면 기본 바인더 구성 프로세스가 사용 불가능하게됩니다. 이 작업을 수행하는 경우 사용중인 모든 바인더가 구성에 포함되어야합니다. Spring Cloud Stream을 투명하게 사용하려는 프레임 워크는 이름으로 참조 할 수있는 바인더 구성을 만들지 만 기본 바인더 구성에는 영향을 미치지 않습니다. 그렇게하기 위해서 바인더 `defaultCandidate`설정 은 그 플래그를 false로 설정할 수 `spring.cloud.stream.binders.<configurationName>.defaultCandidate=false`있습니다. 이것은 기본 바인더 구성 프로세스와 독립적으로 존재하는 구성을 나타냅니다.













예를 들어 두 개의 RabbitMQ 브로커 인스턴스에 연결하는 프로세서 응용 프로그램의 일반적인 구성은 다음과 같습니다.







    spring:
      cloud:
        stream:
          bindings:
            input:
              destination: foo
              binder: rabbit1
            output:
              destination: bar
              binder: rabbit2
          binders:
            rabbit1:
              type: rabbit
              environment:
                spring:
                  rabbitmq:
                    host: <host1>
            rabbit2:
              type: rabbit
              environment:
                spring:
                  rabbitmq:
                    host: <host2>









### 바인더 구성 등록 정보



사용자 정의 바인더 구성을 만들 때 다음 등록 정보를 사용할 수 있습니다. 접두어가 붙어야합니다 `spring.cloud.stream.binders.<configurationName>`.





<dl>

<dt class="hdlist1">유형</dt>

<dd>

바인더 타입. 일반적으로 클래스 패스에있는 바인더 중 하나, 특히 `META-INF/spring.binders`파일 의 키를 참조 합니다.



기본적으로 구성 이름과 동일한 값을 갖습니다.



</dd>

<dt class="hdlist1">상속 환경</dt>

<dd>

구성이 응용 프로그램 자체의 환경을 상속하는지 여부



기본값 `true`.



</dd>

<dt class="hdlist1">환경</dt>

<dd>

바인더 환경을 사용자 정의하는 데 사용할 수있는 특성 세트의 루트. 이것이 구성되면 바인더가 작성되는 컨텍스트가 응용 프로그램 컨텍스트의 하위가 아닙니다. 이를 통해 바인더 구성 요소와 응용 프로그램 구성 요소를 완전히 분리 할 수 ​​있습니다.



기본값 `empty`.



</dd>

<dt class="hdlist1">defaultCandidate</dt>

<dd>

바인더 구성이 기본 바인더로 간주 될 수 있는지 여부 또는 명시 적으로 참조 할 때만 사용할 수 있는지 여부 이렇게하면 기본 처리를 방해하지 않고 바인더 구성을 추가 할 수 있습니다.



기본값 `true`.



</dd>

</dl>







### 구현 전략



이 절에서는 Kafka와 Rabbit MQ에 대한 바인더 구현 전략에 대해 자세히 설명하며 Spring Cloud Stream 개념을 미들웨어 개념에 매핑하는 데 관심이있다.





#### 카프카 바인더



![카프카 바인더](./spring-cloud-doc-resources/kafka-binder.png)

그림 9\. 카프카 바인더





카프카 바인더 구현은 목적지를 카프카 (Kafka) 주제로 매핑합니다. 소비자 그룹은 동일한 카프카 개념에 직접 매핑됩니다. Spring Cloud Stream은 상위 소비자를 사용하지 않지만 단순한 소비자를 위해 유사한 개념을 구현한다.







#### RabbitMQ 바인더



![토끼 바인더](./spring-cloud-doc-resources/rabbit-binder.png)

그림 10\. RabbitMQ 바인더





RabbitMQ Binder 구현은 대상을 a로 매핑합니다 `TopicExchange`. 각 소비자 그룹에 대해 a `Queue`가 그것에 바인딩됩니다 `TopicExchange`. 바인딩하는 각 소비자 인스턴스는 `Consumer`해당 그룹의 해당 RabbitMQ 인스턴스 생성을 트리거 `Queue`합니다.













## 구성 옵션





Spring Cloud Stream은 바인딩 및 바인더에 대한 구성뿐만 아니라 일반 구성 옵션을 지원합니다. 일부 바인더는 미들웨어 관련 기능을 지원하기 위해 추가 바인딩 속성을 허용합니다.





Spring Boot가 지원하는 모든 메커니즘을 통해 Spring Cloud Stream 애플리케이션에 구성 옵션을 제공 할 수 있습니다. 여기에는 응용 프로그램 인수, 환경 변수 및 YAML 또는 .properties 파일이 포함됩니다.





### Spring Cloud Stream 등록 정보



<dl>

<dt class="hdlist1">spring.cloud.stream.instanceCount</dt>

<dd>

응용 프로그램의 배포 된 인스턴스 수입니다. 파티셔닝과 Kafka를 사용하는 경우 설정해야합니다.



기본값 : `1`.



</dd>

<dt class="hdlist1">spring.cloud.stream.instanceIndex</dt>

<dd>

응용 프로그램의 인스턴스 지수 :의 숫자 `0`로 `instanceCount`-1\. 파티셔닝 및 Kafka와 함께 사용됩니다. 애플리케이션의 인스턴스 색인과 일치하도록 Cloud Foundry에 자동으로 설정됩니다.

</dd>

<dt class="hdlist1">spring.cloud.stream.dynamicDestinations</dt>

<dd>

동적 라우팅 시나리오와 같이 동적으로 바인딩 할 수있는 대상 목록입니다. 설정된 경우 나열된 대상 만 바인딩 할 수 있습니다.



기본값 : 비어 있습니다 (대상을 바인딩 할 수 있음).



</dd>

<dt class="hdlist1">spring.cloud.stream.defaultBinder</dt>

<dd>

여러 바인더가 구성된 경우 사용할 기본 바인더입니다. [클래스 패스의 다중 바인더를](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#multiple-binders) 참조하십시오 .



기본값 : 비어 있습니다.



</dd>

<dt class="hdlist1">spring.cloud.stream.overrideCloudConnectors</dt>

<dd>

이 등록 정보는 `cloud`프로파일이 활성 상태이고 Spring Cloud Connectors가 응용 프로그램과 함께 제공되는 경우에만 적용 할 수 있습니다. 속성이 false (기본값) 인 경우 바인더는 적합한 바인딩 된 서비스 (예 : RabbitMQ 바인더에 대해 Cloud Foundry에서 바인딩 된 RabbitMQ 서비스)를 감지하고이를 연결 만들기 (일반적으로 Spring Cloud Connectors를 통해)에 사용합니다. true로 설정하면이 속성은 바인더가 바인딩 된 서비스를 완전히 무시하고 Spring 부트 속성에 의존하도록 지시합니다 (예 : `spring.rabbitmq.*`RabbitMQ 바인더의 환경에서 제공되는 속성에 의존 ). 이 속성의 일반적인 사용법은 [여러 시스템에](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#multiple-systems) 연결할 [때 사용자](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#multiple-systems) 정의 된 환경에 중첩됩니다 .



기본값 : false.



</dd>

</dl>







### 바인딩 속성



바인딩 속성은 형식을 사용하여 제공됩니다 `spring.cloud.stream.bindings.<channelName>.<property>=<value>`. 는 `<channelName>`구성중인 채널의 이름을 나타냅니다 (예 : `output`a `Source`).





다음에서는 `spring.cloud.stream.bindings.<channelName>.`접두사를 생략 한 위치 와 접두사가 런타임에 포함된다는 것을 알고 속성 이름에만 초점을 둡니다.





#### Spring Cloud Stream 사용을위한 등록 정보



다음 바인딩 특성은 입력 및 출력 바인딩 모두에 사용할 수 있으며 접두사가 붙어야합니다 `spring.cloud.stream.bindings.<channelName>.`.





<dl>

<dt class="hdlist1">목적지</dt>

<dd>

바운드 미들웨어 (예 : RabbitMQ exchange 또는 Kafka 주제)의 채널 대상 대상입니다. 채널이 소비자로 바인딩되면 여러 대상에 바인딩 될 수 있으며 대상 이름은 쉼표로 구분 된 문자열 값으로 지정할 수 있습니다. 설정하지 않으면 대신 채널 이름이 사용됩니다.

</dd>

<dt class="hdlist1">그룹</dt>

<dd>

채널의 소비자 그룹. 인바운드 바인딩에만 적용됩니다. [소비자 그룹을](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#consumer-groups) 참조하십시오 .



기본값 : null (익명 사용자를 나타냄).



</dd>

<dt class="hdlist1">컨텐츠 타입</dt>

<dd>

채널의 콘텐츠 유형입니다. // [[콘텐츠 형식 관리]를](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#content type management) 참조하십시오 .



기본값 : null (형식 강제 변환이 수행되지 않도록).



</dd>

<dt class="hdlist1">접합재</dt>

<dd>

이 바인딩에 사용되는 바인더입니다. 자세한 내용 [은 클래스 패스의 다중 바인더](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#multiple-binders) 를 참조하십시오.



기본값 : null (존재하는 경우 기본 바인더가 사용됩니다).



</dd>

</dl>







#### 소비자 재산



다음 Y 인딩 특성은 입력 Y 인딩에 대해서만 사용 가능하며 앞에 접두사가 있어야합니다 `spring.cloud.stream.bindings.<channelName>.consumer.`.





<dl>

<dt class="hdlist1">동시성</dt>

<dd>

인바운드 소비자의 동시성



기본값 : `1`.



</dd>

<dt class="hdlist1">분할 된</dt>

<dd>

소비자가 분할 된 제작자로부터 데이터를 수신하는지 여부입니다.



기본값 : `false`.



</dd>

<dt class="hdlist1">headerMode</dt>

<dd>

으로 설정 `raw`하면 입력시 헤더 구문 분석을 사용하지 않습니다. 기본적으로 메시지 헤더를 지원하지 않고 헤더 내장이 필요한 메시징 미들웨어에만 유효합니다. 인바운드 데이터가 Spring Cloud Stream 애플리케이션 외부에서 들어올 때 유용합니다.



기본값 : `embeddedHeaders`.



</dd>

<dt class="hdlist1">maxAttempts</dt>

<dd>

인바운드 메시지를 다시 처리하려는 시도 횟수입니다.



기본값 : `3`.



</dd>

<dt class="hdlist1">backOffInitialInterval</dt>

<dd>

다시 시도 할 때 백 오프 초기 간격입니다.



기본값 : `1000`.



</dd>

<dt class="hdlist1">backOffMaxInterval</dt>

<dd>

최대 백 오프 간격.



기본값 : `10000`.



</dd>

<dt class="hdlist1">backOffMultiplier</dt>

<dd>

백 오프 승수입니다.



기본값 : `2.0`.



</dd>

</dl>







#### 제작자 속성



다음 바인딩 특성은 출력 바인딩에만 사용 가능하며 접두어가 붙어야합니다 `spring.cloud.stream.bindings.<channelName>.producer.`.





<dl>

<dt class="hdlist1">partitionKeyExpression</dt>

<dd>

아웃 바운드 데이터를 분할하는 방법을 결정하는 SpEL 식입니다. set 또는 if `partitionKeyExtractorClass`가 설정된 경우,이 채널의 아웃 바운드 데이터가 분할되어 유효 `partitionCount`하기 위해 1보다 큰 값으로 설정되어야합니다. 두 옵션은 상호 배타적입니다. [파티셔닝 지원을](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#partitioning) 참조 [하십시오](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#partitioning) .



기본값 : null.



</dd>

<dt class="hdlist1">partitionKeyExtractorClass</dt>

<dd>

`PartitionKeyExtractorStrategy`구현입니다. set 또는 if `partitionKeyExpression`가 설정된 경우,이 채널의 아웃 바운드 데이터가 분할되어 유효 `partitionCount`하기 위해 1보다 큰 값으로 설정되어야합니다. 두 옵션은 상호 배타적입니다. [파티셔닝 지원을](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#partitioning) 참조 [하십시오](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#partitioning) .



기본값 : null.



</dd>

<dt class="hdlist1">partitionSelectorClass</dt>

<dd>

`PartitionSelectorStrategy`구현입니다. 함께 배타적입니다 `partitionSelectorExpression`. 모두가 설정되면, 파티션이 선정 될 `hashCode(key) % partitionCount`경우, `key`어느 하나를 통해 계산 `partitionKeyExpression`하거나 `partitionKeyExtractorClass`.



기본값 : null.



</dd>

<dt class="hdlist1">partitionSelectorExpression</dt>

<dd>

파티션 선택을 사용자 정의하기위한 SpEL 표현식. 함께 배타적입니다 `partitionSelectorClass`. 모두가 설정되면, 파티션이 선정 될 `hashCode(key) % partitionCount`경우, `key`어느 하나를 통해 계산 `partitionKeyExpression`하거나 `partitionKeyExtractorClass`.



기본값 : null.



</dd>

<dt class="hdlist1">partitionCount</dt>

<dd>

파티셔닝이 사용 가능한 경우 데이터의 대상 파티션 수입니다. 제작자가 분할 된 경우 1보다 큰 값으로 설정해야합니다. 카프카에서 힌트로 해석; 이것보다 크고 대상 주제의 파티션 수가 대신 사용됩니다.



기본값 : `1`.



</dd>

<dt class="hdlist1">필수 그룹</dt>

<dd>

생산자가 생성 된 후에 시작하더라도 (예 : RabbitMQ에서 영구 대기열을 미리 작성하여) 제작자가 메시지 전달을 보장해야하는 쉼표로 구분 된 그룹 목록입니다.

</dd>

<dt class="hdlist1">headerMode</dt>

<dd>

로 설정 `raw`하면 출력시 헤더 임베딩을 비활성화합니다. 기본적으로 메시지 헤더를 지원하지 않고 헤더 내장이 필요한 메시징 미들웨어에만 유효합니다. 비 Spring Cloud Stream 어플리케이션을위한 데이터를 생성 할 때 유용합니다.



태만: `embeddedHeaders`.



</dd>

</dl>













## 바인더 특정 구성





다음 바인더, 소비자 및 제작자 속성은 바인더 구현에만 적용됩니다.





### 토끼 별 설정



#### RabbitMQ 바인더 등록 정보



기본적으로 RabbitMQ 바인더는 Spring Boot 's를 사용합니다. `ConnectionFactory` SpringBoot를 모든 SpringBoot 구성 옵션을 지원합니다. (참고로 [스프링 부트 문서를](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/#common-application-properties) 참고하십시오 .) RabbitMQ 설정 옵션은 `spring.rabbitmq`접두사를 사용합니다 .





Spring Boot 옵션 외에도 RabbitMQ 바인더는 다음 등록 정보를 지원합니다.





<dl>

<dt class="hdlist1">spring.cloud.stream.rabbit.binder.adminAddresses</dt>

<dd>

쉼표로 구분 된 RabbitMQ 관리 플러그인 URL 목록입니다. 다음 경우에만 사용됩니다.`nodes`둘 이상의 항목이있을 . 이 목록의 각 항목에는에 해당 항목이 있어야합니다 `spring.rabbitmq.addresses`.



기본값 : 비어 있습니다.



</dd>

<dt class="hdlist1">spring.cloud.stream.rabbit.binder.nodes</dt>

<dd>

쉼표로 구분 된 RabbitMQ 노드 이름 목록. 둘 이상의 항목이있는 경우 대기열이있는 서버 주소를 찾는 데 사용됩니다. 이 목록의 각 항목에는 해당 항목이 있어야합니다.`spring.rabbitmq.addresses` .



기본값 : 비어 있습니다.



</dd>

<dt class="hdlist1">spring.cloud.stream.rabbit.binder.compressionLevel</dt>

<dd>

압축 된 바인딩의 압축 수준입니다. 참조하십시오 `java.util.zip.Deflater`.



기본값 : `1`(BEST_LEVEL).



</dd>

</dl>







#### RabbitMQ 소비자 속성



다음 속성은 토끼 소비자 만 사용할 수 있으며 접두어가 붙어야합니다 `spring.cloud.stream.rabbit.bindings.<channelName>.consumer.`.





<dl>

<dt class="hdlist1">acknowledgeMode</dt>

<dd>

확인 모드.



기본값 : `AUTO`.



</dd>

<dt class="hdlist1">autoBindDlq</dt>

<dd>

자동으로 DLQ를 선언하고 바인더 DLX에 바인드할지 여부.



기본값 : `false`.



</dd>

<dt class="hdlist1">내구재 구독</dt>

<dd>

가입이 내구성이 있어야하는지 여부. if `group`가 설정된 경우에만 유효 합니다.



기본값 : `true`.



</dd>

<dt class="hdlist1">maxConcurrency</dt>

<dd>

태만: `1`.

</dd>

<dt class="hdlist1">프리 페치</dt>

<dd>

프리 페치 횟수.



기본값 : `1`.



</dd>

<dt class="hdlist1">접두사</dt>

<dd>

이름에 추가 할 접두사 `destination`및 큐 .



기본값 : "".



</dd>

<dt class="hdlist1">recoverInterval</dt>

<dd>

연결 복구 시도 간격 (밀리 초).



기본값 : `5000`.



</dd>

<dt class="hdlist1">requeueRejected</dt>

<dd>

배달 오류를 다시 큐에 넣어야하는지 여부.



기본값 : `true`.



</dd>

<dt class="hdlist1">requestHeaderPatterns</dt>

<dd>

요청 헤더가 전송됩니다.



기본값 : `[STANDARD_REQUEST_HEADERS,'*']`.



</dd>

<dt class="hdlist1">replyHeaderPatterns</dt>

<dd>

응답 헤더가 전송됩니다.



기본값 : `[STANDARD_REPLY_HEADERS,'*']`.



</dd>

<dt class="hdlist1">republishToDlq</dt>

<dd>

기본적으로 재 시도 후에 실패한 메시지는 거부됩니다. 데드 - 레터 큐 (DLQ)가 구성된 경우, RabbitMQ는 실패한 메시지를 변경하지 않고 DLQ로 라우트합니다. 로 설정 `true`하면 버스는 최종 오류의 원인에서 발생한 예외 메시지 및 스택 추적을 포함하여 추가 헤더를 사용하여 실패한 메시지를 DLQ에 다시 게시합니다.

</dd>

<dt class="hdlist1">거래를 한</dt>

<dd>

거래 된 채널을 사용할지 여부.



기본값 : `false`.



</dd>

<dt class="hdlist1">txSize</dt>

<dd>

ack 사이의 배달 횟수.



기본값 : `1`.



</dd>

</dl>







#### 토끼 생산자 속성



다음 속성은 토끼 제작자 만 사용할 수 있으며 접두어가 붙어야합니다 `spring.cloud.stream.rabbit.bindings.<channelName>.producer.`.





<dl>

<dt class="hdlist1">autoBindDlq</dt>

<dd>

자동으로 DLQ를 선언하고 바인더 DLX에 바인드할지 여부.



기본값 : `false`.



</dd>

<dt class="hdlist1">batchingEnabled</dt>

<dd>

생산자가 메시지 일괄 처리를 사용할지 여부.



기본값 : `false`.



</dd>

<dt class="hdlist1">batchSize</dt>

<dd>

일괄 처리를 사용할 때 버퍼링 할 메시지 수입니다.



기본값 : `100`.



</dd>

<dt class="hdlist1">batchBufferLimit</dt>

<dd>

기본값 : `10000`.

</dd>

<dt class="hdlist1">batchTimeout</dt>

<dd>

기본값 : `5000`.

</dd>

<dt class="hdlist1">압박 붕대</dt>

<dd>

전송할 때 데이터를 압축해야하는지 여부.



기본값 : `false`.



</dd>

<dt class="hdlist1">배달 모드</dt>

<dd>

배달 모드.



기본값 : `PERSISTENT`.



</dd>

<dt class="hdlist1">접두사</dt>

<dd>

`destination`교환 의 이름에 추가되는 접두사 .



기본값 : "".



</dd>

<dt class="hdlist1">requestHeaderPatterns</dt>

<dd>

요청 헤더가 전송됩니다.



기본값 : `[STANDARD_REQUEST_HEADERS,'*']`.



</dd>

<dt class="hdlist1">replyHeaderPatterns</dt>

<dd>

응답 헤더가 전송됩니다.



기본값 : `[STANDARD_REPLY_HEADERS,'*']`.



</dd>

</dl>









### 카프카 특정 설정



#### 카프카 바인더 속성



<dl>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.brokers</dt>

<dd>

Kafka 바인더가 연결할 브로커 목록입니다.



기본값 : `localhost`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.defaultBrokerPort</dt>

<dd>

`brokers`포트 정보의 유무에 관계없이 지정된 호스트를 허용합니다 (예 :) `host1,host2:port2`. 브로커 목록에 포트가 구성되지 않은 경우 기본 포트를 설정합니다.



기본값 : `9092`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.zkNodes</dt>

<dd>

Kafka 바인더가 연결할 수있는 ZooKeeper 노드 목록입니다.



기본값 : `localhost`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.defaultZkPort</dt>

<dd>

`zkNodes`포트 정보의 유무에 관계없이 지정된 호스트를 허용합니다 (예 :) `host1,host2:port2`. 노드 목록에 포트가 구성되지 않은 경우 기본 포트를 설정합니다.



기본값 : `2181`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.headers</dt>

<dd>

바인더가 전송할 사용자 지정 헤더 목록입니다.



기본값 : 비어 있습니다.



</dd>

<dt class="hdlist1">offline.kafka.binder.offsetUpdateTimeWindow</dt>

<dd>

오프셋을 저장하는 빈도 (밀리 초)입니다. If는 무시됩니다 `0`.



기본값 : `10000`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.offsetUpdateCount</dt>

<dd>

소비 된 오프셋이 유지되는 업데이트 횟수의 빈도입니다. If는 무시됩니다 `0`. 함께 배타적입니다 `offsetUpdateTimeWindow`.



기본값 : `0`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.requiredAcks</dt>

<dd>

브로커에서 필요한 ack 수입니다.



기본값 : `1`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.minPartitionCount</dt>

<dd>

효과적인 경우에만 `autoCreateTopics`또는 `autoAddPartitions`설정됩니다. 바인더가 데이터를 생성 / 소비하는 주제에 대해 바인더가 구성 할 전역 최소 파티션 수입니다. `partitionCount`생산자 의 설정 또는 생산자의 `instanceCount`* `concurrency`설정 값에 의해 대체 될 수 있습니다 (둘 중 더 큰 경우).



기본값 : `1`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.replicationFactor</dt>

<dd>

자동 생성 된 주제의 복제 계수 `autoCreateTopics`활성화 된 .



기본값 : `1`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.autoCreateTopics</dt>

<dd>

로 설정 `true`하면 바인더가 자동으로 새 항목을 만듭니다. 으로 설정 `false`하면 바인더는 이미 구성된 주제에 의존합니다. 후자의 경우 주제가 존재하지 않으면 바인더가 시작되지 않습니다. 참고로이 설정은 `auto.topic.create.enable`브로커 의 설정과 는 독립적이며 영향을 미치지 않습니다. 서버가 항목 자동 생성으로 설정된 경우 기본 브로커 설정으로 메타 데이터 검색 요청의 일부로 만들어 질 수 있습니다.



기본값 : `true`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.autoAddPartitions</dt>

<dd>

로 설정 `true`하면 바인더가 필요한 경우 새 파티션을 추가합니다. 로 설정된 경우`false` 하면 바인더는 이미 구성된 주제의 파티션 크기에 의존합니다. 대상 항목의 파티션 수가 예상 값보다 작 으면 바인더가 시작되지 않습니다.



기본값 : `false`.



</dd>

<dt class="hdlist1">spring.cloud.stream.kafka.binder.socketBufferSize</dt>

<dd>

Kafka 소비자가 사용할 소켓 버퍼의 크기 (바이트).



기본값 : `2097152`.



</dd>

</dl>







#### 카프카 소비자 속성



다음 속성은 Kafka 소비자 만 사용할 수 있으며 접두어가 붙어야합니다 `spring.cloud.stream.kafka.bindings.<channelName>.consumer.`.





<dl>

<dt class="hdlist1">autoCommitOffset</dt>

<dd>

메시지가 처리되었을 때 오프셋을 자동 커밋할지 여부입니다. 로 설정된 `false`경우`Acknowledgment` 헤더 늦게 확인에 대한 메시지 헤더에서 사용할 수 있습니다.



기본값 : `true`.



</dd>

<dt class="hdlist1">autoCommitOnError</dt>

<dd>

if `autoCommitOffset`가 true 로 설정된 경우에만 유효합니다 `true`. 이 옵션을 `false`true 로 설정하면 오류가 발생하는 메시지에 대한 자동 커밋을 억제하고 성공적인 메시지에 대해서만 커밋합니다. 오류가 계속 발생하면 스트림에서 자동으로 마지막으로 처리 된 메시지를 재생할 수 있습니다. 로 설정된 경우 `true`, 항상 자동 커밋 (자동 커밋이 활성화 된 경우)됩니다. 설정되지 않은 경우 (기본값), `enableDlq`DLQ로 보내지는 오류 메시지를 자동 커미트하고, 그렇지 않은 경우 커미트하지 않는 것과 동일한 값을 효과적으로 갖습니다.



기본값 : 설정되지 않습니다.



</dd>

<dt class="hdlist1">recoverInterval</dt>

<dd>

연결 복구 시도 간격 (밀리 초).



기본값 : `5000`.



</dd>

<dt class="hdlist1">resetOffsets</dt>

<dd>

소비자가 제공 한 값으로 오프셋을 재설정할지 여부 `startOffset`.



기본값 : `false`.



</dd>

<dt class="hdlist1">startOffset</dt>

<dd>

새 그룹의 시작 오프셋 또는 때 `resetOffsets`입니다 `true`. 허용되는 값 : `earliest`, `latest`.



기본값 : null (와 동등 `earliest`).



</dd>

<dt class="hdlist1">enableDlq</dt>

<dd>

true로 설정되면 소비자에 대해 사용 가능 DLQ 작동을 송신합니다. 오류가 발생한 메시지는 이름이 지정된 주제로 전달 `error.<destination>.<group>`됩니다. 이는 오류의 수가 상대적으로 적고 원래의 전체 주제를 재생하는 것이 너무 번거로운 경우에 대한보다 일반적인 카프카 재생 시나리오에 대한 대체 옵션을 제공합니다.



기본값 : `false`.



</dd>

</dl>







#### 카프카 프로듀서 속성



다음 속성은 카프카 제작자 만 사용할 수 있으며 접두어가 붙어야합니다 `spring.cloud.stream.kafka.bindings.<channelName>.producer.`.





<dl>

<dt class="hdlist1">버퍼 크기</dt>

<dd>

Kafka 제작자가 전송하기 전에 배치 할 데이터의 양에 대한 상한값 (바이트).



기본값 : `16384`.



</dd>

<dt class="hdlist1">동조</dt>

<dd>

제작자가 동기인지 여부입니다.



기본값 : `false`.



</dd>

<dt class="hdlist1">batchTimeout</dt>

<dd>

생산자가 더 많은 메시지를 동일한 배치에 축적 할 수 있도록 보내기 전에 얼마나 기다릴 지 결정합니다. 일반적으로 제작자는 전혀 기다리지 않고 이전 보내기가 진행되는 동안 누적 된 모든 메시지를 보내기 만합니다. 0이 아닌 값은 대기 시간을 희생시키면서 처리량을 늘릴 수 있습니다.



기본값 : `0`.



</dd>

<dt class="hdlist1">maxRequestSize</dt>

<dd>

요청을 보내는 메시지의 최대 크기입니다.



기본값 : `1048576`.



</dd>

<dt class="hdlist1">구성</dt>

<dd>

일반 Kafka 제작자 속성을 포함하는 키 / 값 쌍으로 매핑합니다.



기본값 : 빈지도.



</dd>

</dl>













## 콘텐츠 유형 및 변환





생성 된 메시지의 컨텐트 유형에 대한 정보를 전달할 수 있도록 Spring Cloud Stream은 기본적으로 `contentType`헤더를 아웃 바운드 메시지 에 첨부 합니다. 헤더를 직접 지원하지 않는 미들웨어의 경우, Spring Cloud Stream은 아웃 바운드 메시지를 자체 봉투로 자동 포장하는 자체 메커니즘을 제공한다. 헤더를 지원하는 미들웨어의 경우, Spring Cloud Stream 애플리케이션은 비 Spring Cloud Stream 애플리케이션에서 주어진 컨텐츠 유형으로 메시지를 수신 할 수있다.





Spring Cloud Stream은 두 가지 방법으로이 정보를 기반으로 메시지를 처리 ​​할 수있다.





*   `contentType`인바운드 및 아웃 바운드 채널 설정을 통해

*   주석이 달린 메소드에 대해 수행 된 인수 맵핑을 통해 `@StreamListener`





Spring Cloud Stream을 사용하면 `content-type`바인딩 의 속성을 사용하여 입력 및 출력에 대한 유형 변환을 선언적으로 구성 할 수 있습니다 . 일반적인 유형 변환은 응용 프로그램 내부에서 변환기를 사용하여 쉽게 수행 할 수 있습니다. 현재, Spring Cloud Stream은 기본적으로 스트림에서 일반적으로 사용되는 다음 유형 변환을 지원합니다.





*   **POJO** 에서 / **POJO** 로가는 **JSON**

*   [org.springframework.tuple.Tuple](https://github.com/spring-projects/spring-tuple/blob/master/spring-tuple/src/main/java/org/springframework/tuple/Tuple.java) 에서 **JSON** 으로[](https://github.com/spring-projects/spring-tuple/blob/master/spring-tuple/src/main/java/org/springframework/tuple/Tuple.java)

*   **Object** to / from **byte []** : 원격 전송을 위해 직렬화 된 원시 바이트, 응용 프로그램에서 생성 된 바이트 또는 Java 직렬화를 사용하여 바이트로 변환 된 바이트 (객체가 직렬화 가능해야 함)

*   **바이트 [** /에서 **] ****문자열**

*   **Object** to **plain text** (객체의 _toString ()_ 메소드를 호출합니다 )





_JSON_ 은 _JSON이_ 포함 된 바이트 배열 또는 String 페이로드를 나타냅니다. 현재 개체는 JSON 바이트 배열 또는 String에서 변환 될 수 있습니다. JSON으로 변환하면 항상 String이 생성됩니다.





### MIME 유형



`content-type`값은 미디어 유형 (예 : `application/json`또는) 으로 구문 분석됩니다 `text/plain;charset=UTF-8`. MIME 유형은 특히 String 또는 byte [] 컨텐츠로 변환하는 방법을 나타내는 데 유용합니다. Spring Cloud Stream은 MIME 유형 형식을 사용하여 일반 유형 `application/x-java-object`을 `type`매개 변수 와 함께 사용하여 Java 유형을 나타 냅니다. 예를 들어, `application/x-java-object;type=java.util.Map`또는 입력 바인딩 `application/x-java-object;type=com.bar.Foo`의 `content-type`특성 으로 설정할 수 있습니다 . 또한 Spring Cloud Stream은 `application/x-spring-tuple`튜플을 지정하기 위해 사용자 정의 MIME 유형을 제공한다 .







### MIME 유형 및 Java 유형



Spring Cloud Stream에서 제공되는 유형 변환은 다음 표에 요약되어 있습니다.


| Source Payload          | Target Payload                | content-type header                  | content-type                         | Comments                                                    |
|-------------------------|-------------------------------|--------------------------------------|--------------------------------------|-------------------------------------------------------------|
| POJO                    | JSON String                   | ignored                              | application/json                     |                                                             |
| Tuple                   | JSON String                   | ignored                              | application/json                     | JSON is tailored for Tuple                                  |
| POJO                    | String (toString())           | ignored                              | text/plain, java.lang.String         |                                                             |
| POJO                    | byte\[\] (java.io serialized) | ignored                              | application/x-java-serialized-object |                                                             |
| JSON byte\[\] or String | POJO                          | application/json (or none)           | application/x-java-object            |                                                             |
| byte\[\] or String      | Serializable                  | application/x-java-serialized-object | application/x-java-object            |                                                             |
| JSON byte\[\] or String | Tuple                         | application/json (or none)           | application/x-spring-tuple           |                                                             |
| byte\[\]                | String                        | any                                  | text/plain, java.lang.String         | will apply any Charset specified in the content-type header |
| String                  | byte\[\]                      | any                                  | application/octet-stream             | will apply any Charset specified in the content-type header |




변환은 유형 변환이 필요한 페이로드에 적용됩니다. 예를 들어 모듈에서 outputType = application / json으로 XML 문자열을 생성하면 페이로드가 XML에서 JSON으로 변환되지 않습니다. 이는 모듈의 출력 채널에있는 페이로드가 이미 String이므로 런타임에 변환이 적용되지 않기 때문입니다.

변환은 입력 및 출력 채널 모두에서 지원되지만, 특히 아웃 바운드 메시지의 변환에 사용하는 것이 좋습니다. 인바운드 메시지 변환의 경우, 특히 대상이 POJO 인 경우 `@StreamListener`지원이 자동으로 변환을 수행합니다.




### `@StreamListener` 및 메시지 변환



`@StreamListener`주석 입력 채널의 컨텐츠 유형을 지정할 필요없이 수신 메시지를 변환하기위한 편리한 방법을 제공한다. 주석이 달린 메소드로 디스 `@StreamListener`패칭하는 동안 인수가 필요하면 변환이 자동으로 적용됩니다.





예를 들어 문자열 내용 `{"greeting":"Hello, world"}`과 `content-type`헤더 `application/json`가 입력 채널에서 수신 된 메시지를 생각해 봅시다 . 그것을받는 다음 응용 프로그램을 고려해 보겠습니다.







    public class GreetingMessage {

      String greeting;

      public String getGreeting() {
        return greeting;
      }

      public void setGreeting(String greeting) {
        this.greeting = greeting;
      }
    }

    @EnableBinding(Sink.class)
    @EnableAutoConfiguration
    public static class GreetingSink {

            @StreamListener(Sink.INPUT)
            public void receive(Greeting greeting) {
                // handle Greeting
            }
        }







메소드의 인수는 비 정렬 화 된 형태의 JSON String을 포함하는 POJO로 자동으로 채워질 것이다.











## 응용 프로그램 간 통신





### 여러 응용 프로그램 인스턴스 연결



Spring Cloud Stream은 개별 Spring Boot 애플리케이션이 메시징 시스템에 쉽게 연결될 수있게 해주지 만 Spring Cloud Stream의 전형적인 시나리오는 다중 애플리케이션 파이프 라인을 생성하는 것입니다. 여기서 다중 서비스 애플리케이션은 서로 데이터를 전송합니다. 인접한 응용 프로그램의 입력 목적지와 출력 목적지를 서로 연관시켜이 시나리오를 달성 할 수 있습니다.





디자인에서 Time Source 응용 프로그램이 Log Sink 응용 프로그램에 데이터를 보내도록 요청하면 `ticktock`두 응용 프로그램 내에서 바인딩 용으로 명명 된 공통 대상을 사용할 수 있습니다 .





시간 원본은 다음 속성을 설정합니다.







```spring.cloud.stream.bindings.output.destination = ticktock```







로그 싱크는 다음 속성을 설정합니다.







```spring.cloud.stream.bindings.input.destination = ticktock```









### 인스턴스 인덱스 및 인스턴스 수



Spring Cloud Stream 애플리케이션을 확장 할 때, 각 인스턴스는 동일한 애플리케이션의 다른 인스턴스가 몇 개 있고 인스턴스 인덱스가 무엇인지에 대한 정보를 수신 할 수 있습니다. Spring Cloud Stream은 `spring.cloud.stream.instanceCount`and 를 통해 이를 `spring.cloud.stream.instanceIndex`수행한다. 예를 들어, HDFS 싱크 애플리케이션의 세 가지 경우가있을 경우, 세 개의 인스턴스 것이다 `spring.cloud.stream.instanceCount`로 설정 `3`하고, 각각의 애플리케이션 것이다 `spring.cloud.stream.instanceIndex`설정 `0`, `1`및 `2`각각.





Spring Cloud Stream 애플리케이션이 Spring Cloud Data Flow를 통해 배치 될 때, 이러한 속성은 자동으로 구성됩니다. Spring Cloud Stream 애플리케이션이 독립적으로 실행될 때, 이러한 특성은 올바르게 설정되어야한다. 기본적 `spring.cloud.stream.instanceCount`이며 `1`, 및 `spring.cloud.stream.instanceIndex`이다 `0`.





규모가 확대 된 시나리오에서 이러한 두 속성의 올바른 구성은 일반적으로 파티션 동작 (아래 참조)을 처리하는 데 중요하며 두 속성은 특정 바인더 (예 : Kafka 바인더)에서 항상 필요하므로 데이터가 여러 소비자 인스턴스로 올바르게 분리.







### 파티셔닝



#### 파티셔닝을위한 출력 바인딩 구성



An output binding is configured to send partitioned data by setting one and only one of its `partitionKeyExpression` or `partitionKeyExtractorClass` properties, as well as its `partitionCount` property. For example, the following is a valid and typical configuration:







```spring.cloud.stream.bindings.output.producer.partitionKeyExpression=payload.id
spring.cloud.stream.bindings.output.producer.partitionCount=5```







Based on the above example configuration, data will be sent to the target partition using the following logic.





A partition key’s value is calculated for each message sent to a partitioned output channel based on the `partitionKeyExpression`. The `partitionKeyExpression` is a SpEL expression which is evaluated against the outbound message for extracting the partitioning key.













Tip

SpEL 표현식이 사용자의 필요에 충분하지 않은 경우 대신 인터페이스 `partitionKeyExtractorClass`를 구현하는 클래스로 속성 을 설정하여 파티션 키 값을 `org.springframework.cloud.stream.binder.PartitionKeyExtractorStrategy`계산할 수 있습니다. 대개 SpEL 표현식으로 충분해야하지만보다 복잡한 경우에는 사용자 정의 구현 전략을 사용할 수 있습니다.













메시지 키가 계산되면 파티션 선택 프로세스는 `0`및 사이의 값으로 대상 파티션을 결정합니다 `partitionCount - 1`. 대부분의 시나리오에서 적용 할 수있는 기본 계산은 수식을 기반으로합니다 `key.hashCode() % partitionCount`. 이것은 바인딩에서 사용자 정의 할 수 있습니다. SpEL 표현식을 키에 대해 ( `partitionSelectorExpression`속성 을 통해 ) 평가하거나 구현을 설정하여 `org.springframework.cloud.stream.binder.PartitionSelectorStrategy`( `partitionSelectorClass`속성 을 통해) 설정할 수 있습니다.





다음 섹션에서 설명하는 것처럼 고급 속성에 대해 추가 속성을 구성 할 수 있습니다.













노트





Kafka 바인더는이 `partitionCount`설정을 힌트로 사용하여 지정된 파티션 수 (함께 `minPartitionCount`사용되는 값 중 두 개가 최대 값) 와 함께 항목을 만듭니다 . `minPartitionCount`바인더와 응용 프로그램 모두 를 구성 할 때는 `partitionCount`큰 값이 사용 되므로주의하십시오 . 주제가 더 작은 파티션 수로 이미 존재하고 `autoAddPartitions`비활성화 된 경우 (기본값) 바인더가 시작되지 않습니다. 주제가 더 작은 파티션 수로 이미 존재하고 `autoAddPartitions`활성화 된 경우, 새 파티션이 추가됩니다. 최대 ( `minPartitionCount`및 `partitionCount`) 보다 많은 수의 파티션이있는 항목이 이미 있으면 기존 파티션 수가 사용됩니다.













##### 파티셔닝을위한 입력 바인딩 구성



입력 바인딩은 다음 예제 `partitioned`와 같이 속성 `instanceIndex`과 `instanceCount`응용 프로그램 자체 의 속성 을 설정하여 분할 된 데이터를 받도록 구성됩니다 .







```spring.cloud.stream.bindings.input.consumer.partitioned = true spring.cloud.stream.instanceIndex = 3 spring.cloud.stream.instanceCount = 5```







`instanceCount`값 데이터를 분할 할 필요가있는 어플리케이션 인스턴스들 사이의 총 수를 나타내고,이 `instanceIndex`사이에, 상기 복수의 인스턴스에서 유일한 값이어야 `0`하고 `instanceCount - 1`. 인스턴스 색인은 각 응용 프로그램 인스턴스가 데이터를 수신하는 고유 한 파티션 (또는 파티션 세트 인 Kafka의 경우)을 식별하는 데 도움이됩니다. 모든 데이터가 사용되도록하고 응용 프로그램 인스턴스가 상호 배타적 인 데이터 집합을 수신하도록하려면 두 값을 올바르게 설정하는 것이 중요합니다.





분할 된 데이터 처리를 위해 여러 인스턴스를 사용하는 시나리오는 독립형 케이스에서 설정하는 것이 복잡 할 수 있지만, Spring Cloud Dataflow는 입력 및 출력 값을 올바르게 채우고 런타임 인프라에 의존하여 정보를 제공함으로써 프로세스를 크게 단순화 할 수 있습니다 인스턴스 인덱스와 인스턴스 수에 대한 정보.















## 테스트





Spring Cloud Stream은 메시징 시스템에 연결하지 않고도 마이크로 서비스 애플리케이션을 테스트 할 수 있도록 지원합니다. 를 사용하여이를 수행 할 수 있습니다 `TestSupportBinder`. 이것은 특히 마이크로 서비스를 테스트하는 데 유용합니다.





은 `TestSupportBinder`사용자가 채널 바인딩과 상호 작용 애플리케이션에 의해 전송되고 수신 된 메시지하는지 검사 할 수 있도록





아웃 바운드 메시지 채널의 `TestSupportBinder`경우 단일 구독자를 등록하고 응용 프로그램에서 보낸 메시지를 유지합니다 `MessageCollector`. 그것들은 테스트 중에 검색 될 수 있고 그들에 대한 주장을 가질 수 있습니다.





또한 사용자는 인바운드 메시지 채널에 메시지를 보낼 수 있으므로 소비자 응용 프로그램에서 메시지를 사용할 수 있습니다. 다음 예는 프로세서에서 입력 및 출력 채널을 테스트하는 방법을 보여줍니다.







    @RunWith(SpringJUnit4ClassRunner.class)
    @SpringApplicationConfiguration(classes = ExampleTest.MyProcessor.class)
    @IntegrationTest({"server.port=-1"})
    @DirtiesContext
    public class ExampleTest {

      @Autowired
      private Processor processor;

      @Autowired
      private BinderFactory<MessageChannel> binderFactory;

      @Autowired
      private MessageCollector messageCollector;

      @Test
      @SuppressWarnings("unchecked")
      public void testWiring() {
        Message<String> message = new GenericMessage<>("hello");
        processor.input().send(message);
        Message<String> received = (Message<String>) messageCollector.forChannel(processor.output()).poll();
        assertThat(received.getPayload(), equalTo("hello world"));
      }

      @SpringBootApplication
      @EnableBinding(Processor.class)
      public static class MyProcessor {

        @Autowired
        private Processor channels;

        @Transformer(inputChannel = Processor.INPUT, outputChannel = Processor.OUTPUT)
        public String transform(String in) {
          return in + " world";
        }
      }
    }







위의 예에서는 입력 및 출력 채널이 있고 `Processor`인터페이스 를 통해 바인딩 된 응용 프로그램을 만듭니다. 바인딩 된 인터페이스가 테스트에 삽입되므로 두 채널 모두에 액세스 할 수 있습니다. 우리는 입력 채널 `MessageCollector`에서 메시지를 전송하고 있으며 결과적으로 출력 채널로 메시지를 전송하기 위해 Spring Cloud Stream의 테스트 지원에서 제공 한 것을 사용하고 있습니다. 메시지를 받으면 구성 요소가 올바르게 작동하는지 확인할 수 있습니다.









## 건강 지표





Spring Cloud Stream은 바인더에 대한 상태 표시기를 제공한다. 이름으로 등록 `binders`되며 `management.health.binders.enabled`속성 을 설정하여 활성화 또는 비활성화 할 수 있습니다 .









## 견본





Spring Cloud Stream 샘플의 경우 GitHub 의 [spring-cloud-stream-samples](https://github.com/spring-cloud/spring-cloud-stream-samples) 저장소 를 참조하십시오 .









## 시작하기





봄 클라우드 스트림 응용 프로그램을 만드는 시작하려면 방문 [봄 Initializr을](https://start.spring.io/) 하고 "GreetingSource"라는 이름의 새로운 메이븐 프로젝트를 만듭니다. Spring Boot 버전 1.3.4 SNAPSHOT을 선택하고 Stream Kafka (메시징을 위해 Kafka를 사용하게 될 것입니다)의 체크 박스를 검색하거나 체크하십시오.





그런 다음 클래스 `GreetingSource`와 동일한 패키지에 새 클래스를 만듭니다 `GreetingSourceApplication`. 다음 코드를 지정하십시오.







    import org.springframework.cloud.stream.annotation.EnableBinding;
    import org.springframework.cloud.stream.messaging.Source;
    import org.springframework.integration.annotation.InboundChannelAdapter;

    @EnableBinding(Source.class)
    public class GreetingSource {

        @InboundChannelAdapter(Source.OUTPUT)
        public String greet() {
            return "hello world " + System.currentTimeMillis();
        }
    }







`@EnableBinding`주석 스프링 통합 인프라 컴포넌트의 생성을 유발하는 것이다. 특히 Kafka 연결 팩토리, Kafka 아웃 바운드 채널 어댑터 및 Source 인터페이스 내에 정의 된 메시지 채널을 만듭니다.







    public interface Source {

      String OUTPUT = "output";

      @Output(Source.OUTPUT)
      MessageChannel output();

    }







또한 자동 구성은 기본 폴러를 생성하므로 `greet()`메서드가 초당 한 번 호출됩니다. 표준 Spring Integration `@InboundChannelAdapter`annotation은 반환 값을 메시지의 페이로드로 사용하여 소스의 출력 채널에 메시지를 보냅니다.





이 설정을 테스트하려면 Kafka 메시지 브로커를 실행하십시오. 이렇게하는 쉬운 방법은 Docker 이미지를 사용하는 것입니다.







    # On OS X
    $ docker run -p 2181:2181 -p 9092:9092 --env ADVERTISED_HOST=`docker-machine ip \`docker-machine active\`` --env ADVERTISED_PORT=9092 spotify/kafka

    # On Linux
    $ docker run -p 2181:2181 -p 9092:9092 --env ADVERTISED_HOST=localhost --env ADVERTISED_PORT=9092 spotify/kafka







응용 프로그램 빌드 :







```./mvnw 클린 패키지```







소비자 응용 프로그램은 비슷한 방식으로 코딩됩니다. Initializr로 돌아가서 LoggingSink라는 다른 프로젝트를 만듭니다. 그런 다음 `LoggingSink`클래스 `LoggingSinkApplication`와 동일한 패키지에 다음 코드를 사용하여 새 클래스를 만듭니다 .







    import org.springframework.cloud.stream.annotation.EnableBinding;
    import org.springframework.cloud.stream.annotation.StreamListener;
    import org.springframework.cloud.stream.messaging.Sink;

    @EnableBinding(Sink.class)
    public class LoggingSink {

        @StreamListener(Sink.INPUT)
        public void log(String message) {
            System.out.println(message);
        }
    }







응용 프로그램 빌드 :







```./mvnw 클린 패키지```







GreetingSource 응용 프로그램을 LoggingSink 응용 프로그램에 연결하려면 각 응용 프로그램이 동일한 대상 이름을 공유해야합니다. 아래 그림과 같이 두 응용 프로그램을 모두 시작하면 콘솔에 "hello world"및 타임 스탬프를 인쇄하는 소비자 응용 프로그램이 표시됩니다.







    cd GreetingSource
    java -jar target/GreetingSource-0.0.1-SNAPSHOT.jar --spring.cloud.stream.bindings.output.destination=mydest

    cd LoggingSink
    java -jar target/LoggingSink-0.0.1-SNAPSHOT.jar --server.port=8090 --spring.cloud.stream.bindings.input.destination=mydest







(다른 서버 포트는 두 응용 프로그램의 Spring Boot Actuator 끝점을 서비스하는 데 사용되는 HTTP 포트의 충돌을 방지합니다.)





LoggingSink 응용 프로그램의 출력은 다음과 같습니다.







    [           main] s.b.c.e.t.TomcatEmbeddedServletContainer : Tomcat started on port(s): 8090 (http)
    [           main] com.example.LoggingSinkApplication       : Started LoggingSinkApplication in 6.828 seconds (JVM running for 7.371)
    hello world 1458595076731
    hello world 1458595077732
    hello world 1458595078733
    hello world 1458595079734
    hello world 1458595080735









# 스프링 클라우드 버스



Spring Cloud Bus는 분산 시스템의 노드를 간단한 메시지 브로커와 연결합니다. 그런 다음 상태 변경 (예 : 구성 변경) 또는 기타 관리 지침을 브로드 캐스트하는 데 사용할 수 있습니다. 핵심 아이디어는 버스가 확장 된 스프링 부트 응용 프로그램 용 분산 액츄에이터와 비슷하지만 앱 간의 통신 채널로도 사용할 수 있다는 것입니다. 유일한 구현은 현재 AMQP 중개자를 전송으로 사용하지만 동일한 기본 기능 집합 (그리고 일부는 전송에 따라 다름)은 다른 전송을위한 로드맵에 있습니다.





## 빠른 시작





스프링 클라우드 버스는 클래스 패스에서 자체를 감지하면 스프링 부트 자동 구성을 추가하여 작동합니다. 버스를 활성화 하려면 종속성 관리 를 추가 `spring-cloud-starter-bus-amqp`하거나 `spring-cloud-starter-bus-kafka`Spring Cloud가 나머지를 처리해야합니다. 브로커 (RabbitMQ 또는 Kafka)가 사용 가능하고 구성되어 있는지 확인하십시오. localhost에서 실행하면 아무 것도 할 필요가 없지만 원격으로 실행중인 경우 Spring Cloud Connectors 또는 Spring Boot 규칙을 사용하여 브로커 자격 증명을 정의하십시오 (예 : Rabbit).





application.yml



```봄: rabbitmq : 호스트 : mybroker.com 포트 : 5672 사용자 이름 : 사용자 비밀 번호 : 비밀```







버스는 현재 모든 노드 수신 대기 또는 특정 서비스 (유레카에 정의 된대로)를위한 모든 노드로의 메시지 전송을 지원합니다. 미래에는 더 많은 선택기 기준이 추가 될 수 있습니다 (예 : 데이터 센터 Y의 서비스 X 노드 등 ...). 또한 `/bus/*`액추에이터 네임 스페이스 아래에 http 끝 점이 있습니다. 현재 두 가지가 구현되어 있습니다. 첫 번째 `/bus/env`노드는 각 노드의 스프링 환경을 업데이트하기 위해 키 / 값 쌍을 전송합니다. 둘째,, `/bus/refresh`모두가 `/refresh`끝점 에서 핑 (ping) 된 것처럼 각 응용 프로그램의 구성을 다시로드 합니다.













노트

버스 시동기는 Rabbit과 Kafka를 포함합니다. 두 가지가 가장 일반적인 구현이기 때문에 Spring Cloud Stream은 매우 유연하고 바인더는 함께 작동 `spring-cloud-bus`합니다.|















## 인스턴스 주소 지정





HTTP 종점은 "대상"매개 변수를 허용합니다 (예 : "/ bus / refresh? destination = customers : 9000", 대상은 `ApplicationContext`ID 임). ID가 버스의 인스턴스에 의해 소유되면 메시지를 처리하고 다른 모든 인스턴스는 ID를 무시합니다. 봄 부트는 당신의 ID를 설정 `ContextIdApplicationContextInitializer`의 조합으로 `spring.application.name`, 활성 프로필과 `server.port`기본적으로.









## 서비스의 모든 인스턴스 주소 지정





"destination"매개 변수는 인스턴스에서 메시지를 처리할지 여부를 결정 하기 위해 Spring에서 사용됩니다 `PathMatcher`(경로 구분자는 콜론 `:`). 위의 예제를 사용하면 "/ bus / refresh? destination = customers : **"는 `ApplicationContext`ID 로 설정된 프로필과 포트에 관계없이 "고객"서비스의 모든 인스턴스를 대상으로합니다 .









## 응용 프로그램 컨텍스트 ID는 고유해야합니다.





버스는 이벤트를 두 번 처리하지 않으려 `ApplicationEvent`고합니다. 한 번은 원본에서, 한 번은 대기열에서 처리합니다. 이렇게하려면 보내는 응용 프로그램 컨텍스트 ID가 현재 응용 프로그램 컨텍스트 ID를 다시 확인합니다. 서비스의 여러 인스턴스가 동일한 응용 프로그램 컨텍스트 ID를 갖는 경우 이벤트는 처리되지 않습니다. 로컬 컴퓨터에서 실행되는 각 서비스는 다른 포트에 있으며 응용 프로그램 컨텍스트 ID의 일부가됩니다. Cloud Foundry는 차별화 지수를 제공합니다. 응용 프로그램 컨텍스트 ID가 고유한지 확인하려면 `spring.application.index`서비스의 각 인스턴스에 대해 고유 한 값 으로 설정 하십시오. 예를 들어, lattice `spring.application.index=${INSTANCE_INDEX}`에서 application.properties (또는 configserver를 사용하는 경우 bootstrap.properties)를 설정하십시오.









## 메시지 브로커 사용자 정의





Spring Cloud Bus는 [Spring Cloud Stream](https://cloud.spring.io/spring-cloud-stream) 을 사용하여 메시지를 브로드 캐스트하므로 메시지를 전달할 때 클래스 패스에 선택한 바인더 구현 만 포함하면된다. AMQP (RabbitMQ)와 Kafka ( `spring-cloud-starter-bus-[amqp,kafka]`) 가있는 버스를위한 편리한 시동기가 있습니다 . 일반적으로 스프링 클라우드 스트림은 미들웨어 구성을위한 스프링 부트 자동 구성 규칙에 의존하기 때문에 구성 등록 정보를 사용하여 AMQP 브로커 주소를 변경할 수 있습니다 `spring.rabbitmq.*` . Spring Cloud Bus는 소수의 네이티브 구성 등록 정보를 가지고 있습니다 `spring.cloud.bus.*` (예 : 외부 미들웨어 `spring.cloud.bus.destination`를 사용하는 주제 이름). 일반적으로 기본값으로 충분합니다.





메시지 브로커 설정을 사용자 정의하는 방법에 대한 자세한 내용은 Spring Cloud Stream 문서를 참조하십시오.









## 추적 버스 이벤트





버스 이벤트 (서브 클래스 `RemoteApplicationEvent`)는 설정을 통해 추적 할 수 있습니다 `spring.cloud.bus.trace.enabled=true`. 이렇게하면 Spring Boot `TraceRepository`(있는 경우)는 전송 된 각 이벤트와 각 서비스 인스턴스의 모든 확인을 표시합니다. 예제 ( `/trace`끝점에서) :







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





상기 ACK 신호를 직접 처리하기 위해 당신은 추가 할 수 `@EventListener` 에 대한 `AckRemoteApplicationEvent`및 `SentApplicationEvent`앱에 대한 유형을 (그리고 추적을 사용 가능). 또는 `TraceRepository`거기에서 데이터를 가져 와서 데이터를 마이닝 할 수 있습니다.













노트

모든 버스 응용 프로그램은 acks를 추적 할 수 있지만 때때로 데이터에 대해 더 복잡한 쿼리를 수행 할 수있는 중앙 서비스에서이 작업을 수행하는 것이 유용합니다. 또는 전문화 된 추적 서비스로 전달하십시오.|















## 나만의 이벤트 방송





Bus는 어떤 타입의 이벤트라도 `RemoteApplicationEvent`나눌 수 있지만 기본 전송은 JSON이며 deserializer는 어떤 타입이 미리 사용될 것인지를 알아야합니다. 새로운 유형을 등록하려면 하위 패키지에 있어야 `org.springframework.cloud.bus.event`합니다. `@JsonTypeName`사용자 정의 클래스에서 사용하거나 클래스의 단순한 이름을 사용하는 기본 전략에 의존 할 수 있습니다 . 제작자와 소비자 모두 클래스 정의에 액세스해야합니다.







# 봄 구름 슬럼프







Adrian Cole, Spencer Gibb, Marcin Grzejszczak, Dave Syer





**Brixton.BUILD-SNAPSHOT**





Spring Cloud Sleuth는 [Spring Cloud](http://cloud.spring.io/) 를위한 분산 형 추적 솔루션을 구현 한다.









### 술어



Spring Cloud Sleuth는 [Dapper의](http://research.google.com/pubs/pub36356.html) 용어를 빌립니다.





**스팬 (Span) :** 기본 작업 단위. 예를 들어 RPC 전송은 새로운 응답이며 RPC에 응답을 보냅니다. 스팬은 스팬에 대한 고유 한 64 비트 ID와 스팬이 속한 트레이스에 대한 또 다른 64 비트 ID로 식별됩니다. 범위에는 설명, 타임 스탬프 이벤트, 키 - 값 주석 (태그), 원인이 된 범위의 ID 및 프로세스 ID (일반적으로 IP 주소)와 같은 다른 데이터도 있습니다.





스팬은 시작 및 중지되고 타이밍 정보를 추적합니다. 스팬을 작성한 후에는 나중에 스팬을 중지해야합니다.













팁

추적을 시작하는 초기 범위를 a라고합니다 `root span`. 해당 범위의 span id 값은 trace id와 같습니다.|











**추적 (Trace) :** 나무와 같은 구조를 형성하는 일련의 경간. 예를 들어 분산 대형 데이터 저장소를 실행중인 경우 put 요청으로 추적을 구성 할 수 있습니다.





**Annotation :** 일정 시간 내에 이벤트의 존재를 기록하는 데 사용됩니다. 요청 시작 및 중지를 정의하는 데 사용되는 핵심 주석 중 일부는 다음과 같습니다.





*   **cs** - 클라이언트 전송 됨 - 클라이언트가 요청했습니다. 이 주석은 범위의 시작을 나타냅니다.

*   **sr** - Server Received - 서버 쪽에서 요청을 받았으며 처리를 시작합니다. 이 타임 스탬프에서 cs 타임 스탬프를 빼면 네트워크 대기 시간이 표시됩니다.

*   **ss** - Server Sent - 요청 처리가 완료되면 주석이 달립니다 (응답이 클라이언트로 되돌아온 경우). 이 타임 스탬프에서 sr 시간 소인 수를 뺀 경우 서버 측에서 요청을 처리하는 데 필요한 시간을받습니다.

*   **cr** - 클라이언트 수신 - 범위의 끝을 나타냅니다. 클라이언트가 서버 측으로부터 응답을 성공적으로 수신했습니다. 이 타임 스탬프에서 cs 타임 스탬프를 빼면 서버에서 응답을 받기 위해 클라이언트가 필요로하는 전체 시간이 수신됩니다.





무엇을 시각화 **스팬** 및 **추적이** 지프 킨 주석과 함께 시스템에 보일 것이다 :





![추적 정보 전파](./spring-cloud-doc-resources/trace-id.png)





음표의 각 색상은 범위를 의미합니다 ( **A** 에서 **G** 까지 7 개 ). 메모에 이러한 정보가있는 경우 :







    Trace Id = X
    Span Id = D
    Client Sent







즉, 현재의 범위는 것을 의미 **추적 - 이드** 로 설정 **X** , **스팬 - 아이디** 로 설정 **D** . 또한 **Client Sent** 이벤트가 발생했습니다.





이것은 스팬의 부모 / 자식 관계를 시각화하는 방법입니다.





![부모 자녀 관계](./spring-cloud-doc-resources/parents.png)







### 목적



다음 섹션에서는 위 이미지의 예제가 고려됩니다.





#### Zipkin을 사용한 분산 추적



전체적으로 **7 개의 스팬이** 있습니다. Zipkin의 흔적에 가면 두 번째 흔적에이 숫자가 표시됩니다.





![흔적](./spring-cloud-doc-resources/zipkin-traces.png)





그러나 특정 추적을 선택하면 **4 개의 범위** 가 표시됩니다 .





![추적 정보 전파](./spring-cloud-doc-resources/zipkin-ui.png)













노트

특정 추적을 선택하면 병합 된 기간이 표시됩니다. 즉, Zipkin에 서버 수신 및 서버 전송 / 클라이언트 수신 및 클라이언트 전송 주석이있는 2 개의 스팬이있는 경우 단일 스팬으로 표시됩니다.|











왜이 경우 7과 4 사이의 차이가 있습니까?





*   2 스팬은 스팬에서옵니다 `http:/start`. 서버 수신 (SR) 및 서버 전송 (SS) 주석이 있습니다.

*   2 스팬에서 RPC 호출에서 오는 `service1`에 `service2`받는 `http:/foo`엔드 포인트. 클라이언트 송신 (CS) 및 클라이언트 수신 (CR) 주석이 `service1`있습니다. 또한 서버 수신 (SR) 및 서버 송신 (SS) 주석이 `service2`측면에 있습니다. 물리적으로 2 개의 범위가 있지만 RPC 호출과 관련된 1 개의 논리적 범위를 형성합니다.

*   2 스팬에서 RPC 호출에서 오는 `service2`에 `service3`받는 `http:/bar`엔드 포인트. 클라이언트 송신 (CS) 및 클라이언트 수신 (CR) 주석이 `service2`있습니다. 또한 서버 수신 (SR) 및 서버 송신 (SS) 주석이 `service3`측면에 있습니다. 물리적으로 2 개의 범위가 있지만 RPC 호출과 관련된 1 개의 논리적 범위를 형성합니다.

*   2 스팬에서 RPC 호출에서 오는 `service2`에 `service4`받는 `http:/baz`엔드 포인트. 클라이언트 송신 (CS) 및 클라이언트 수신 (CR) 주석이 `service2`있습니다. 또한 서버 수신 (SR) 및 서버 송신 (SS) 주석이 `service4`측면에 있습니다. 물리적으로 2 개의 범위가 있지만 RPC 호출과 관련된 1 개의 논리적 범위를 형성합니다.





우리는 물리적 스팬을 계산한다면 우리는이 **일** 에서 `http:/start`, **2** 에서 `service1`호출 `service2`, **이** 형태의 `service2` 호출 `service3`과 **2** 에서 `service2`호출 `service4`. 전체 **7 개의** 스팬.





논리적으로 우리의 정보를 참조 **총 스팬 : 4** 우리가 가지고 있기 때문에 **1** 입력에 요청 관련 기간 `service1`과 **3** RPC 호출과 관련된 스팬.







#### 오류 시각화



Zipkin을 사용하면 추적에서 오류를 시각화 할 수 있습니다. 예외가 발생하고 잡히지 않으면 Zipkin이 제대로 채색 할 수있는 범위에 적절한 태그를 설정합니다. 추적 목록에서 빨간색으로 된 하나의 추적을 볼 수 있습니다. 예외가 발생했기 때문입니다.





해당 추적을 클릭하면 비슷한 그림이 나타납니다.





![오류 추적](./spring-cloud-doc-resources/zipkin-error-traces.png)





다음 중 하나를 클릭하면 다음을 볼 수 있습니다.





![오류 추적 정보 전파](./spring-cloud-doc-resources/zipkin-error-trace-screenshot.png)





보시다시피 오류의 원인과 오류와 관련된 전체 스택 추적을 쉽게 볼 수 있습니다.







#### 실제 예제



[![Zivkin이 Pivotal Web Services에 배포되었습니다.](./spring-cloud-doc-resources/pws.png)](https://docssleuth-zipkin-server.cfapps.io/)

Pivotal Web Services 아이콘을 클릭하면 라이브가 표시됩니다. Pivotal Web Services 아이콘을 클릭하면 라이브가 표시됩니다.





Zipkin의 종속성 그래프는 다음과 같습니다.





![종속성](./spring-cloud-doc-resources/dependencies.png)





[![Zivkin이 Pivotal Web Services에 배포되었습니다.](./spring-cloud-doc-resources/pws.png)](https://docssleuth-zipkin-server.cfapps.io/dependency)

Pivotal Web Services 아이콘을 클릭하면 라이브가 표시됩니다. Pivotal Web Services 아이콘을 클릭하면 라이브가 표시됩니다.







#### 로그 상관 관계



예를 들어 `2485ec27856c56f4`1 과 같은 추적 ID로 4 개의 애플리케이션 로그를 그릴 때 다음과 같은 결과가 나옵니다.







    service1.log:2016-02-26 11:15:47.561  INFO [service1,2485ec27856c56f4,2485ec27856c56f4,true] 68058 --- [nio-8081-exec-1] i.s.c.sleuth.docs.service1.Application   : Hello from service1\. Calling service2
    service2.log:2016-02-26 11:15:47.710  INFO [service2,2485ec27856c56f4,9aa10ee6fbde75fa,true] 68059 --- [nio-8082-exec-1] i.s.c.sleuth.docs.service2.Application   : Hello from service2\. Calling service3 and then service4
    service3.log:2016-02-26 11:15:47.895  INFO [service3,2485ec27856c56f4,1210be13194bfe5,true] 68060 --- [nio-8083-exec-1] i.s.c.sleuth.docs.service3.Application   : Hello from service3
    service2.log:2016-02-26 11:15:47.924  INFO [service2,2485ec27856c56f4,9aa10ee6fbde75fa,true] 68059 --- [nio-8082-exec-1] i.s.c.sleuth.docs.service2.Application   : Got response from service3 [Hello from service3]
    service4.log:2016-02-26 11:15:48.134  INFO [service4,2485ec27856c56f4,1b1845262ffba49d,true] 68061 --- [nio-8084-exec-1] i.s.c.sleuth.docs.service4.Application   : Hello from service4
    service2.log:2016-02-26 11:15:48.156  INFO [service2,2485ec27856c56f4,9aa10ee6fbde75fa,true] 68059 --- [nio-8082-exec-1] i.s.c.sleuth.docs.service2.Application   : Got response from service4 [Hello from service4]
    service1.log:2016-02-26 11:15:48.182  INFO [service1,2485ec27856c56f4,2485ec27856c56f4,true] 68058 --- [nio-8081-exec-1] i.s.c.sleuth.docs.service1.Application   : Got response from service2 [Hello from service2, response from service3 [Hello from service3] and from service4 [Hello from service4]]







이 같은 로그 집계 도구를 사용하는 경우 [키바을](https://www.elastic.co/products/kibana) , [인 Splunk는](http://www.splunk.com/) 등 당신이 일어난 이벤트를 주문할 수 있습니다. Kibana의 예는 다음과 같습니다.





![Kibana와 로그 상관 관계](./spring-cloud-doc-resources/kibana.png)





여기서 [Logstash](https://www.elastic.co/guide/en/logstash/current/index.html) 를 사용하려면 [Logstash](https://www.elastic.co/guide/en/logstash/current/index.html) 의 Grok 패턴을 사용하십시오.







    filter {
           # pattern matching logback pattern
           grok {
                  match => { "message" => "%{TIMESTAMP_ISO8601:timestamp}\s+%{LOGLEVEL:severity}\s+\[%{DATA:service},%{DATA:trace},%{DATA:span},%{DATA:exportable}\]\s+%{DATA:pid}---\s+\[%{DATA:thread}\]\s+%{DATA:class}\s+:\s+%{GREEDYDATA:rest}" }
           }
    }















노트

Grok을 Cloud Foundry의 로그와 함께 사용하려면이 패턴을 사용해야합니다.|













    filter {
           # pattern matching logback pattern
           grok {
                  match => { "message" => "(?m)OUT\s+%{TIMESTAMP_ISO8601:timestamp}\s+%{LOGLEVEL:severity}\s+\[%{DATA:service},%{DATA:trace},%{DATA:span},%{DATA:exportable}\]\s+%{DATA:pid}---\s+\[%{DATA:thread}\]\s+%{DATA:class}\s+:\s+%{GREEDYDATA:rest}" }
           }
    }







##### Logstash로 JSON 로그백



로그 파일을 텍스트 파일에 저장하지 않고 Logstash에서 즉시 선택할 수있는 JSON 파일에 저장하는 경우가 많습니다. 그렇게하기 위해서는 다음을 수행해야합니다 (가독성을 위해 `groupId:artifactId:version`표기법 의 종속성을 전달합니다) .





**종속성 설정**





*   Classback ( `ch.qos.logback:logback-core`) 에 Logback이 있는지 확인하십시오.

*   Logstash Logback 인코딩 추가 - 버전 예 `4.6`:`net.logstash.logback:logstash-logback-encoder:4.6`





**로그백 설정**





다음은 Logback 구성 ( [logback-spring.xml](https://github.com/spring-cloud-samples/sleuth-documentation-apps/blob/master/service1/src/main/resources/logback-spring.xml) 파일 )의 예입니다.





*   애플리케이션의 정보를 JSON 형식으로 `build/${spring.application.name}.json`파일 에 기록 합니다.

*   콘솔과 표준 로그 파일이라는 두 개의 추가 appenders를 주석 처리했습니다.

*   이전 섹션에서 제시된 것과 동일한 로깅 패턴을가집니다.













노트

사용자 정의 `logback-spring.xml`를 사용하는 경우 속성 파일 대신 `spring.application.name`in 을 전달해야 합니다. 그렇지 않으면 사용자 지정 로그백 파일이 속성을 제대로 읽지 않습니다. `bootstrap``application`|

















### 프로젝트에 추가하기



#### Only Sleuth (로그 상관)



Zipkin 통합없이 Spring Cloud Sleuth에서만 이익을 얻고 싶다면 `spring-cloud-starter-sleuth`프로젝트에 모듈을 추가하십시오 .





메이븐



    <dependencyManagement> (1)
          <dependencies>
              <dependency>
                  <groupId>org.springframework.cloud</groupId>
                  <artifactId>spring-cloud-dependencies</artifactId>
                  <version>Brixton.RELEASE</version>
                  <type>pom</type>
                  <scope>import</scope>
              </dependency>
          </dependencies>
    </dependencyManagement>

    <dependency> (2)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-starter-sleuth</artifactId>
    </dependency>







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-starter-sleuth`





요람



    dependencyManagement { (1)
        imports {
            mavenBom "org.springframework.cloud:spring-cloud-dependencies:Brixton.RELEASE"
        }
    }

    dependencies { (2)
        compile "org.springframework.cloud:spring-cloud-starter-sleuth"
    }







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-starter-sleuth`







#### HTTP를 통한 Zipkin의 숙달



Sleuth와 Zipkin을 모두 추가하려면 종속성 만 추가하면 `spring-cloud-starter-zipkin`됩니다.





메이븐



    <dependencyManagement> (1)
          <dependencies>
              <dependency>
                  <groupId>org.springframework.cloud</groupId>
                  <artifactId>spring-cloud-dependencies</artifactId>
                  <version>Brixton.RELEASE</version>
                  <type>pom</type>
                  <scope>import</scope>
              </dependency>
          </dependencies>
    </dependencyManagement>

    <dependency> (2)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-starter-zipkin</artifactId>
    </dependency>







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-starter-zipkin`





요람



    dependencyManagement { (1)
        imports {
            mavenBom "org.springframework.cloud:spring-cloud-dependencies:Brixton.RELEASE"
        }
    }

    dependencies { (2)
        compile "org.springframework.cloud:spring-cloud-starter-zipkin"
    }







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-starter-zipkin`







#### 스프링 클라우드 스트림을 통한 Zipkin의 Sleuth



Sleuth와 Zipkin을 모두 추가하려면 종속성 만 추가하면 `spring-cloud-sleuth-stream`됩니다.





메이븐



    <dependencyManagement> (1)
          <dependencies>
              <dependency>
                  <groupId>org.springframework.cloud</groupId>
                  <artifactId>spring-cloud-dependencies</artifactId>
                  <version>Brixton.RELEASE</version>
                  <type>pom</type>
                  <scope>import</scope>
              </dependency>
          </dependencies>
    </dependencyManagement>

    <dependency> (2)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-sleuth-stream</artifactId>
    </dependency>
    <dependency> (3)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-starter-sleuth</artifactId>
    </dependency>
    <!-- EXAMPLE FOR RABBIT BINDING -->
    <dependency> (4)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-stream-binder-rabbit</artifactId>
    </dependency>







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-sleuth-stream`

3.  의존성 추가 `spring-cloud-starter-sleuth`- 모든 종속 종속성이 다운로드됩니다.

4.  바인더 (예 : 토끼 바인더)를 추가하여 Spring Cloud Stream에 바인드 할 내용을 지정하십시오.





요람



    dependencyManagement { (1)
        imports {
            mavenBom "org.springframework.cloud:spring-cloud-dependencies:Brixton.RELEASE"
        }
    }

    dependencies {
        compile "org.springframework.cloud:spring-cloud-sleuth-stream" (2)
        compile "org.springframework.cloud:spring-cloud-starter-sleuth" (3)
        // Example for Rabbit binding
        compile "org.springframework.cloud:spring-cloud-stream-binder-rabbit" (4)
    }







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-sleuth-stream`

3.  의존성 추가 `spring-cloud-starter-sleuth`- 모든 종속 종속성이 다운로드됩니다.

4.  바인더 (예 : 토끼 바인더)를 추가하여 Spring Cloud Stream에 바인드 할 내용을 지정하십시오.







#### 봄 구름 슬 루 스트 스트림 Zipkin 수집기



Spring Cloud Sleuth Stream Zipkin 콜렉터를 시작하려면 의존성을 추가하기 `spring-cloud-sleuth-zipkin-stream` 만하면된다.





메이븐



    <dependencyManagement> (1)
          <dependencies>
              <dependency>
                  <groupId>org.springframework.cloud</groupId>
                  <artifactId>spring-cloud-dependencies</artifactId>
                  <version>Brixton.RELEASE</version>
                  <type>pom</type>
                  <scope>import</scope>
              </dependency>
          </dependencies>
    </dependencyManagement>

    <dependency> (2)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-sleuth-zipkin-stream</artifactId>
    </dependency>
    <dependency> (3)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-starter-sleuth</artifactId>
    </dependency>
    <!-- EXAMPLE FOR RABBIT BINDING -->
    <dependency> (4)
        <groupId>org.springframework.cloud</groupId>
        <artifactId>spring-cloud-stream-binder-rabbit</artifactId>
    </dependency>







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-sleuth-zipkin-stream`

3.  의존성 추가 `spring-cloud-starter-sleuth`- 모든 종속 종속성이 다운로드됩니다.

4.  바인더 (예 : 토끼 바인더)를 추가하여 Spring Cloud Stream에 바인드 할 내용을 지정하십시오.





요람



    dependencyManagement { (1)
        imports {
            mavenBom "org.springframework.cloud:spring-cloud-dependencies:Brixton.RELEASE"
        }
    }

    dependencies {
        compile "org.springframework.cloud:spring-cloud-sleuth-zipkin-stream" (2)
        compile "org.springframework.cloud:spring-cloud-starter-sleuth" (3)
        // Example for Rabbit binding
        compile "org.springframework.cloud:spring-cloud-stream-binder-rabbit" (4)
    }







1.  Spring BOM을 통해 종속성 관리를 추가하면 버전을 직접 선택하지 않기 때문에 훨씬 좋습니다.

2.  의존성 추가 `spring-cloud-sleuth-zipkin-stream`

3.  의존성 추가 `spring-cloud-starter-sleuth`- 모든 종속 종속성이 다운로드됩니다.

4.  바인더 (예 : 토끼 바인더)를 추가하여 Spring Cloud Stream에 바인드 할 내용을 지정하십시오.





메인 클래스에 주석을 달아 주시면 `@EnableZipkinStreamServer`됩니다.









## 추가 리소스





**Marcin Grzejszczak, Spring Cloud Sleuth와 Zipkin에 대해 이야기하기**











[동영상을 보려면 여기를 클릭하십시오.](https://www.youtube.com/watch?v=eQV71Mw1u1c)









## 풍모





*   추적 및 스팬 ID를 Slf4J MDC에 추가하므로 로그 수집기에서 지정된 추적 또는 범위의 모든 로그를 추출 할 수 있습니다. 로그 예 :





    ```2016-02-02 15 : 30 : 57.902 정보 [bar, 6bfd228dc00d216b, 6bfd228dc00d216b, false] 23030 --- [nio-8081-exec-3] ... 2016-02-02 15 : 30 : 58.372 오류 [bar, 6bfd228dc00d216b, 6bfd228dc00d216b, false] 23030 --- [nio-8081-exec-3] ... 2016-02-02 15 : 31 : 01.936 정보 [bar, 46ab0d418373cbc9,46ab0d418373cbc9, false] 23030 --- [nio-8081-exec-4] ...```







    `[appname,traceId,spanId,exportable]`MDC 에서 항목을 확인하십시오.





    *   **spanId** - 발생한 특정 조작의 ID

    *   **appname** - 스팬을 기록한 응용 프로그램의 이름

    *   **traceId** - 스팬이 포함 된 대기 시간 그래프의 ID

    *   **exportable** - 로그를 Zipkin으로 내보낼 지 여부. 언제 스팬을 내보낼 수 없으시겠습니까? Span에서 일부 조작을 랩하고 로그에만 기록하도록하려는 경우.



*   <font class="">트레이스, 스팬 (DAG 형성), 주석, 키 - 값 주석과 같은 일반적인 분산 트레이싱 데이터 모델에 대한 추상화를 제공합니다. 느슨하게 HTrace를 기반으로하지만 Zipkin (Dapper) 호환.

*   Sleuth는 대기 시간 분석을 돕기 위해 타이밍 정보를 기록합니다. sleuth를 사용하면 애플리케이션에서 대기 시간의 원인을 찾아 낼 수 있습니다. Sleuth는 너무 많이 로그하지 않고 프로덕션 애플리케이션을 중단시키지 않기 위해 작성되었습니다.



    *   콜 그래프 (call-graph)에 대한 구조적 데이터를 대역 내에서 전파하고 나머지는 대역 외 (out-of-band)로 전달합니다.

    *   HTTP와 같은 계층의 독창적 인 계측을 포함합니다.

    *   볼륨 관리를위한 샘플링 정책 포함

    *   쿼리 및 시각화를 위해 Zipkin 시스템에보고 할 수 있습니다.



*   Spring 애플리케이션 (서블릿 필터, 비동기 끝점, 나머지 템플리트, 예약 된 액션, 메시지 채널, 필터 필터, 클라이언트)에서 일반적인 입구 및 출구 지점을 측정합니다.

*   Sleuth에는 http 또는 메시징 경계에서 추적에 참여하는 기본 논리가 포함되어 있습니다. 예를 들어 http 전파는 Zipkin 호환 요청 헤더를 통해 작동합니다. 이 전파 로직 정의로 정의된다 `SpanInjector`및 `SpanExtractor`구현.

*   허용 / 삭제 된 기간의 간단한 메트릭을 제공합니다.

*   만약 `spring-cloud-sleuth-zipkin`다음 응용 프로그램은 생성과 지프 킨 호환 트레이스를 수집합니다. 기본적으로 HTTP를 통해 로컬 호스트의 Zipkin 서버 (포트 9411)로 보냅니다. 를 사용하여 서비스의 위치를 ​​구성하십시오 `spring.zipkin.baseUrl`.

*   만약 `spring-cloud-sleuth-stream`다음 응용 프로그램은 생성을 통해 추적을 수집 [봄 클라우드 스트림](https://github.com/spring-cloud/spring-cloud-stream) . 귀하의 앱은 자동으로 귀하의 중개인 (예 : RabbitMQ, Apache Kafka, Redis)을 통해 전송되는 추적자 메시지의 제작자가됩니다.













중대한

Zipkin 또는 Stream을 사용하는 경우 내보내는 범위의 비율 `spring.sleuth.sampler.percentage` (기본값 0.1, 즉 10 %)을 구성합니다. **그렇지 않으면 Sleuth가 작동하지 않는다고 생각할 수 있습니다. 일부 기간을 생략했기 때문입니다.**|



















노트

SLF4J MDC가 항상 설정되고 로그백 사용자는 위 예제에 따라 로그에서 추적 및 스팬 ID를 즉시 보게됩니다. 다른 로깅 시스템은 동일한 결과를 얻으려면 자체 포맷터를 구성해야합니다. 기본이되는 `logging.pattern.level`설정 `%clr(%5p) %clr([${spring.application.name:},%X{X-B3-TraceId:-},%X{X-B3-SpanId:-},%X{X-Span-Export:-}]){yellow}` (이 logback 사용자를위한 봄 부팅 기능입니다). **즉, SLF4J를 사용하지 않을 경우이 패턴이 자동으로 적용되지 않습니다** .|















## 견본 추출





분산 형 추적에서는 데이터 볼륨이 매우 높을 수 있으므로 샘플링이 중요 할 수 있습니다 (일반적으로 발생하는 상황을 파악하기 위해 모든 기간을 내보낼 필요가 없습니다). Spring Cloud Sleuth는 `Sampler`샘플링 알고리즘을 제어하기 위해 구현할 수 있는 전략을 가지고 있습니다. 샘플러는 스팬 (상관) ID가 생성되는 것을 중지하지 않지만 첨부 및 내보내기되는 태그 및 이벤트를 방지합니다. 기본적으로 스팬이 이미 활성화되어 있지만 새로운 스팬이 항상 내보낼 수없는 것으로 표시되면 계속 추적하는 전략을 얻습니다. 모든 응용 프로그램이이 샘플러로 실행되면 로그에 추적이 표시되지만 원격 저장소에는 추적이 표시되지 않습니다. 테스트를 위해 기본값이 충분하기 때문에 로그 만 사용하는 경우 (예 : ELK 애그리 게이터와 함께) 필요할 수도 있습니다. span 데이터를 Zipkin 또는 Spring Cloud Stream으로 내보내는 경우,`AlwaysSampler``PercentageBasedSampler`













노트

은 `PercentageBasedSampler`당신이 사용하는 경우 기본이다 `spring-cloud-sleuth-zipkin`나 `spring-cloud-sleuth-stream`. 를 사용하여 내보내기를 구성 할 수 있습니다 `spring.sleuth.sampler.percentage`. 전달 된 값은 이중 있어야 `0.0`에 `1.0`이 비율하지 그래서. 이전 버전과의 호환성을 위해 속성 이름을 변경하지 않습니다.|











샘플러는 bean 정의를 생성하는 것만으로 설치 될 수 있습니다.







    @Bean
    public Sampler defaultSampler() {
        return new AlwaysSampler();
    }











## 수단





Spring Cloud Sleuth는 모든 Spring 애플리케이션을 자동으로 인스트루먼트하므로, 활성화하려면 아무 것도하지 않아도됩니다. 계측은 사용 가능한 스택에 따라 다양한 기술을 사용하여 추가됩니다. 예를 들어 우리가 사용하는 서블릿 웹 응용 프로그램과 우리가 사용하는 `Filter`스프링 통합에 사용할 수 있습니다 `ChannelInterceptors`.





span 태그에 사용되는 키를 사용자 정의 할 수 있습니다. 범위 데이터의 양을 제한하기 위해 기본적으로 HTTP 요청에는 상태 코드, 호스트 및 URL과 같은 소수의 메타 데이터 만 태그가 지정됩니다. 구성 `spring.sleuth.keys.http.headers`(헤더 이름 목록)을 통해 요청 헤더를 추가 할 수 있습니다 .













노트

태그는 태그 `Sampler`를 허용하고 있는 경우에만 수집되고 내보내집니다 (기본적으로 태그 가 없기 때문에 무언가를 구성하지 않으면 실수로 너무 많은 데이터를 수집 할 위험이 없습니다).|



















노트

현재 Spring Cloud Sleuth의 도구는 열심입니다. 즉, 우리는 스레드간에 추적 컨텍스트를 능동적으로 전달하려고합니다. 또한 타이밍 이벤트는 추적 시스템이 추적 시스템으로 데이터를 내보내지 않는 경우에도 캡처됩니다. 이 접근 방식은 앞으로이 문제에 대해 게으른쪽으로 바뀔 수 있습니다.|















## 수명주기





당신은에 의해 스팬에 다음과 같은 작업을 수행 할 수 있습니다 **org.springframework.cloud.sleuth.Tracer의** 인터페이스 :





*   [시작](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#creating-and-closing-spans) - 스팬을 시작하면 스팬의 이름이 지정되고 시작 타임 스탬프가 기록됩니다.

*   [가까운](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#creating-and-closing-spans) - 스팬이 완료됩니다 (스팬의 종료 시간이 기록) 및 스팬 인 경우 **내보낼** 다음은 지프 킨에 컬렉션을받을 수 있습니다. 스팬은 현재 스레드에서 제거됩니다.

*   [continue](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#continuing-spans) - 스팬의 새로운 인스턴스가 생성되는 반면, [지속](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#continuing-spans) 되는 인스턴스의 복사본이됩니다.

*   [detach](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#continuing-spans) - 스팬이 중지되거나 닫히지 않습니다. 현재 스레드에서만 제거됩니다.

*   [명시 적 부모로 작성](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#creating-spans-with-explicit-parent) - 새 범위를 작성하고 명시 적 상위를 설정할 수 있습니다













팁

Spring은 `Tracer`당신 을 위한 인스턴스를 생성한다 . 그것을 사용하기 위해서는 당신이 필요로하는 모든 것은 단지 그것을 자동 배선하는 것입니다.|











### 범위 생성 및 닫기



**추적기** 인터페이스 를 사용하여 수동으로 기간을 생성 할 수 있습니다 .







    // Start a span. If there was a span present in this thread it will become
    // the `newSpan`'s parent.
    Span newSpan = this.tracer.createSpan("calculateTax");
    try {
        // ...
        // You can tag a span
        this.tracer.addTag("taxValue", taxValue);
        // ...
        // You can log an event on a span
        newSpan.logEvent("taxCalculated");
    } finally {
        // Once done remember to close the span. This will allow collecting
        // the span to send it to Zipkin
        this.tracer.close(newSpan);
    }







이 예제에서 span의 새 인스턴스를 만드는 방법을 볼 수 있습니다. 이 thread에 이미 스팬이 있다고 가정하면, 그 스팬의 부모가됩니다.













중대한

스팬을 만든 후에는 항상 청소하십시오! Zipkin으로 보내려면 범위를 닫는 것을 잊지 마십시오.|













### 계속되는 범위



때로는 새 범위를 만들지 않고 계속 유지하려고합니다. 그러한 상황의 예는 (물론 모든 것이 유스 케이스에 달려있다) :





*   **AOP** - 애스펙트에 도달하기 전에 스팬이 이미 존재하는 경우, 새로운 스팬을 작성하고 싶지 않을 가능성이 있습니다.

*   **Hystrix** - Hystrix 명령을 실행하는 것이 현재 처리의 논리적 부분 일 가능성이 큽니다. 사실, 기술 구현의 세부 사항만으로 별도의 존재로 추적 할 필요는 없습니다.





계속되는 span의 인스턴스는, 계속되는 인스턴스와 같습니다.







    Span continuedSpan = this.tracer.continueSpan(spanToContinue);
    assertThat(continuedSpan).isEqualTo(spanToContinue);







범위를 계속하려면 **추적기** 인터페이스 를 사용할 수 있습니다 .







    // let's assume that we're in a thread Y and we've received
    // the `initialSpan` from thread X
    Span continuedSpan = this.tracer.continueSpan(initialSpan);
    try {
        // ...
        // You can tag a span
        this.tracer.addTag("taxValue", taxValue);
        // ...
        // You can log an event on a span
        continuedSpan.logEvent("taxCalculated");
    } finally {
        // Once done remember to detach the span. That way you'll
        // safely remove it from the current thread without closing it
        this.tracer.detach(continuedSpan);
    }















중대한

스팬을 만든 후에는 항상 청소하십시오! 하나의 스레드 (예 : 스레드 X)에서 시작된 작업과 다른 스레드 (예 : Y, Z)가 완료 될 때까지 기다리는 작업이있는 경우 스팬을 분리하는 것을 잊지 마십시오. 그런 다음 작업 Y, Z의 스팬은 작업이 끝나면 분리해야합니다. 결과가 수집되면 스레드 X의 스팬을 닫아야합니다.|













### 명시 적 상위가있는 범위 생성



새로운 범위를 시작하고 해당 범위의 명시적인 부모를 제공하려는 가능성이 있습니다. 스팬의 부모가 한 스레드에 있고 다른 스레드에서 새 스팬을 시작한다고 가정 해 봅시다. `startSpan`의 방법 `Tracer`인터페이스는 당신이 찾고있는 방법입니다.







    // let's assume that we're in a thread Y and we've received
    // the `initialSpan` from thread X. `initialSpan` will be the parent
    // of the `newSpan`
    Span newSpan = this.tracer.createSpan("calculateCommission", initialSpan);
    try {
        // ...
        // You can tag a span
        this.tracer.addTag("commissionValue", commissionValue);
        // ...
        // You can log an event on a span
        newSpan.logEvent("commissionCalculated");
    } finally {
        // Once done remember to close the span. This will allow collecting
        // the span to send it to Zipkin. The tags and events set on the
        // newSpan will not be present on the parent
        this.tracer.close(newSpan);
    }















중대한

그런 범위를 창조 한 후에 그것을 닫는 것을 기억하십시오. 그렇지 않으면 닫으려는 스레드가 아닌 현재 스레드에 스팬이 있다는 사실과 관련된 많은 경고가 로그에 표시됩니다. 스파크가 제대로 닫히지 않으면 Zipkin에 수집되지 않습니다.|

















## 범위 이름 지정





스팬 이름을 선택하는 것은 쉬운 일이 아닙니다. 스팬 이름은 작업 이름을 나타내야합니다. 이름은 하위 카디널리티 (예 : 식별자 포함 안 함) 여야합니다.





계측기가 많기 때문에 스팬 이름 중 일부는 다음과 같이 인공적입니다.





*   `controller-method-name` 컨트롤러가 메소드 이름으로 수신 한 경우 `conrollerMethodName`

*   `async`포장을 통해 이루어 비동기 작업에 `Callable`와 `Runnable`.

*   `@Scheduled` 주석 첨부 메소드는, 클래스의 단순 명을 돌려줍니다.





다행히도 비동기 처리의 경우 명시 적 명명을 제공 할 수 있습니다.





### @SpanName 주석



어노테이션을 통해 스팬의 이름을 명시 적으로 지정할 수 있습니다 `@SpanName`.







    @SpanName("calculateTax")
    class TaxCountingRunnable implements Runnable {

        @Override public void run() {
            // perform logic
        }
    }







이 경우 다음과 같은 방식으로 처리됩니다.







    Runnable runnable = new TraceRunnable(tracer, spanNamer, new TaxCountingRunnable());
    Future<?> future = executorService.submit(runnable);
    // ... some additional logic ...
    future.get();







스팬의 이름이 지정 `calculateTax`됩니다.







### toString () 메서드



`Runnable`또는 에 대해 별도의 클래스를 만드는 것은 거의 `Callable`없습니다. 일반적으로 이러한 클래스의 익명 인스턴스를 만듭니다. 이러한 클래스에 주석을 달아 주석을 재정의 할 수는 없습니다. 주석이없는 `@SpanName`경우 클래스에 `toString()`메소드 의 사용자 정의 구현이 있는지 확인하고 있습니다 .





그래서 그러한 코드를 실행하는 것 :







    Runnable runnable = new TraceRunnable(tracer, spanNamer, new Runnable() {
        @Override public void run() {
            // perform logic
        }

        @Override public String toString() {
            return "calculateTax";
        }
    });
    Future<?> future = executorService.submit(runnable);
    // ... some additional logic ...
    future.get();







라는 이름의 스팬을 만듭니다 `calculateTax`.











## 사용자 지정





덕분에 스팬이 생성되고 전파되는 방식 `SpanInjector`을 `SpanExtractor`사용자 정의 할 수 있습니다.





현재 프로세스간에 추적 정보를 전달하는 두 가지 기본 제공 방법이 있습니다.





*   봄 통합을 통해

*   HTTP를 통해





Span ID는 Zipkin 호환 (B3) 헤더 ( `Message` HTTP 헤더 중 하나)에서 추출 되어 기존 추적을 시작하거나 결합합니다. 다음 홉이 추출 할 수 있도록 추적 정보가 모든 아웃 바운드 요청에 주입됩니다.





### 스프링 통합



Spring Integration의 경우, 이들은 a에서 Span을 `Message` 작성 `MessageBuilder`하고 추적 정보를 채우는 bean입니다.







    @Bean
    public SpanExtractor<Message> messagingSpanExtractor() {
        ...
    }

    @Bean
    public SpanInjector<MessageBuilder> messagingSpanInjector() {
        ...
    }







자신 만의 `@Primary`구현을 제공하고 bean 정의 에 주석을 추가하여 재정의 할 수 있습니다.







### HTTP



HTTP의 경우 이들은 a에서 Span을 생성하는 bean `HttpServletRequest`입니다.







    @Bean
    public SpanExtractor<HttpServletRequest> httpServletRequestSpanExtractor() {
        ...
    }







자신 만의 `@Primary`구현을 제공하고 bean 정의 에 주석을 추가하여 재정의 할 수 있습니다.







### 예



표준 Zipkin 호환 추적 HTTP 헤더 이름 대신





*   추적 ID에 대한 - `correlationId`

*   span id - `mySpanId`





이것은의 예입니다. `SpanExtractor`







    static class CustomHttpServletRequestSpanExtractor
            implements SpanExtractor<HttpServletRequest> {

        @Override
        public Span joinTrace(HttpServletRequest carrier) {
            long traceId = Span.hexToId(carrier.getHeader("correlationId"));
            long spanId = Span.hexToId(carrier.getHeader("mySpanId"));
            // extract all necessary headers
            Span.SpanBuilder builder = Span.builder().traceId(traceId).spanId(spanId);
            // build rest of the Span
            return builder.build();
        }
    }







그러면 다음과 같이 등록 할 수 있습니다.







    @Bean
    @Primary
    SpanExtractor<HttpServletRequest> customHttpServletRequestSpanExtractor() {
        return new CustomHttpServletRequestSpanExtractor();
    }







Spring Cloud Sleuth는 보안상의 이유로 Http Response에 추적 / 스팬 관련 헤더를 추가하지 않습니다. 헤더가 필요한 경우 헤더 `SpanInjector` 응답을 HTTP 응답에 삽입 하는 사용자 정의 와이를 사용하는 서블릿 필터를 다음과 같이 추가 할 수 있습니다.







    static class CustomHttpServletResponseSpanInjector
            implements SpanInjector<HttpServletResponse> {

        @Override
        public void inject(Span span, HttpServletResponse carrier) {
            carrier.addHeader(Span.TRACE_ID_NAME, span.traceIdString());
            carrier.addHeader(Span.SPAN_ID_NAME, Span.idToHex(span.getSpanId()));
        }
    }

    static class HttpResponseInjectingTraceFilter extends GenericFilterBean {

        private final Tracer tracer;
        private final SpanInjector<HttpServletResponse> spanInjector;

        public HttpResponseInjectingTraceFilter(Tracer tracer, SpanInjector<HttpServletResponse> spanInjector) {
            this.tracer = tracer;
            this.spanInjector = spanInjector;
        }

        @Override
        public void doFilter(ServletRequest request, ServletResponse servletResponse, FilterChain filterChain) throws IOException, ServletException {
            HttpServletResponse response = (HttpServletResponse) servletResponse;
            Span currentSpan = this.tracer.getCurrentSpan();
            this.spanInjector.inject(currentSpan, response);
            filterChain.doFilter(request, response);
        }
    }







그러면 다음과 같이 등록 할 수 있습니다.







    @Bean
    SpanInjector<HttpServletResponse> customHttpServletResponseSpanInjector() {
        return new CustomHttpServletResponseSpanInjector();
    }

    @Bean
    HttpResponseInjectingTraceFilter responseInjectingTraceFilter(Tracer tracer) {
        return new HttpResponseInjectingTraceFilter(tracer, customHttpServletResponseSpanInjector());
    }









### Zipkin의 맞춤 SA 태그



때로는 인스트루먼트되지 않은 외부 서비스로 호출을 래핑하는 수동 Span을 생성하려고합니다. 할 수있는 일은 `peer.service`호출하려는 서비스의 값을 포함 할 태그가 있는 범위를 만드는 것입니다. 아래에서 그러한 범위에 래핑 된 Redis 통화에 대한 예를 볼 수 있습니다.







    org.springframework.cloud.sleuth.Span newSpan = tracer.createSpan("redis");
    try {
        newSpan.tag("redis.op", "get");
        newSpan.tag("lc", "redis");
        newSpan.logEvent(org.springframework.cloud.sleuth.Span.CLIENT_SEND);
        // call redis service e.g
        // return (SomeObj) redisTemplate.opsForHash().get("MYHASH", someObjKey);
    } finally {
        newSpan.tag("peer.service", "redisService");
        newSpan.tag("peer.ipv4", "1.2.3.4");
        newSpan.tag("peer.port", "1234");
        newSpan.logEvent(org.springframework.cloud.sleuth.Span.CLIENT_RECV);
        tracer.close(newSpan);
    }















중대한

`peer.service`태그와 태그를 모두 추가하지 않도록하십시오 `SA`! 추가 만해야합니다 `peer.service`.|













### 사용자 지정 서비스 이름



기본적으로 Sleuth는 Zipkin에 스팬을 보내면 스팬의 서비스 이름이 `spring.application.name`value 와 같을 것이라고 가정 합니다. <font class="">그것은 항상 그런 경우는 아니지만. 응용 프로그램에서 오는 모든 기간에 대해 다른 서비스 이름을 명시 적으로 제공하려는 경우가 있습니다. 이를 달성하려면 응용 프로그램에 다음 속성을 전달하여 해당 값을 재정의하면 충분합니다 ( `foo`서비스 이름 예 ).







    spring.zipkin.service.name: foo













## 메시지를 메시지로 확장





jar를 의존성으로 포함하고 Channel Binder 구현을 추가함으로써 [Spring Cloud Stream](http://cloud.spring.io/spring-cloud-stream) 을 통해 스팬 데이터를 축적하고 보낼 수 있습니다 `spring-cloud-sleuth-stream`(예 : `spring-cloud-starter-stream-rabbit`RabbitMQ 또는 `spring-cloud-starter-stream-kafka`Kafka의 경우). 이렇게하면 자동으로 앱이 페이로드 유형의 메시지 생성자로 바뀝니다 `Spans`.





### Zipkin 소비자



Span 데이터에 대한 메시지 소비자를 설정하고 Zipkin으로 푸시하기위한 특수 편의 주석이 `SpanStore`있습니다. 이 신청서







    @SpringBootApplication
    @EnableZipkinStreamServer
    public class Consumer {
        public static void main(String[] args) {
            SpringApplication.run(Consumer.class, args);
        }
    }







Spring Cloud Stream을 통해 제공하는 모든 전송에 대한 Span 데이터를 수신합니다 `Binder`(예 : `spring-cloud-starter-stream-rabbit`RabbitMQ 포함 ). Redis와 Kafka의 유사한 시작 자가 존재합니다. 다음 UI 종속성을 추가하면







    <groupId>io.zipkin.java</groupId>
    <artifactId>zipkin-autoconfigure-ui</artifactId>







그런 다음 , 포트 9411에 UI와 API를 호스팅 하는 [Zipkin 서버를](https://github.com/openzipkin/zipkin) 앱에 [설치하게됩니다](https://github.com/openzipkin/zipkin) .





기본값 `SpanStore`은 메모리에 있습니다 (데모 및 빠른 시작에 좋습니다). 보다 견고한 솔루션을 `spring-boot-starter-jdbc`위해 MySQL과 클래스 패스를 추가하고 구성 을 `SpanStore`통해 JDBC 를 활성화 할 수 있습니다 ( 예 :







    spring:
      rabbitmq:
        host: ${RABBIT_HOST:localhost}
      datasource:
        schema: classpath:/mysql.sql
        url: jdbc:mysql://${MYSQL_HOST:localhost}/test
        username: root
        password: root
    # Switch this on to create the schema on startup:
        initialize: true
        continueOnError: true
      sleuth:
        enabled: false
    zipkin:
      storage:
        type: mysql















노트

또한 `@EnableZipkinStreamServer`이 주석은 주석으로 `@EnableZipkinServer`처리되어 HTTP를 통해 범위를 수집하고 Zipkin 웹 UI에서 쿼리하는 표준 Zipkin 서버 끝점을 노출합니다.|













### 맞춤형 소비자



커스텀 소비자는 또한를 사용하여 쉽게 구현 `spring-cloud-sleuth-stream`되고 바인딩 될 수 `SleuthSink`있습니다. 예:







    @EnableBinding(SleuthSink.class)
    @SpringBootApplication(exclude = SleuthStreamAutoConfiguration.class)
    @MessageEndpoint
    public class Consumer {

        @ServiceActivator(inputChannel = SleuthSink.INPUT)
        public void sink(Spans input) throws Exception {
            // ... process spans
        }
    }















노트

위의 샘플 소비자 애플리케이션은 명시 적으로 제외 `SleuthStreamAutoConfiguration`되므로 자체적으로 메시지를 보내지 않지만 선택 사항입니다 (실제로 소비자 애플리케이션으로 요청을 추적하려고 할 수 있습니다).|

















## 측정 항목





현재 Spring Cloud Sleuth는 범위와 관련된 매우 간단한 메트릭을 등록합니다. [스프링 부트의 메트릭 지원](http://docs.spring.io/spring-boot/docs/current/reference/html/production-ready-metrics.html#production-ready-recording-metrics) 을 사용하여 수용 및 삭제 된 스팬의 수를 계산합니다. 스팬이 Zipkin으로 전송 될 때마다 허용 범위가 늘어납니다. 오류가있는 경우 삭제 된 기간의 수가 증가합니다.









## 통합





### 실행 가능 및 호출 가능



만약 당신이 당신의 논리를 감싸고 있다면, `Runnable`또는 `Callable`그것들을 그들의 Sleuth 대 표로 포장하기에 충분합니다.





예 `Runnable`:







    Runnable runnable = new Runnable() {
        @Override
        public void run() {
            // do some work
        }

        @Override
        public String toString() {
            return "spanNameFromToStringMethod";
        }
    };
    // Manual `TraceRunnable` creation with explicit "calculateTax" Span name
    Runnable traceRunnable = new TraceRunnable(tracer, spanNamer, runnable, "calculateTax");
    // Wrapping `Runnable` with `Tracer`. The Span name will be taken either from the
    // `@SpanName` annotation or from `toString` method
    Runnable traceRunnableFromTracer = tracer.wrap(runnable);







예 `Callable`:







    Callable<String> callable = new Callable<String>() {
        @Override
        public String call() throws Exception {
            return someLogic();
        }

        @Override
        public String toString() {
            return "spanNameFromToStringMethod";
        }
    };
    // Manual `TraceCallable` creation with explicit "calculateTax" Span name
    Callable<String> traceCallable = new TraceCallable<>(tracer, spanNamer, callable, "calculateTax");
    // Wrapping `Callable` with `Tracer`. The Span name will be taken either from the
    // `@SpanName` annotation or from `toString` method
    Callable<String> traceCallableFromTracer = tracer.wrap(callable);







그렇게하면 각 실행마다 새 Span이 만들어지고 닫히도록 할 수 있습니다.







### Hystrix



#### 커스텀 동시성 전략



우리 [`HystrixConcurrencyStrategy`](https://github.com/Netflix/Hystrix/wiki/Plugins#concurrencystrategy) 는 모든 `Callable`인스턴스를 자신의 Sleuth 담당자에게 랩핑 하는 커스텀 을 등록합니다 `TraceCallable`. Hystrix 명령이 호출되기 전에 추적이 이미 진행되고 있는지 여부에 따라 전략이 시작되거나 지속됩니다. 사용자 지정을 해제하려면 Hystrix 동시성 전략은 설정 `spring.sleuth.hystrix.strategy.enabled`에 `false`.







#### 수동 명령 설정



당신은 다음을 가지고 있다고 가정합니다 `HystrixCommand`:







    HystrixCommand<String> hystrixCommand = new HystrixCommand<String>(setter) {
        @Override
        protected String run() throws Exception {
            return someLogic();
        }
    };







추적 정보를 전달하려면 다음과 같은 Sleuth 버전에서 동일한 논리를 래핑해야 `HystrixCommand`합니다 `TraceCommand`.







    TraceCommand<String> traceCommand = new TraceCommand<String>(tracer, traceKeys, setter) {
        @Override
        public String doRun() throws Exception {
            return someLogic();
        }
    };











### RxJava



우리 [`RxJavaSchedulersHook`](https://github.com/ReactiveX/RxJava/wiki/Plugins#rxjavaschedulershook) 는 모든 `Action0`인스턴스를 자신의 Sleuth 담당자에게 랩핑 하는 커스텀 을 등록합니다 `TraceAction`. 후크는 동작이 예약되기 전에 이미 추적이 진행되고 있는지 여부에 따라 기간을 시작하거나 지속합니다. 사용자 지정을 해제하려면 RxJavaSchedulersHook는 설정 `spring.sleuth.rxjava.schedulers.hook.enabled`에 `false`.





Span을 생성하지 않으려는 스레드 이름에 대한 정규 표현식 목록을 정의 할 수 있습니다. `spring.sleuth.rxjava.schedulers.ignoredthreads`속성 에 쉼표로 구분 된 정규 표현식 목록을 제공하기 만하면됩니다 .







### HTTP 통합



이 섹션의 기능은 `spring.sleuth.web.enabled`속성에 값 을 제공하여 비활성화 할 수 있습니다 `false`.





#### HTTP 필터



비아 `TraceFilter`모든 샘플 들어오는 요청 스팬의 생성 결과. Span의 이름은 `http:`요청을 보낸 경로입니다. 예를 들어 요청이 전송 된 `/foo/bar`경우 이름이됩니다 `http:/foo/bar`. `spring.sleuth.web.skipPattern`속성 을 통해 건너 뛸 URI를 구성 할 수 있습니다 . 당신은 할 경우 `ManagementServerProperties`다음 클래스 패스의 값 `contextPath`제공된 스킵 패턴에 추가됩니다합니다.







#### HandlerInterceptor



우리가 span 이름을 정확하기를 원하기 때문에, 우리 `TraceHandlerInterceptor`는 기존 의 것을 감싸거나 기존 `HandlerInterceptor`의리스트에 직접 추가되는 것을 사용합니다 `HandlerInterceptors`. The `TraceHandlerInterceptor`는 주어진 요청에 특별한 요청 속성을 추가합니다 `HttpServletRequest`. 하여이 경우 `TraceFilter`표시되지 않습니다이 속성은 추적이 UI에 제대로 표시되도록 서버 측에서 만든 추가 분리하는 "대체"범위를 만듭니다 설정합니다. 대부분의 가능성이 있다는 것은 장비가 누락되었음을 나타냅니다. 이 경우 Spring Cloud Sleuth에서 문제를 제기하십시오.







#### 비동기 서블릿 지원



컨트롤러가 Spring Cloud `Callable`또는 `WebAsyncTask`Spring Cloud를 반환하면 Sleuth는 새로운 하나를 생성하는 대신 기존의 범위를 계속 유지합니다.









### HTTP 클라이언트 통합



#### 동기 휴지통 템플릿



우리는 `RestTemplate`모든 추적 정보가 요청에 전달되도록하는 인터셉터를 삽입하고 있습니다. 전화가 걸려 올 때마다 새 Span이 만들어집니다. 응답을 받으면 닫힙니다. 동기 차단하기 위해 `RestTemplate`단지 설정 기능 `spring.sleuth.web.client.enabled`을을 `false`.













중대한

`RestTemplate`인터셉터가 주입되도록 빈 으로 등록 해야합니다. 키워드 로 `RestTemplate`인스턴스 를 생성 `new`하면 도구가 작동하지 않습니다.|













#### 비동기 나머지 템플릿











중대한

추적 된 버전의 `AsyncRestTemplate`bean이 사용자를 위해 즉시 등록됩니다. 자신의 bean을 가지고 있다면 그것을 표현으로 포장해야 `TraceAsyncRestTemplate`합니다. 가장 좋은 해결책은 `ClientHttpRequestFactory`및 / 또는을 (를) 사용자 지정하는 것 `AsyncClientHttpRequestFactory`입니다. **자신 만의 것이 `AsyncRestTemplate`있고 그것을 포장하지 않으면 귀하의 전화가 추적되지 않습니다** .|











사용자 지정 계측은 요청을 보내고받을 때 범위를 만들고 닫도록 설정됩니다. bean을 등록하여 `ClientHttpRequestFactory` and를 사용자 정의 할 수 있습니다 `AsyncClientHttpRequestFactory`. (예를 들어 포장하는 것을 잊지 마세요 호환 구현을 추적 사용해야합니다 `ThreadPoolTaskScheduler`A의 `TraceAsyncListenableTaskExecutor`). 사용자 정의 요청 팩토리의 예 :







    @EnableAutoConfiguration
    @Configuration
    public static class TestConfiguration {

        @Bean
        ClientHttpRequestFactory mySyncClientFactory() {
            return new MySyncClientHttpRequestFactory();
        }

        @Bean
        AsyncClientHttpRequestFactory myAsyncClientFactory() {
            return new MyAsyncClientHttpRequestFactory();
        }
    }







블록에 `AsyncRestTemplate`설정 한 기능 `spring.sleuth.web.async.client.enabled`에를 `false`. 기본 생성하지 않으려면 `TraceAsyncClientHttpRequestFactoryWrapper`세트 `spring.sleuth.web.async.client.factory.enabled` 에를 `false`. 당신은 생성하지 않으려면 `AsyncRestClient`모든 설정 `spring.sleuth.web.async.client.template.enabled`에 `false`.









### 기소하다



기본적으로 Spring Cloud Sleuth는를 통해 feign과의 통합을 제공합니다 `TraceFeignClientAutoConfiguration`. `spring.sleuth.feign.enabled`false 로 설정하면 완전히 비활성화 할 수 있습니다 . 당신이 그렇게한다면, Feign 관련 계기는 발생하지 않을 것입니다.





Feign 계측의 일부는을 통해 수행됩니다 `FeignBeanPostProcessor`. `spring.sleuth.feign.processor.enabled`같음을 제공하여 비활성화 할 수 있습니다 `false`. 이렇게 설정하면 Spring Cloud Sleuth는 사용자 지정 Feign 구성 요소를 사용하지 않습니다. 그러나 모든 기본 계측은 여전히있을 것입니다.







### 비동기 통신



#### @Async 주석이 달린 메소드



Spring Cloud Sleuth에서는 비동기 관련 구성 요소를 계측하여 추적 정보가 스레드간에 전달되도록합니다. 의 값을 `spring.sleuth.async.enabled`로 설정하여이 동작을 비활성화 할 수 있습니다 `false`.





메소드에 주석 `@Async`을 달면 다음과 같은 특성을 가진 새로운 Span이 자동으로 생성됩니다.





*   스팬 이름은 주석이 달린 메소드 이름이됩니다.

*   Span은 해당 메소드의 클래스 이름과 메소드 이름으로 태그가 지정됩니다.







#### @Scheduled 주석이 달린 메소드



Spring Cloud Sleuth에서는 스케쥴 된 메소드 실행을 계측하여 추적 정보가 스레드간에 전달되도록합니다. 의 값을 `spring.sleuth.scheduled.enabled`로 설정하여이 동작을 비활성화 할 수 있습니다 `false`.





메소드에 주석 `@Scheduled`을 달면 다음과 같은 특성을 가진 새로운 Span이 자동으로 생성됩니다.





*   스팬 이름은 주석이 달린 메소드 이름이됩니다.

*   Span은 해당 메소드의 클래스 이름과 메소드 이름으로 태그가 지정됩니다.





`@Scheduled`주석이 달린 일부 클래스 에 대해 스팬 만들기를 건너 뛰려면 주석이 달린 클래스 `spring.sleuth.scheduled.skipPattern`의 정규화 된 이름과 일치하는 정규 표현식을 사용하여 설정할 수 있습니다 `@Scheduled`.













팁

당신이 사용하는 경우 `spring-cloud-sleuth-stream`와 `spring-cloud-netflix-hystrix-stream`함께, 스팬 각 Hystrix 메트릭 생성 및 지프 킨로 전송됩니다. 이것은 귀찮을 수 있습니다. 설정을 통해이를 방지 할 수 있습니다.`spring.sleuth.scheduled.skipPattern=org.springframework.cloud.netflix.hystrix.stream.HystrixStreamTask`|













#### Executor, ExecutorService 및 ScheduledExecutorService



우리는 제공하고 `LazyTraceExecutor`, `TraceableExecutorService`하고 `TraceableScheduledExecutorService`. 이러한 구현은 새로운 작업이 제출, 호출 또는 예약 될 때마다 기간을 생성합니다.





여기서 `TraceableExecutorService`작업 할 때 추적 정보를 전달하는 방법의 예를 볼 수 있습니다 `CompletableFuture`.







    CompletableFuture<Long> completableFuture = CompletableFuture.supplyAsync(() -> {
        // perform some logic
        return 1_000_000L;
    }, new TraceableExecutorService(executorService,
            // 'calculateTax' explicitly names the span - this param is optional
            tracer, traceKeys, spanNamer, "calculateTax"));











### 메시지



Spring Cloud Sleuth는 [Spring Integration](http://projects.spring.io/spring-integration/) 과 [통합](http://projects.spring.io/spring-integration/) 됩니다. 게시 및 가입 이벤트의 범위를 만듭니다. Spring Integration 도구를 사용하지 않으려면 `spring.sleuth.integration.enabled`false로 설정하십시오.





스프링 클라우드는 버전 1.0.4가 메시징을 사용할 때 유효하지 않은 추적 헤더를 전송할 때까지 사용되지 않습니다. 이러한 헤더는 실제로 HTTP에서 보낸 `-`이름과 같습니다 (이름에 a 포함 ). 1.0.4의 이전 버전과의 호환성을 위해 유효한 헤더와 유효하지 않은 헤더를 모두 보내기 시작했습니다. 1.0.4로 업그레이드하십시오. Spring Cloud Sleuth 1.1에서는 더 이상 사용되지 않는 헤더에 대한 지원이 제거 될 것이기 때문입니다.





1.0.4부터 `spring.sleuth.integration.patterns`추적을 위해 포함시킬 채널의 이름을 명시 적으로 제공하는 패턴을 제공 할 수 있습니다 . 기본적으로 모든 채널이 포함됩니다.







### 주울



우리는 Zuul 필터를 등록하여 추적 정보를 전파합니다 (요청 헤더는 추적 데이터로 보강되었습니다). Zuul 지원을 비활성화하려면 `spring.sleuth.zuul.enabled`속성을 로 설정하십시오 `false`.











## 예제 실행





[Pivotal Web Services에](https://run.pivotal.io/) 배포 된 실행중인 예제를 찾을 수 있습니다 . 다음 링크에서 확인하십시오.





*   [샘플에 제시된 앱의 Zipkin](https://docssleuth-zipkin-server.cfapps.io/)

*   [PWS에 양조장을위한 Zipkin](https://docsbrewing-zipkin-web.cfapps.io/) , 그것의 [Github 부호](https://github.com/spring-cloud-samples/brewery)







# 봄 구름 영사



이 프로젝트는 자동 환경 설정과 Spring Environment 및 다른 Spring 프로그래밍 모델 관용구에 대한 바인딩을 통해 Spring Boot 애플리케이션을위한 영사 통합을 제공합니다. 몇 가지 간단한 주석을 사용하면 응용 프로그램 내부의 공통 패턴을 신속하게 활성화 및 구성하고 영사 (Consul) 기반 구성 요소로 대규모 분산 시스템을 구축 할 수 있습니다. 제공되는 패턴에는 서비스 발견, 제어 버스 및 구성이 포함됩니다. 지능형 라우팅 (Zuul) 및 클라이언트 측로드 밸런싱 (리본), 회로 차단기 (Hystrix)는 Spring Cloud Netflix와 통합되어 제공됩니다.





## 영사 설치





영사를 설치하는 방법은 설치 [설명서](https://www.consul.io/intro/getting-started/install.html) 를 참조하십시오 .









## 영사 요원





Consul Agent Client는 모든 Spring Cloud Consul 어플리케이션에서 사용할 수 있어야합니다. 기본적으로 에이전트 클라이언트는에 있어야합니다 `localhost:8500`. 에이전트 클라이언트를 시작하는 방법과 Consul Agent Server 클러스터에 연결하는 방법에 대한 자세한 내용은 [에이전트 설명서](https://consul.io/docs/agent/basics.html) 를 참조하십시오 . 개발을 위해 영사를 설치 한 후 다음 명령을 사용하여 영사 대리인을 시작할 수 있습니다 :







```./src/main/bash/local_run_consul.sh```







그러면 포트 8500에서 서버 모드의 에이전트가 시작되고 ui는 [http : // localhost : 8500](http://localhost:8500/) 에서 사용할 수 [있습니다.](http://localhost:8500/)









## 영사를 통한 봉사 활동





서비스 검색은 마이크로 서비스 기반 아키텍처의 핵심 교리 중 하나입니다. 각 클라이언트 또는 일부 형식의 컨벤션을 손으로 구성하려는 것은 매우 어려울 수 있으며 매우 약해질 수 있습니다. Consul은 [HTTP API](https://www.consul.io/docs/agent/http.html) 및 [DNS](https://www.consul.io/docs/agent/dns.html) 를 통해 Service Discovery 서비스를 제공합니다 . Spring Cloud Consul은 서비스 등록 및 발견을 위해 HTTP API를 활용합니다. 이것은 비 스프링 클라우드 애플리케이션이 DNS 인터페이스를 이용하는 것을 방지하지 못한다. Consul Agents 서버는 [가십 프로토콜](https://www.consul.io/docs/internals/gossip.html) 을 통해 [통신](https://www.consul.io/docs/internals/gossip.html) 하고 [뗏목 합의 프로토콜](https://www.consul.io/docs/internals/consensus.html) 을 사용 하는 [클러스터](https://www.consul.io/docs/internals/architecture.html) 에서 실행됩니다 .[](https://www.consul.io/docs/internals/gossip.html)[](https://www.consul.io/docs/internals/consensus.html)





### 영사에 등록하기



클라이언트가 영사관에 ​​등록하면 호스트 및 포트, ID, 이름 및 태그와 같은 자체에 대한 메타 데이터를 제공합니다. 영사가 10 초마다 끝점 에 도달 하는 HTTP [검사](https://www.consul.io/docs/agent/checks.html) 가 기본적으로 만들어집니다 `/health`. 상태 확인에 실패하면 서비스 인스턴스가 위험으로 표시됩니다.





영사 클라이언트의 예 :







    @SpringBootApplication
    @EnableDiscoveryClient
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







(즉, 완전히 정상적인 스프링 부트 응용 프로그램). 영사 클라이언트가 다른 곳에있는 `localhost:8500`경우 클라이언트를 찾으려면 구성이 필요합니다. 예:





application.yml



```봄: 구름: 영사: 호스트 : localhost 포트 : 8500```















주의

[Spring Cloud Consul Config](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-consul-config) 를 사용 하는 경우 위의 값을 `bootstrap.yml`대신에 배치해야합니다 `application.yml`.|











로부터 촬영의 기본 서비스 이름, 인스턴스 ID와 포트, `Environment`이다 `${spring.application.name}`, 스프링 컨텍스트 ID 및 `${server.port}`각각.





`@EnableDiscoveryClient` 앱을 Consul "서비스"(즉, 자체 등록)와 "클라이언트"(즉, Consul에 다른 서비스를 찾기 위해 질의 할 수 있음)로 만듭니다.







### HTTP 상태 확인



Consul 인스턴스의 상태 검사는 기본적으로 Spring Boot Actuator 응용 프로그램에서 유용한 끝점의 기본 위치 인 "/ health"로 검사합니다. 기본값이 아닌 컨텍스트 경로 나 서블릿 경로 (예 `server.servletPath=/foo`:) 또는 관리 끝점 경로 (예 :) 를 사용하는 경우 액추에이터 응용 프로그램의 경우에도 이러한 내용을 변경해야합니다 `management.contextPath=/admin`. 영사가 건강 종점을 확인하기 위해 사용하는 간격도 구성 될 수 있습니다. "10s"및 "1m"은 각각 10 초 및 1 분을 나타냅니다. 예:





application.yml



```봄: 구름: 영사: 발견: healthCheckPath : $ {management.contextPath} / 건강 healthCheckInterval : 15s```







#### 메타 데이터 및 영사 태그



영사는 아직 서비스에 대한 메타 데이터를 지원하지 않습니다. 봄 구름 `ServiceInstance`에는 `Map<String, String> metadata`들판이 있습니다. Spring Cloud Consul은 영사가 공식적으로 메타 데이터를 지원할 때까지 영사 태그를 사용하여 메타 데이터를 추정합니다. 양식 `key=value`이있는 태그 는 분할되어 각각 `Map`키와 값으로 사용됩니다 . 등호가없는 태그 `=`는 키와 값으로 사용됩니다.





application.yml



```봄: 구름: 영사: 발견: 태그 : foo = bar, baz```







위의 구성은 `foo→bar`및 로 맵핑됩니다 `baz→baz`.







#### 총영사관 고유 ID 만들기



기본적으로 영사 인스턴스는 Spring Application Context ID와 동일한 ID로 등록됩니다. 기본적으로 Spring 애플리케이션 컨텍스트 ID는 `${spring.application.name}:comma,separated,profiles:${server.port}`이다. 대부분의 경우 하나의 서비스에 대한 여러 인스턴스가 하나의 시스템에서 실행될 수 있습니다. 더 많은 유일성이 필요하다면, Spring Cloud를 사용하여 고유 한 식별자를 제공함으로써 이것을 오버라이드 할 수있다 `spring.cloud.consul.discovery.instanceId`. 예 :





application.yml



```봄: 구름: 영사: 발견: instanceId : $ {spring.application.name} : $ {spring.application.instance_id : $ {random.value}}```







이 메타 데이터와 localhost에 배포 된 여러 서비스 인스턴스를 사용하면 무작위 값이 인스턴스를 고유하게 만듭니다. Cloudfoundry에서는 `spring.application.instance_id`Spring Boot Actuator 응용 프로그램에 자동으로 채워 지므로 무작위 값은 필요하지 않습니다.









### DiscoveryClient 사용



Spring Cloud는 [Feign](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/docs/src/main/asciidoc/spring-cloud-netflix.adoc#spring-cloud-feign) (REST 클라이언트 빌더)과 물리적 URL 대신 논리적 서비스 이름을 사용하는 [Spring`RestTemplate`](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/docs/src/main/asciidoc/spring-cloud-netflix.adoc#spring-cloud-ribbon) 을 지원한다.





또한 `org.springframework.cloud.client.discovery.DiscoveryClient`Netflix와 관련이없는 검색 클라이언트를위한 간단한 API를 제공하는을 사용할 수도 있습니다.







```@Autowired 개인용 DiscoveryClient discoveryClient;
 public String serviceUrl () { List <ServiceInstance> list = discoveryClient.getInstances ( "STORES"); if (list! = null && list.size ()> 0) { return list.get (0) .getUri (); } null를 돌려 준다. }```













## 영사를 통한 분산 구성





영사는 구성 및 기타 메타 데이터를 저장하기위한 [키 / 값 저장소](https://consul.io/docs/agent/http/kv.html) 를 제공합니다 . Spring Cloud Consul Config는 [Config Server 및 Client](https://github.com/spring-cloud/spring-cloud-config) 의 대안 입니다. 특별한 "부트 스트랩"단계에서 설정은 스프링 환경으로로드됩니다. 구성은 `/config`기본적으로 폴더에 저장 됩니다. `PropertySource`애플리케이션의 이름과 프로퍼티 해석의 Spring Cloud Config 순서를 모방 한 활성 프로파일을 기반으로 다중 인스턴스가 작성된다. 예를 들어, 이름이 "testApp"이고 "dev"프로파일이있는 응용 프로그램에는 다음과 같은 등록 정보 소스가 생성됩니다.







```config / testApp, dev / 구성 / testApp / config / application, dev / config / application /```







가장 구체적인 속성 소스는 맨 위에 있으며 가장 구체적인 것은 맨 아래에 있습니다. Properties는 구성을 위해 `config/application`consul을 사용하는 모든 응용 프로그램에 적용 가능한 폴더입니다. 의 속성 `config/testApp`폴더 "TestApp가"라는 이름의 서비스의 인스턴스에서만 사용할 수 있습니다.





구성은 현재 응용 프로그램 시작시 읽습니다. HTTP POST를 보내면 구성 `/refresh`이 다시로드됩니다. 영사가 지원하는 핵심 가치 저장소를 시청하는 것은 현재 가능하지 않지만이 프로젝트의 향후 추가 사항입니다.





### 활성화 방법



의존성을 포함하면 `org.springframework.cloud:spring-cloud-consul-config`Spring Cloud Consul Config를 설정할 자동 구성이 가능합니다.







### 커스터마이징



영사 구성은 다음 속성을 사용하여 사용자 정의 할 수 있습니다.





bootstrap.yml



```봄: 구름: 영사: config : enabled : true 접두사 : 구성 defaultContext : apps profileSeparator : '::'```







*   `enabled` 이 값을 "false"로 설정하면 영사 구성이 비활성화됩니다.

*   `prefix` 구성 값의 기본 폴더를 설정합니다.

*   `defaultContext` 모든 응용 프로그램에서 사용하는 폴더 이름을 설정합니다.

*   `profileSeparator` 속성 소스의 프로필 이름과 프로필을 구분하는 데 사용되는 구분 기호의 값을 설정합니다.











## 구성이있는 YAML 또는 등록 정보





개별 키 / 값 쌍과 대조적으로 YAML 또는 속성 형식의 속성 집합을 저장하는 것이 더 편리 할 수 ​​있습니다. 또는로 `spring.cloud.consul.config.format`속성을 설정하십시오 . YAML을 사용하는 예를 들면 다음과 같습니다.`YAML``PROPERTIES`





bootstrap.yml



```봄: 구름: 영사: config : 형식 : YAML```







YAML은 `data`영사 의 적절한 열쇠에 있어야합니다 . 키 위의 기본값을 사용하면 다음과 같습니다.







```config / testApp, dev / data config / testApp / data config / application, dev / data config / application / data```







위에 나열된 키 중 하나에 YAML 문서를 저장할 수 있습니다.





를 사용하여 데이터 키를 변경할 수 있습니다 `spring.cloud.consul.config.data-key`.









## 구성이있는 git2consul





git2consul은 영사체 프로젝트에서 영창 저장소에서 개별 키를 영사에로드하는 프로젝트입니다. 기본적으로 키 이름은 파일 이름입니다. YAML 및 Properties 파일은 및의 파일 확장자로 `.yml`각각 `.properties`지원됩니다. 에 `spring.cloud.consul.config.format`속성을 설정하십시오 `FILES`. 예 :





bootstrap.yml



```봄: 구름: 영사: config : 형식 : 파일```







에서 다음 키를 감안할 `/config`의 `development`프로파일 및 응용 프로그램의 이름은 `foo`:







```.gitignore application.yml bar.properties foo-development.properties foo-production.yml foo.properties master.ref```







다음 속성 소스가 생성됩니다.







```config / foo-development.properties config / foo.properties config / application.yml```







각 키의 값은 올바르게 형식화 된 YAML 또는 특성 파일이어야합니다.









## 실패 빠른





영사를 구성 할 수없는 경우 특정 상황 (예 : 지역 개발 또는 특정 테스트 시나리오)이 실패하지 않는 것이 편리 할 수 ​​있습니다. 설정 `spring.cloud.consul.config.failFast=false`에서하면 `bootstrap.yml`구성 모듈은 경고를 기록보다는 예외가 발생하게됩니다. 이렇게하면 응용 프로그램이 정상적으로 시작될 수 있습니다.









## 영사 재 시도





영사 대리인이 앱을 시작할 때 때때로 사용할 수 없을 것으로 예상되는 경우 실패 후 계속 시도하도록 요청할 수 있습니다. 당신은 추가해야 `spring-retry`하고 `spring-boot-starter-aop`클래스 경로에. 기본 동작은 1000ms의 초기 백 오프 간격과 후속 백 오프의 지수 배율 1.1로 6 회 재 시도하는 것입니다. 구성 등록 정보를 사용하여 이러한 등록 정보 (및 기타 등록 정보)를 `spring.cloud.consul.retry.*`구성 할 수 있습니다 . 이는 Spring Cloud Consul Config와 Discovery 등록 모두에서 작동합니다.













팁

재시도를 완전히 제어하려면 id가 "consulRetryInterceptor" `@Bean`인 유형 `RetryOperationsInterceptor`을 추가하십시오 . Spring Retry에는 `RetryInterceptorBuilder`쉽게 재사용 할 수 있는 재 시도가 있습니다.|















## 영사가있는 봄 구름 버스





나중에 출시됩니다.









## Hystrix가있는 회로 차단기





응용 프로그램은 Spring Cloud Netflix 프로젝트에서 제공하는 Hystrix 회로 차단기를이 pter.xml 프로젝트에 포함하여 사용할 수 있습니다 `spring-cloud-starter-hystrix`. Hystrix는 Netflix Discovery Client에 의존하지 않습니다. `@EnableHystrix`주석은 구성 클래스 (일반적으로 기본 클래스)에 배치해야합니다. 그런 다음 `@HystrixCommand`회로 차단기로 보호 할 수 있도록 주석을 달 수 있습니다 . 자세한 내용 [은 설명서](http://projects.spring.io/spring-cloud/spring-cloud.html#_circuit_breaker_hystrix_clients) 를 참조하십시오.









## Turbine 및 Consul과의 Hystrix 메트릭 집합





터빈 (Spring Cloud Netflix 프로젝트에서 제공)은 여러 인스턴스의 Hystrix 메트릭 스트림을 집계하므로 대시 보드는 집계 뷰를 표시 할 수 있습니다. Turbine은 `DiscoveryClient`인터페이스를 사용하여 관련 인스턴스를 조회합니다. Spring Cloud Consul과 함께 Turbine을 사용하려면 다음 예제와 비슷한 방법으로 Turbine 응용 프로그램을 구성하십시오.





pom.xml



```<의존성> <groupId> org.springframework.cloud </ groupId> <artifactId> spring-cloud-netflix-turbine </ artifactId> </ dependency> <의존성> <groupId> org.springframework.cloud </ groupId> <artifactId> spring-cloud-starter-consul-discovery </ artifactId> </ dependency>```







터빈 의존성은 시동기가 아닙니다. 터빈 스타터에는 Netflix Eureka가 지원됩니다.





application.yml



```spring.application.name : 터빈 응용 프로그램 : consulhystrixclient 터빈: 어 그리 게이터 : clusterConfig : $ {응용 프로그램} appConfig : $ {applications}```







`clusterConfig`및 `appConfig`부분이 일치해야하므로 별도의 구성 속성에 서비스 ID 년대의 쉼표로 구분 된 목록을 넣어 유용합니다.





Turbine.java



```@EnableTurbine @EnableDiscoveryClient @SpringBootApplication public class Turbine { 공공 정적 무효 메인 (문자열 [] args) { SpringApplication.run (DemoturbinecommonsApplication.class, args); } }```









# 봄 구름 사육사



이 프로젝트는 자동 환경 설정과 Spring Environment 및 다른 Spring 프로그래밍 모델 관용구에 대한 바인딩을 통해 Spring Boot 애플리케이션 용 사육자 통합을 제공합니다. 몇 가지 간단한 주석을 사용하여 애플리케이션 내부의 공통 패턴을 신속하게 활성화 및 구성하고 사육사 기반 구성 요소로 대규모 분산 시스템을 구축 할 수 있습니다. 제공되는 패턴에는 서비스 검색 및 구성이 포함됩니다. 지능형 라우팅 (Zuul) 및 클라이언트 측로드 밸런싱 (리본), 회로 차단기 (Hystrix)는 Spring Cloud Netflix와 통합되어 제공됩니다.





## 사육사 설치





[사육사](https://zookeeper.apache.org/doc/current/zookeeperStarted.html) 설치 방법에 대해서는 설치 설명서 를 참조하십시오 .









## 사육사를 통한 서비스 검색





서비스 검색은 마이크로 서비스 기반 아키텍처의 핵심 교리 중 하나입니다. 각 클라이언트 또는 일부 형식의 컨벤션을 손으로 구성하려는 것은 매우 어려울 수 있으며 매우 약해질 수 있습니다. [큐레이터](https://curator.apache.org/) (Zookeeper 용 자바 라이브러리)는 Service Discovery Extension을 통해 [서비스 검색](https://curator.apache.org/curator-x-discovery/) 서비스를 제공합니다 . Spring Cloud Zookeeper는 서비스 등록 및 발견을 위해이 확장 기능을 활용합니다.





### 활성화 방법



의존성을 포함하면 `org.springframework.cloud:spring-cloud-starter-zookeeper-discovery`Spring Cloud Zookeeper Discovery를 설정할 자동 구성이 활성화됩니다.







### 사육사와 함께 등록하기



클라이언트가 Zookeeper에 등록하면 호스트 및 포트, ID 및 이름과 같은 자체에 대한 메타 데이터를 제공합니다.





예제 사자 클라이언트 :







    @SpringBootApplication
    @EnableDiscoveryClient
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







(즉, 완전히 정상적인 스프링 부트 응용 프로그램). 사육사가 아닌 다른 곳에 `localhost:2181`위치하면 서버를 찾는 구성이 필요합니다. 예:





application.yml



```봄: 구름: 사육사 : connect-string : localhost : 2181```















주의

[Spring Cloud Zookeeper Config](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-zookeeper-config) 를 사용 하는 경우 위의 값을 `bootstrap.yml`대신에 배치해야합니다 `application.yml`.|











로부터 촬영의 기본 서비스 이름, 인스턴스 ID와 포트, `Environment`이다 `${spring.application.name}`, 스프링 컨텍스트 ID 및 `${server.port}`각각.





`@EnableDiscoveryClient` Zookeeper "서비스"(즉, 자신을 등록)와 "클라이언트"(즉, Zookeeper를 쿼리하여 다른 서비스를 찾을 수 있음)로 앱을 만듭니다.







### DiscoveryClient 사용



Spring Cloud는 [Feign](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/docs/src/main/asciidoc/spring-cloud-netflix.adoc#spring-cloud-feign) (REST 클라이언트 빌더)과 물리적 URL 대신 논리적 서비스 이름을 사용하는 [Spring`RestTemplate`](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/docs/src/main/asciidoc/spring-cloud-netflix.adoc#spring-cloud-ribbon) 을 지원한다.





또한 `org.springframework.cloud.client.discovery.DiscoveryClient`Netflix와 관련이없는 검색 클라이언트를위한 간단한 API를 제공하는을 사용할 수도 있습니다.







```@Autowired 개인용 DiscoveryClient discoveryClient;
 public String serviceUrl () { List <ServiceInstance> list = discoveryClient.getInstances ( "STORES"); if (list! = null && list.size ()> 0) { return list.get (0) .getUri (). toString (); } null를 돌려 준다. }```













## 사육사 종속성





### 사육사 종속성 사용



Spring Cloud Zookeeper는 응용 프로그램의 종속성을 특성으로 제공 할 수있는 기능을 제공합니다. 종속성에 따라 Zookeeper에 등록되어 있고 [Feign](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/docs/src/main/asciidoc/spring-cloud-netflix.adoc#spring-cloud-feign) (REST 클라이언트 작성기) 및 [Spring`RestTemplate`](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/docs/src/main/asciidoc/spring-cloud-netflix.adoc#spring-cloud-ribbon) 을 통해 호출 할 다른 응용 프로그램을 이해할 수 있습니다 .





또한 Zookeeper Dependency Watchers의 기능을 사용하면 종속성의 상태를 제어하고 모니터링하고 그로 인해 수행 할 작업을 결정할 수 있습니다.







### 사육사 종속성을 활성화하는 방법



*   의존성을 포함하면 `org.springframework.cloud:spring-cloud-starter-zookeeper-discovery`Spring Cloud Zookeeper Dependencies를 설정할 자동 구성이 활성화됩니다.

*   `spring.cloud.zookeeper.dependencies`섹션을 올바르게 설정 해야하는 경우 - 다음 섹션에서 자세한 내용을 확인한 다음 해당 기능이 활성화되어 있는지 확인하십시오

*   속성에 종속성을 제공 한 경우에도 종속성을 해제 할 수 있습니다. 속성 `spring.cloud.zookeeper.dependency.enabled`을 false 로 설정하면 됩니다 (기본값 `true`).







### 사육사 종속성 설정



종속성 표현의 예를 자세히 살펴 보겠습니다.





application.yml



```spring.application.name : yourServiceName spring.cloud.zookeeper : 의존성 : 뉴스 레터: 경로 : / path / where / newsletter / has / registered / in / zookeeper loadBalancerType : ROUND_ROBIN contentTypeTemplate : application / vnd.newsletter. $ version + json 버전 : v1 헤더 : header1 : - value1 header2 : - 값 2 required : false 스텁 : org.springframework : foo : 스텁 메일 링 : 경로 : / path / where / mailing / has / registered / in / zookeeper loadBalancerType : ROUND_ROBIN contentTypeTemplate : application / vnd.mailing. $ version + json 버전 : v1 required : true```







이제 의존 관계의 각 부분을 하나씩 살펴 보겠습니다. 루트 등록 정보 이름은 `spring.cloud.zookeeper.dependencies`입니다.





#### 별칭



루트 속성 아래에는 각 종속성을 나타 내기 위해 리본의 제약으로 인해 별칭이 있습니다 (응용 프로그램 ID는 URL에 있어야하므로 / foo / bar / name과 같은 복잡한 경로를 전달할 수 없습니다). 별칭은 serviceId 대신에 사용할 이름 이거나 `DiscoveryClient`, `Feign`또는 `RestTemplate`.





앞의 예에서 별칭은 `newsletter`및 `mailing`입니다. 예를 들면 다음과 `newsletter`같습니다.







```@FeignClient ( "뉴스 레터") 공용 인터페이스 NewsletterService { @RequestMapping (method = RequestMethod.GET, value = "/ newsletter") String getNewsletters (); }```









#### 통로



로 표시 `path`YAML 속성입니다.





Path는 Zookeeper에서 종속성이 등록되는 경로입니다. 리본이 URL에서 작동하기 전에 제시된 것과 같이 따라서이 경로는 요구 사항을 준수하지 않습니다. Spring Cloud Zookeeper가 별칭을 적절한 경로로 매핑하는 이유입니다.







#### 로드 밸런서 유형



로 표시 `loadBalancerType`YAML 속성입니다.





특정 종속성을 호출 할 때 어떤 종류의로드 밸런싱 전략을 적용해야하는지 알면 yaml 파일에로드 밸런싱 전략을 제공하면 자동으로 적용됩니다. 다음로드 균형 조정 전략 중 하나를 선택할 수 있습니다





*   STICKY - 한번 선택하면 인스턴스가 항상 호출됩니다.

*   RANDOM - 무작위로 인스턴스를 선택합니다.

*   ROUND_ROBIN - 인스턴스를 반복해서 반복합니다.







#### 콘텐츠 형식 템플릿 및 버전



에 의해 대표 `contentTypeTemplate`되고 `version`yaml 재산.





`Content-Type`헤더를 통해 API를 버전 화하면 각 요청에이 헤더를 추가하지 않으려 고합니다. 또한 API의 새 버전을 호출하려는 경우 코드 주위를 돌아 다니면서 API 버전을 높이기를 원하지 않습니다. 그래서 `contentTypeTemplate`특수 `$version`자리 표시자를 제공 할 수 있습니다 . 해당 자리 표시자는 `version`yaml 속성 의 값으로 채워집니다 . 예제를 살펴 보겠습니다.





다음과 같은 것들이 있습니다 `contentTypeTemplate`:







```application / vnd.newsletter. $ version + json```







및 다음 `version`:







```v1```







`Content-Type`각 요청에 대해 헤더를 설정합니다 .







```application / vnd.newsletter.v1 + json```









#### 기본 머리글



`headers`yaml 의지도에 의해 표시됨





때로는 종속성을 호출 할 때마다 일부 기본 헤더를 설정해야합니다. 코드에서 그렇게하지 않으려면 yaml 파일에서 설정할 수 있습니다. 다음 `headers`섹션이 있습니다.







```헤더 : 수락 : - text / html - application / xhtml + xml 캐시 제어 : - no-cache```







가산의 결과 `Accept`와 `Cache-Control`당신의 HTTP 요청에서 값의 해당 목록 헤더를.







#### 필수 종속성



`required`yaml의 부동산에 의해 대표 됨





응용 프로그램이 부팅 될 때 종속성 중 하나가 작동해야하는 `required: true`경우 yaml 파일에서 등록 정보 를 설정하기 만하면 됩니다.





응용 프로그램이 부팅하는 동안 필요한 종속성을 현지화 할 수없는 경우 예외가 발생하고 Spring 컨텍스트가 설정되지 않습니다. 즉, 필요한 종속성이 사육사에 등록되지 않은 경우 응용 프로그램을 시작할 수 없습니다.





다음 섹션에서 Spring Cloud Zookeeper Presence Checker에 대해 더 자세히 읽을 수 있습니다.







#### 스텁



종속성의 스텁을 포함하는 JAR에 콜론으로 구분 된 경로를 제공 할 수 있습니다. 예







    stubs: org.springframework:foo:stubs







특정 종속성을 찾을 수 있음을 의미합니다.





*   groupId : `org.springframework`

*   artifactId : `foo`

*   classifier : `stubs`- 이것이 기본값입니다.





이것은 실제로







    stubs: org.springframework:foo







이후 `stubs`기본 분류기입니다.









### Spring Cloud Zookeeper 종속성 구성



Zookeeper Dependencies 기능의 일부를 활성화 / 비활성화하도록 설정할 수있는 여러 속성이 있습니다.





*   `spring.cloud.zookeeper.dependencies` -이 속성을 설정하지 않으면 사육사 종속성의 혜택을받지 못합니다.

*   `spring.cloud.zookeeper.dependency.ribbon.enabled`(기본적으로 활성화 됨) - 리본에는 명시 적 전역 구성 또는 종속성을위한 특정 구성이 필요합니다. 이 속성을 실행하면로드 균형 조정 전략이 가능 `loadBalancerType`해지고 Zookeeper Dependencies 섹션 에서 이익을 얻을 수 있습니다 . 이 속성을 필요로하는 구성의 구현이 `LoadBalancerClient`받는 사람이 대표 `ILoadBalancer`다음 글 머리 기호로 표시를

*   `spring.cloud.zookeeper.dependency.ribbon.loadbalancer`(기본적으로 활성화 됨) -이 속성 덕분에 사용자 지정 `ILoadBalancer`은 리본에 전달 된 URI의 일부가 실제로 사육사의 적절한 경로로 해석되어야하는 별칭 일 수 있음을 알고 있습니다. 이 속성이 없으면 중첩 된 경로로 응용 프로그램을 등록 할 수 없습니다.

*   `spring.cloud.zookeeper.dependency.headers.enabled`(기본적으로 활성화 됨) -이 등록 정보는 자동 `RibbonClient`으로 종속성 구성에 표시된 버전으로 적절한 헤더 및 내용 유형을 추가합니다. 이 두 가지 매개 변수를 설정하지 않으면 작동하지 않습니다.

*   `spring.cloud.zookeeper.dependency.resttemplate.enabled`(기본적으로 활성화 됨) - 활성화 된 경우 `@LoadBalanced`주석 이 달린 요청 헤더를 수정하여 종속성 `RestTemplate`구성에 설정된 버전으로 헤더 및 컨텐츠 유형을 전달합니다. 이 두 매개 변수의 설정은 작동하지 않습니다.











## Spring Cloud Zookeeper Dependency Watcher





Dependency Watcher 메커니즘을 사용하면 종속성에 리스너를 등록 할 수 있습니다. 이 기능은 사실 `Observator`패턴의 구현입니다. 종속성이 상태 (UP 또는 DOWN)를 변경하면 일부 사용자 정의 논리를 적용 할 수 있습니다.





### 활성화 방법



Spring Cloud Zookeeper Dependencies 기능은 Dependency Watcher 메커니즘으로부터 이익을 얻을 수 있어야합니다.







### 청취자 등록하기



리스너를 등록하려면 인터페이스를 구현 `org.springframework.cloud.zookeeper.discovery.watcher.DependencyWatcherListener`하고 Bean으로 등록해야합니다. 인터페이스는 다음과 같은 한 가지 방법을 제공합니다.







``` void stateChanged (String dependencyName, DependencyState newState);```







특정 종속성에 대한 리스너를 등록하려는 경우 `dependencyName`구체적인 구현을위한 discriminator가됩니다. `newState`의존성이 `CONNECTED`또는으로 변경되었는지 여부에 대한 정보를 제공합니다 `DISCONNECTED`.







### 현재 상태 검사기



Dependency Watcher와 연결된 것은 Presence Checker라는 기능입니다. 의존성 상태에 따라 반응하도록 응용 프로그램을 부팅 할 때 사용자 정의 동작을 제공 할 수 있습니다.





추상 `org.springframework.cloud.zookeeper.discovery.watcher.presence.DependencyPresenceOnStartupVerifier`클래스 의 기본 구현은 다음 `org.springframework.cloud.zookeeper.discovery.watcher.presence.DefaultDependencyPresenceOnStartupVerifier`과 같은 방식으로 작동합니다.





*   종속성이 우리에게 표시되고 사육사에 `required`있지 않은 경우 응용 프로그램을 부팅하면 예외가 발생하고 종료됩니다

*   종속성이없는 `required`경우 `org.springframework.cloud.zookeeper.discovery.watcher.presence.LogMissingDependencyChecker`해당 애플리케이션이 `WARN`수준 에서 누락 될 것이라는 로그를 기록합니다.





`DefaultDependencyPresenceOnStartupVerifier`Bean이 없을 때만 등록되므로 기능을 재정의 할 수 있습니다 `DependencyPresenceOnStartupVerifier`.











## 사육사가있는 분산 구성





사육사는 클라이언트가 구성 데이터와 같은 임의의 데이터를 저장할 수 있는 [계층 적 네임 스페이스](https://zookeeper.apache.org/doc/current/zookeeperOver.html#sc_dataModelNameSpace) 를 제공합니다 . Spring Cloud Zookeeper Config는 [Config Server와 Client](https://github.com/spring-cloud/spring-cloud-config) 의 대안 입니다. 특별한 "부트 스트랩"단계에서 설정은 스프링 환경으로로드됩니다. 구성은 `/config`기본적으로 네임 스페이스에 저장 됩니다. `PropertySource`애플리케이션의 이름과 프로퍼티 해석의 Spring Cloud Config 순서를 모방 한 활성 프로파일을 기반으로 다중 인스턴스가 작성된다. 예를 들어, 이름이 "testApp"이고 "dev"프로파일이있는 응용 프로그램에는 다음과 같은 등록 정보 소스가 생성됩니다.







```config / testApp, dev config / testApp config / application, dev config / application```







가장 구체적인 속성 소스는 맨 위에 있으며 가장 구체적인 것은 맨 아래에 있습니다. Properties는 구성 `config/application`자를 사육사를 사용하는 모든 응용 프로그램에 적용 할 수있는 네임 스페이스입니다. 네임 스페이스의 `config/testApp`속성은 "testApp"라는 서비스 인스턴스에서만 사용할 수 있습니다.





구성은 현재 응용 프로그램 시작시 읽습니다. HTTP POST를 보내면 구성 `/refresh`이 다시로드됩니다. Zookeeper가 지원하는 구성 네임 스페이스는 현재 구현되지 않지만 향후이 프로젝트에 추가됩니다.





### 활성화 방법



의존성을 포함하면 `org.springframework.cloud:spring-cloud-starter-zookeeper-config`Spring Cloud Zookeeper Config를 설정할 자동 구성이 활성화됩니다.







### 커스터마이징



사육사 구성은 다음 속성을 사용하여 사용자 정의 할 수 있습니다.





bootstrap.yml



```봄: 구름: 사육사 : config : enabled : true 루트 : 구성 defaultContext : apps profileSeparator : '::'```







*   `enabled` 이 값을 "false"로 설정하면 Zookeeper Config가 비활성화됩니다.

*   `root` 구성 값의 기본 네임 스페이스를 설정합니다.

*   `defaultContext` 모든 응용 프로그램에서 사용하는 이름을 설정합니다.

*   `profileSeparator` 속성 소스의 프로필 이름과 프로필을 구분하는 데 사용되는 구분 기호의 값을 설정합니다.









# 스프링 부트 클라우드 CLI



Spring Boot CLI는 [Spring Cloud](https://github.com/spring-cloud) 에 대한 [Spring ](https://github.com/spring-cloud)[Boot](http://projects.spring.io/spring-boot) 명령 행 기능을 제공합니다 . Groovy 스크립트를 작성하여 Spring Cloud 컴포넌트 애플리케이션 (예 :)을 실행할 수 있다. 또한 암호화 및 암호 해독과 같은 작업을 수행하여 비밀 구성 값으로 Spring Cloud Config 클라이언트를 지원할 수 있습니다. Launcher CLI를 사용하면 Eureka, Zipkin, Config Server와 같은 서비스를 명령 줄에서 편리하게 실행할 수 있습니다 (개발시 매우 유용함). [](https://github.com/spring-cloud)`@EnableEurekaServer`





## 설치





설치하려면 [Spring Boot CLI](https://github.com/spring-projects/spring-boot) (1.4.1 이상) 가 설치되어 있어야합니다 .







```$ 봄 버전 Spring CLI v1.4.1.RELEASE```







예 : SDKMan 사용자







    $ sdk install springboot 1.4.1.RELEASE
    $ sdk use springboot 1.4.1.RELEASE







Spring Cloud 플러그인 설치하기







    $ mvn install
    $ spring install org.springframework.cloud:spring-cloud-cli:1.2.3.BUILD-SNAPSHOT















중대한

**전제 조건 :** 암호화 및 암호 해독 기능을 사용하려면 JVM에 전체 강도의 JCE가 설치되어 있어야합니다 (기본값은 없습니다). Oracle에서 "Java Cryptography Extension (JCE) 무제한 강도 관할 정책 파일"을 다운로드하고 설치 지침을 따르십시오 (기본적으로 JRE lib / security 디렉토리에있는 2 개의 정책 파일을 다운로드 한 정책 파일로 대체하십시오).|















## 개발중인 Spring Cloud Services 실행하기





Launcher CLI를 사용하여 Eureka, Config Server 등의 공통 서비스를 명령 줄에서 실행할 수 있습니다. 사용 가능한 서비스를 나열하고 `spring cloud --list`기본 서비스 세트를 시작 `spring cloud`하십시오. 배포 할 서비스를 선택하려면 명령 줄에 나열하십시오.







```$ 봄 구름 유레카 configserver h2 kafka zipkin```







지원되는 배치의 요약 :



<table class="tableblock frame-all grid-all spread"><colgroup><col style="width: 25%;"> <col style="width: 25%;"> <col style="width: 25%;"> <col style="width: 25%;"></colgroup>

<thead>



<th>서비스</td>

<th>이름</td>

<th>주소</td>

<th>기술</td>



</thead>





<td>

유레카

<td>

유레카 서버

<td>

[http : // localhost : 8761](http://localhost:8761/)

<td>

서비스 등록 및 검색을위한 유레카 서버. 다른 모든 서비스는 기본적으로 카탈로그에 표시됩니다.





<td>

구성 서버

<td>

구성 서버

<td>

[http : // localhost : 8888](http://localhost:8888/)

<td>

"기본"프로파일로 실행되고 로컬 디렉토리 ./launcher에서 구성을 제공하는 Spring Cloud 구성 서버





<td>

h2

<td>

H2 데이터베이스

<td>

[http : // localhost : 9095](http://localhost:9095/) (console), jdbc : h2 : tcp : // localhost : 9096 / {data}

<td>

관계 데이터베이스 서비스. 연결시 파일 경로를 사용하십시오 `{data}`(예 `./target/test`:). 추가 `;MODE=MYSQL`하거나 `;MODE=POSTGRESQL`다른 서버 유형과의 호환성으로 연결할 수 있습니다 .





<td>

카프카

<td>

카프카 브로커

<td>

[http : // localhost : 9091](http://localhost:9091/) (액츄에이터 끝점), localhost : 9092





<td>

hystrix 대시 보드

<td>

Hystrix 대시 보드

<td>

[http : // localhost : 7979](http://localhost:7979/)

<td>

Hystrix 회로 차단기를 선언하는 모든 Spring Cloud 앱은 메트릭을 게시 `/hystrix.stream`합니다. 이 주소를 대시 보드에 입력하여 모든 측정 항목을 시각화하고,





<td>

데이터 흐름

<td>

데이터 흐름 서버

<td>

[http : // localhost : 9393](http://localhost:9393/)

<td>

/ admin-ui에 UI가있는 Spring Cloud Dataflow 서버. 데이터 흐름 쉘을 루트 경로에서 대상에 연결하십시오.





<td>

지퍼 킨

<td>

Zipkin 서버

<td>

[http : // localhost : 9411](http://localhost:9411/)

<td>

추적을 시각화하기위한 UI가있는 Zipkin Server. 상점은 데이터를 메모리에 저장하고 JSON 데이터의 HTTP POST를 통해이를 수용합니다.









이러한 각 응용 프로그램은 같은 이름의 로컬 YAML 파일 (현재 작업 디렉토리 또는 "config"또는 in이라는 하위 디렉토리)을 사용하여 구성 할 수 있습니다 `~/.spring-cloud`. 예 `configserver.yml`를 들어, 백엔드 용 로컬 git 저장소를 찾으려면 다음과 같이 할 수 있습니다.





configserver.yml



    spring:
      profiles:
        active: git
      cloud:
        config:
          server:
            git:
              uri: file://${user.home}/dev/demo/config-repo







### 추가 응용 프로그램 추가



추가 응용 프로그램을 추가 할 수 있습니다 `./config/cloud.yml`( `./config.yml`기본값을 대체 할 수있는 것이 아니기 때문에). 예 :





config / cloud.yml



    spring:
      cloud:
        launcher:
          deployables:
            source:
              coordinates: maven://com.example:source:0.0.1-SNAPSHOT
              port: 7000
            sink:
              coordinates: maven://com.example:sink:0.0.1-SNAPSHOT
              port: 7001







앱 나열시 :







    $ spring cloud --list
    source sink configserver dataflow eureka h2 hystrixdashboard kafka zipkin







(목록의 시작 부분에 추가 앱이 있음을 알 수 있습니다).











## Groovy 스크립트 작성 및 응용 프로그램 실행





Spring Cloud CLI는 주석 `@Enable*`클래스 와 같은 대부분의 Spring Cloud 선언 기능 을 지원한다. 예를 들어, 유레카 서버가 여기 있습니다.





app.groovy



    @EnableEurekaServer
    class Eureka {}







이 명령 줄에서 다음과 같이 실행할 수 있습니다.







```$ spring run app.groovy```







추가 종속성을 포함하려면, 종종 그냥 예를 들어, 해당 기능이 활성화 주석을 추가하기에 충분 `@EnableConfigServer`, `@EnableOAuth2Sso`또는 `@EnableEurekaClient`. 의존성을 수동으로 포함 시키려면 `@Grab`, 특수한 "Spring Boot"짧은 스타일 아티팩트 좌표 (예 : 그룹 또는 버전 정보가 필요 없음)와 함께, 즉 AMQP를 수신 대기하도록 클라이언트 응용 프로그램을 설정하는 것과 같이 Spring CLoud Bus의 관리 이벤트 용 :





app.groovy



    @Grab('spring-cloud-starter-bus-amqp')
    @RestController
    class Service {
      @RequestMapping('/')
      def home() { [message: 'Hello'] }
    }











## 암호화 및 암호 해독





Spring Cloud CLI에는 "encrypt"와 "decrypt"명령이있다. 둘 다 필수적인 "- key"로 지정된 키를 사용하여 동일한 형식의 인수를 허용합니다.







```$ spring encrypt mysecret --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda $ spring decrypt --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda 나의 비밀```







파일 (예 : encyption을위한 RSA 공개 키)에서 키를 사용하려면 키 값 앞에 "@"를 붙이고 파일 경로를 제공하십시오.







```$ spring encrypt mysecret --key @ $ {HOME} /. ssh / id_rsa.pub AQAjPgt3eFZQXwt8tsHAVv / QHiY5sI2dRcR + ...```









# 스프링 클라우드 보안



Spring Cloud Security는 안전한 애플리케이션과 서비스를 최소한의 방법으로 구축하기위한 일련의 프리미티브를 제공합니다. 외부 적으로 (또는 중심적으로) 크게 구성 될 수있는 선언적 모델은 대개 중앙의 들여 쓰기 관리 서비스를 사용하는 대규모 공동 시스템 원격 구성 요소의 구현에 적합합니다. 또한 Cloud Foundry와 같은 서비스 플랫폼에서 사용하기가 매우 쉽습니다. Spring Boot and Spring Security OAuth2를 기반으로 우리는 싱글 사인온 (single sign on), 토큰 릴레이 및 토큰 교환 같은 공통 패턴을 구현하는 시스템을 신속하게 생성 할 수 있습니다.





## 빠른 시작





### OAuth2 싱글 사인온



다음은 HTTP 기본 인증 및 단일 사용자 계정이있는 Spring Cloud "Hello World"앱입니다.





app.groovy



    @Grab('spring-boot-starter-security')
    @Controller
    class Application {

      @RequestMapping('/')
      String home() {
        'Hello World'
      }

    }







`spring run app.groovy`암호를 사용하여 실행 하고 암호에 대한 로그를 볼 수 있습니다 (사용자 이름은 "user"임). 지금까지는 Spring Boot app의 기본값입니다.





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







차이를 발견? 이 앱은 아직 OAuth2 신빙성을 알지 못하기 때문에 실제로 이전 앱과 정확히 동일하게 작동합니다.





github에서 앱을 쉽게 등록 할 수 있으므로 자신의 도메인에 프로덕션 응용 프로그램이 필요한 경우 사용해보십시오. localhost : 8080에서 테스트 할 수 있다면 응용 프로그램 구성에서 다음 등록 정보를 설정하십시오.





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







위의 앱을 실행하면 승인을 위해 github로 리디렉션됩니다. github에 이미 로그인 한 경우 인증을받지 못합니다. 이 자격 증명은 앱이 포트 8080에서 실행되는 경우에만 작동합니다.





클라이언트가 액세스 토큰을 얻을 때 묻는 범위를 제한하기 위해 설정할 수 있습니다 `spring.oauth2.client.scope`(쉼표로 구분되거나 YAML의 배열). 기본적으로 범위는 비어 있으며 권한 서버가 보유해야하는 클라이언트 등록 설정에 따라 기본값을 결정해야합니다.













노트

위의 예는 모두 Groovy 스크립트입니다. 동일한 코드를 Java (또는 Groovy)로 작성하려면 Spring Security OAuth2를 클래스 경로에 추가해야합니다 (예 : [여기 샘플](https://github.com/spring-cloud-samples/sso) 참조 ).|













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







과





application.yml



    spring:
      oauth2:
        resource:
          userInfoUri: https://api.github.com/user
          preferTokenInfo: false













## 자세한 세부 사항





### 싱글 사인온 (SSO)











노트

OAuth2 SSO 및 리소스 서버 기능은 모두 Spring Boot 버전 1.3으로 이전되었습니다. [Spring Boot 사용자 가이드](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/) 에서 문서를 찾을 수 있습니다 .|













### 토큰 릴레이



토큰 릴레이는 OAuth2 고객이 클라이언트 역할을하고 들어오는 토큰을 나가는 리소스 요청으로 전달하는 곳입니다. 소비자는 순수 클라이언트 (SSO 응용 프로그램과 같은) 또는 자원 서버가 될 수 있습니다.





#### 클라이언트 토큰 릴레이



앱이 OAuth2 클라이언트를 향한 (즉, `@EnableOAuth2Sso`또는 선언 된 `@EnableOAuth2Client`) 사용자 인 경우 `OAuth2ClientContext`Spring Boot에서 요청 범위를가집니다. `OAuth2RestTemplate`이 컨텍스트와 autowired에서 자신 만의 컨텍스트 를 만들 수 `OAuth2ProtectedResourceDetails`있으며 컨텍스트는 액세스 토큰을 항상 다운 스트림으로 전달하고 액세스 토큰이 만료되면 자동으로 새로 고칩니다. (이것들은 Spring Security와 Spring Boot의 기능입니다.)













노트

토큰 `OAuth2ProtectedResourceDetails`을 사용하고 있다면 스프링 부트 (1.4.1)가 자동으로 생성되지 않습니다 `client_credentials`. 이 경우 당신은 당신의 자신을 만들 필요 `ClientCredentialsResourceDetails`하고 그것을 구성 `@ConfigurationProperties("security.oauth2.client")`.|













#### 주루 프록시의 클라이언트 토큰 릴레이



앱에 [스프링 클라우드 Zuul이](http://cloud.spring.io/spring-cloud.html#netflix-zuul-reverse-proxy) 내장 된 리버스 프록시 (사용 `@EnableZuulProxy`)가있는 경우 OAuth2 액세스 토큰을 프록 싱중인 서비스로 전달하도록 요청할 수 있습니다. 따라서 위의 SSO 앱은 다음과 같이 간단하게 향상시킬 수 있습니다.





app.groovy



    @Controller
    @EnableOAuth2Sso
    @EnableZuulProxy
    class Application {

    }







(사용자를 로깅하고 토큰을 얻는 것 이외에) 인증 토큰을 `/proxy/*` 서비스의 다운 스트림으로 전달 합니다. 이러한 서비스가 구현 `@EnableResourceServer`되면 올바른 헤더에 유효한 토큰을 가져옵니다.





어떻게 작동합니까? `@EnableOAuth2Sso`주석에 끌어 `spring-cloud-starter-security`(당신은 기존의 응용 프로그램에서 수동으로 할 수있는), 그리고 차례로 그는 몇 가지 자동 트리거 `ZuulFilter`Zuul 클래스 경로 (경유에 있기 때문에 그 자체가 활성화되고 `@EnableZuulProxy`). [필터는](https://github.com/spring-cloud/spring-cloud-security/tree/master/src/main/java/org/springframework/cloud/security/oauth2/proxy/OAuth2TokenRelayFilter.java) 단지 현재 인증 된 사용자의 액세스 토큰을 추출하고, 다운 스트림 요청을 요청 헤더에 넣는다.







#### 리소스 서버 토큰 릴레이



앱에 `@EnableResourceServer`있다면 들어오는 토큰을 다른 서비스로 중계 할 수 있습니다. 를 사용 `RestTemplate`하여 다운 스트림 서비스에 연결하는 경우 올바른 컨텍스트로 템플리트를 작성하는 방법과 관련됩니다.





서비스가 사용하는 경우 `UserInfoTokenServices`(가 사용하는, 즉 수신 토큰을 인증하기 위해 `security.oauth2.user-info-uri` 구성), 당신은 단순히를 만들 수 있습니다 `OAuth2RestTemplate` 를 autowire를 사용하여 `OAuth2ClientContext`(가 백엔드 코드를 명중하기 전에이 인증 프로세스에 의해 채워집니다). 등가 (봄 부팅 1.4), 당신은을 주입 할 수 `UserInfoRestTemplateFactory`와를 잡아 `OAuth2RestTemplate`구성에. 예 :





MyConfiguration.java



    @Bean
    public OAuth2RestTemplate restTemplate(UserInfoRestTemplateFactory factory) {
        return factory.getUserInfoRestTemplate();
    }







그런 다음이 나머지 템플리트는 `OAuth2ClientContext` 인증 필터에서 사용되는 것과 동일한 (요청 범위가) 있으므로 동일한 액세스 토큰으로 요청을 보낼 수 있습니다.





앱이 사용 `UserInfoTokenServices`하지 않지만 여전히 클라이언트 인 경우 (즉 , `@EnableOAuth2Client`또는을 선언 하면) 사용자가 만든 `@EnableOAuth2Sso`모든 `OAuth2RestOperations`것을 Spring Security Cloud 에서 `@Autowired` `@OAuth2Context`토큰을 전달합니다. 이 기능은 기본적으로 MVC 핸들러 인터셉터로 구현되므로 Spring MVC에서만 작동합니다. MVC를 사용하지 않는다면 `AccessTokenContextRelay`동일한 기능을 제공하기 위해 맞춤 필터 또는 AOP 인터셉터를 사용할 수 있습니다 .





다음은 다른 곳에 만들어진 autowired 나머지 템플리트의 사용을 보여주는 기본 예제입니다 ( "foo.com"은 주변 애플리케이션과 동일한 토큰을 허용하는 자원 서버 임).





MyController.java



    @Autowired
    private OAuth2RestOperations restTemplate;

    @RequestMapping("/relay")
    public String relay() {
        ResponseEntity<String> response =
          restTemplate.getForEntity("https://foo.com/bar", String.class);
        return "Success! (" + response.getBody() + ")";
    }







토큰을 전달하고 싶지 않다면 (토큰을 보낸 클라이언트가 아닌 직접 행동하는 것이 좋을 수 있으므로 올바른 선택입니다.) `OAuth2Context`기본값을 autowiring하는 대신 자신 만의 토큰을 만들어야합니다 하나.





Feign 클라이언트는 사용할 수있는 `OAuth2ClientContext`경우이를 사용하는 인터셉터도 선택 하므로 토큰 릴레이를 수행해야합니다 `RestTemplate`.













## Zuul 프록시의 인증 다운 스트림 구성





설정 `@EnableZuulProxy`을 통해 인증 동작 다운 스트림을 제어 할 수 `proxy.auth.*`있습니다. 예:





application.yml



    proxy:
      auth:
        routes:
          customers: oauth2
          stores: passthru
          recommendations: none







이 예에서 '고객'서비스는 OAuth2 토큰 릴레이를 가져 오며, '상점'서비스는 통과 (인증 헤더가 다운 스트림으로 전달됨)되고 '추천'서비스는 인증 헤더가 제거됩니다. 기본 동작은 사용 가능한 토큰이있는 경우 토큰 릴레이를 수행하고 그렇지 않으면 패스 스루를 수행하는 것입니다.





자세한 내용은 [ProxyAuthenticationProperties](https://github.com/spring-cloud/spring-cloud-security/tree/master/src/main/java/org/springframework/cloud/security/oauth2/proxy/ProxyAuthenticationProperties) 를 참조 하십시오.







# 클라우드 파운드리 용 스프링 클라우드







Cloudfoundry 용 Spring Cloud를 사용하면 [Cloud Foundry](https://github.com/cloudfoundry) ( [Cloud](https://github.com/cloudfoundry) Platform) 에서 [Spring Cloud](https://github.com/spring-cloud) 애플리케이션을 쉽게 실행할 수 있습니다 . Cloud Foundry에는 앱에 "바인딩"하는 미들웨어 인 본질적으로 자격 증명이 포함 된 환경 변수 (예 : 서비스에 사용할 위치 및 사용자 이름)를 제공하는 "서비스"개념이 있습니다.[](https://github.com/cloudfoundry)





이 `spring-cloud-cloudfoundry-web`프로젝트는 싱글 사인온 (single-sign-on) 서비스에 자동으로 바인딩하고 필요에 따라 검색을위한 끈적한 라우팅을 가능하게하는 Cloud Foundry의 일부 웹 응용 프로그램 기능을 기본적으로 지원합니다.





`spring-cloud-cloudfoundry-discovery`프로젝트는 봄 구름 풍경의 구현을 제공 `DiscoveryClient`당신이 할 수 있도록 `@EnableDiscoveryClient`하고 자격 증명을 제공 `spring.cloud.cloudfoundry.discovery.[email,password]`하고 사용자가 사용할 수 있습니다 `DiscoveryClient`직접 또는 통해 `LoadBalancerClient` (또한 `*.url`당신이에 연결되지 않은 경우 [중추 웹 서비스](https://run.pivotal.io/) ).





처음으로 사용하는 경우 Cloud Foundry에서 액세스 토큰을 얻어야하므로 검색 클라이언트가 느려질 수 있습니다.









## 발견





클라우드 파운드리 검색 기능이있는 Spring Cloud 앱은 다음과 같습니다.





app.groovy



    @Grab('org.springframework.cloud:spring-cloud-cloudfoundry')
    @RestController
    @EnableDiscoveryClient
    class Application {

      @Autowired
      DiscoveryClient client

      @RequestMapping('/')
      String home() {
        'Hello from ' + client.getLocalServiceInstance()
      }

    }







서비스 바인딩없이 실행하면 :







```$ spring jar app.jar app.groovy $ cf push -p app.jar```







홈 페이지에 앱 이름이 표시됩니다.





`DiscoveryClient`캔은 하나의 공간 기본적으로 클라이언트가 (있는 경우)에서 실행되는가에 인증 자격 증명에 따라, 공간에있는 모든 응용 프로그램을 나열합니다. 조직이나 공간이 구성되어 있지 않으면 Cloud Foundry의 사용자 프로필별로 기본값이 설정됩니다.









## 싱글 사인온 (SSO)













노트

OAuth2 SSO 및 리소스 서버 기능은 모두 Spring Boot 버전 1.3으로 이전되었습니다. [Spring Boot 사용자 가이드](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/) 에서 문서를 찾을 수 있습니다 .|











이 프로젝트는 CloudFoundry 서비스 자격 증명에서 Spring Boot 기능으로 자동 바인딩을 제공합니다. 예를 들어, "client_id", "client_secret"및 "auth_domain"을 포함하는 자격 증명을 사용하여 "sso"라는 CloudFoundry 서비스가 있으면 `@EnableOAuth2Sso`(Spring Boot에서) 사용하도록 설정 한 Spring OAuth2 클라이언트에 자동으로 바인드 됩니다. 를 사용하여 서비스의 이름을 매개 변수화 할 수 있습니다 `spring.oauth2.sso.serviceId`.







# 스프링 클라우드 클러스터



Spring Cloud Cluster는 "클러스터"기능을 분산 시스템에 구축하기위한 기본 세트를 제공합니다. 리더십 선거, 클러스터 상태의 일관된 저장, 전역 잠금 및 일회성 토큰이 그 예입니다.





## 총선거





리더 선거를 통해 응용 프로그램은 다른 응용 프로그램과 함께 작업하여 타사 시스템을 통해 클러스터 리더십을 조정할 수 있습니다. 현재 우리는 `zookeeper`, `hazelcast`및을 (를) 제공 `etcd`합니다.





사용자의 관점에서 선거 인터페이스를 통해 작동 `org.springframework.cloud.cluster.leader.Candidate`하고 `org.springframework.cloud.cluster.leader.Context`. `Candidate` 지도력에 대한 접근권을 포함 `role`하고 `id`있으며 또한 방법론 `onGranted`을 가지고있다 `onRevoked`. 이러한 콜백 메소드는 기본 `Candidate`구현이 변경 되는 경우 유용합니다 .





리더 선거는 경우 자동으로 구성되어 있습니다 `spring-cloud-cluster-autoconfigure` 및 중 하나 `spring-cloud-cluster-hazelcast`, `spring-cloud-cluster-zookeeper` 또는 `spring-cloud-cluster-etcd`항아리가 클래스 경로에서 발견된다. 양쪽 항아리가있는 경우 리더 선거는 두 시스템을 사용하여 생성됩니다. 생성 된 bean에 대한 자세한 정보는 [Zookeeper](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-cluster-leaderelection-zookeeper) , [Hazelcast](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-cluster-leaderelection-hazelcast) 및 [Etcd](http://cloud.spring.io/spring-cloud-static/spring-cloud.html#spring-cloud-cluster-leaderelection-etcd) 섹션을 참조하십시오 .





`Candidate`자동 구성에서 생성 된 기본값은 현재 `org.springframework.cloud.cluster.leader.DefaultCandidate`부여 및 취소 된 이벤트 만 기록합니다.





모든 리더 관련 자동 구성을 비활성화해야하는 경우 a `spring.cloud.cluster.leader.enabled`를 false로 설정할 수 있습니다. 그러면 클래스 패스에 jar 파일이 있더라도 수동 구성을 수행 할 수 있습니다. 속성 `spring.cloud.cluster.leader.id`및 `spring.cloud.cluster.leader.role`기본 식별자와 역할을 설정하는 데 사용할 수 있습니다.





부여 된 이벤트와 취소 된 이벤트에 대한 간단한 통지에 관심이 있다면 하나의 옵션은 이벤트 리스너를 스프링 어플리케이션 컨텍스트에 첨부하는 것입니다. 이벤트 `OnGrantedEvent`및 `OnRevokedEvent`봄 이벤트 개체로 전송됩니다.





자신 만의 이벤트 리스너 클래스를 만들면됩니다.







    class MyEventListener implements ApplicationListener<AbstractLeaderEvent> {

      @Override
      public void onApplicationEvent(AbstractLeaderEvent event) {
        // do something with OnGrantedEvent or OnRevokedEvent
      }
    }







그것을 빈으로 생성하십시오.







    @Configuration
    static class Config {
      @Bean
      public MyEventListener myEventListener() {
        return new MyEventListener();
      }
    }







단순한 로그 이벤트의 경우 `LoggingListener`쉽게 구성 할 수 있는 유틸리티 클래스 를 사용할 수도 있습니다 .







    import org.springframework.cloud.cluster.leader.event.LoggingListener;

    @Configuration
    static class Config {
      @Bean
      public LoggingListener loggingListener() {
        return new LoggingListener("info");
      }
    }







### 사육사



`Candidate`사육사를위한 구현은 `zookeeperLeaderCandidate`자동 구성 중에 생성 된 bean 이름 을 무시하는 데 사용할 수 있는 bean 이름 으로 작성됩니다.





사육사 기반의 선거는 속성을 사용하여 명시 적으로 비활성화 할 수 있습니다 `spring.cloud.cluster.zookeeper.leader.enabled`.





다른 속성 `spring.cloud.cluster.zookeeper.namespace`및 `spring.cloud.cluster.zookeeper.connect`사육사 기본 네임 스페이스 경로 및 연결 문자열을 설정하는 데 사용할 수 있습니다.







### 헤즐



`Candidate`hazelcast 구현은 `hazelcastLeaderCandidate`자동 구성 중에 작성된 bean 이름 을 대체하는 데 사용할 수 있는 bean 이름 으로 작성됩니다.





헤즐 캐스팅 기반 선거는 속성을 사용하여 명시 적으로 비활성화 할 수 있습니다 `spring.cloud.cluster.hazelcast.leader.enabled`. Hazelcast 인스턴스에 대해 xml 기반 설정을 제공하려면 속성 `spring.cloud.cluster.hazelcast.config-location`을 사용 하여 Hazelcast xml 설정 파일의 위치를 ​​알려줍니다. `config-location`정상적인 봄 `Resource`입니다.







### 기타



`Candidate`etcd에 대한 구현은 `etcdLeaderCandidate`자동 구성 중에 생성 된 bean 이름 을 덮어 쓰는 데 사용할 수 있는 bean 이름 으로 작성됩니다.





Etcd 기반 선거는 속성을 사용하여 명시 적으로 비활성화 할 수 있습니다 `spring.cloud.cluster.etcd.leader.enabled`.





속성을 사용하여 여러 개의 etcd 클러스터 URL을 지정할 수 있습니다. `spring.cloud.cluster.etcd.connect`









# 부록 : 구성 등록 정보의 개요





<table class="tableblock frame-all grid-all spread"><colgroup><col style="width: 33%;"> <col style="width: 33%;"> <col style="width: 33%;"></colgroup>

<thead>



<th>이름</td>

<th>태만</td>

<th>기술</td>



</thead>





<td>

<font class="">encrypt.fail-on-error

<td>

참된

<td>

암호화 또는 암호 해독 오류가있는 경우 프로세스가 실패해야한다고 말하는 플래그입니다.





<td>

encrypt.key

<td>

대칭 키. 더 강력한 대안으로 키 스토어 사용을 고려하십시오.





<td>

encrypt.key-store.alias

<td>

저장소의 키 별칭입니다.





<td>

encrypt.key-store.location

<td>

키 저장 파일의 위치 (예 : classpath : /keystore.jks).





<td>

encrypt.key-store.password

<td>

키 저장소를 잠그는 암호입니다.





<td>

encrypt.key-store.secret

<td>

비밀 키 보호 (기본값은 암호와 동일).





<td>

encrypt.rsa.algorithm

<td>

사용할 RSA 알고리즘 (DEFAULT 또는 OEAP)입니다. 설정이 끝나면 변경하지 마십시오 (또는 기존 암호는 해독 할 수 없습니다).





<td>

encrypt.rsa.salt

<td>

죽은 자

<td>

암호 텍스트를 암호화하는 데 사용되는 임의의 암호에 대한 소금. 설정이 끝나면 변경하지 마십시오 (또는 기존 암호는 해독 할 수 없습니다).





<td>

encrypt.rsa.strong

<td>

그릇된

<td>

"강력한"AES 암호화가 내부적으로 사용되어야 함을 나타내는 플래그. true이면 GCM 알고리즘이 AES 암호화 된 바이트에 적용됩니다. 기본값은 false입니다 (이 경우 "표준"CBC가 대신 사용됩니다). 설정이 끝나면 변경하지 마십시오 (또는 기존 암호는 해독 할 수 없습니다).





<td>

endpoints.bus.enabled





<td>

endpoints.bus.id





<td>

endpoints.bus.sensitive





<td>

endpoints.consul.enabled





<td>

endpoints.consul.id





<td>

endpoints.consul.sensitive





<td>

endpoints.features.enabled





<td>

endpoints.features.id





<td>

endpoints.features.sensitive





<td>

endpoints.pause.enabled





<td>

endpoints.pause.id





<td>

endpoints.pause.sensitive





<td>

endpoints.refresh.enabled





<td>

endpoints.refresh.id





<td>

endpoints.refresh.sensitive





<td>

endpoints.restart.enabled





<td>

endpoints.restart.id





<td>

endpoints.restart.pause-endpoint.enabled





<td>

endpoints.restart.pause-endpoint.id





<td>

endpoints.restart.pause-endpoint.sensitive





<td>

endpoints.restart.resume-endpoint.enabled





<td>

endpoints.restart.resume-endpoint.id





<td>

endpoints.restart.resume-endpoint.sensitive





<td>

endpoints.restart.sensitive





<td>

endpoints.restart.timeout

<td>

0





<td>

endpoints.resume.enabled





<td>

endpoints.resume.id





<td>

endpoints.resume.sensitive





<td>

eureka.client.allow-redirects

<td>

그릇된

<td>

서버가 클라이언트 요청을 백업 서버 / 클러스터로 재지 정할 수 있는지 여부를 나타냅니다. false로 설정하면 서버가 요청을 직접 처리합니다. true로 설정하면 새 서버 위치로 클라이언트에 HTTP 리디렉션을 보낼 수 있습니다.





<td>

eureka.client.availability-zones

<td>

이 인스턴스가있는 지역의 가용성 영역 목록 (AWS 데이터 센터에서 사용됨)을 가져옵니다.

변경 사항은 registryFetchIntervalSeconds에 지정된 다음 레지스트리 페치 사이클에서 런타임에 유효합니다.





<td>

eureka.client.backup-registry-impl

<td>

eureka 클라이언트가 처음 시작될 때만 레지스트리 정보를 폴백 옵션으로 가져 오기 위해 BackupRegistry를 구현하는 구현의 이름을 가져옵니다.

레지스트리 정보에 대한 추가 복원력이 필요하지 않은 응용 프로그램에서는이 레지스트리 정보가 작동하지 않을 수 있습니다.





<td>

eureka.client.cache-refresh-executor-exponential-back-off-bound

<td>

10

<td>

executor exponential back off 관련 속성을 캐시에 새로 고칩니다. 일련의 시간 초과가 발생한 경우 재시도 지연에 대한 최대 배율 값입니다.





<td>

eureka.client.cache-refresh-executor-thread-pool-size

<td>

2

<td>

cacheRefreshExecutor가 초기화 할 스레드 풀 크기





<td>

eureka.client.client-data-accept

<td>

클라이언트 데이터 수용을위한 EurekaAccept 이름





<td>

eureka.client.decoder-name

<td>

이것은 일시적인 구성이며 최신 코덱이 안정되면 제거 할 수 있습니다 (단 하나만있을 수 있음).





<td>

eureka.client.disable-delta

<td>

그릇된

<td>

유레카 클라이언트가 델타 가져 오기를 비활성화해야하는지 여부를 나타내며 전체 레지스트리 정보를 가져와야합니다.

델타 페치는 트래픽을 엄청나게 줄일 수 있습니다. 유레카 서버의 변경 속도가 일반적으로 페치 속도보다 훨씬 빠르기 때문입니다.

변경 사항은 런타임에 registryFetchIntervalSeconds에 지정된 다음 레지스트리 페치 사이클에서 유효합니다.





<td>

eureka.client.dollar-replacement

<td>

_-

<td>

유레카 서버에서 정보 직렬화 / 역 직렬화 중에 <code> $ </ code> 달러 기호에 대한 대체 문자열을 가져옵니다.





<td>

eureka.client.enabled

<td>

참된

<td>

유레카 클라이언트가 활성화되었음을 나타내는 플래그입니다.





<td>

eureka.client.encoder-name

<td>

이것은 일시적인 구성이며 최신 코덱이 안정되면 제거 할 수 있습니다 (단 하나만있을 수 있음).





<td>

eureka.client.escape-char-replacement

<td>

__

<td>

유레카 서버의 정보 직렬화 / 직렬화 해제 중 밑줄 기호 <code> _ </ code>에 대한 대체 문자열을 가져옵니다.





<td>

eureka.client.eureka-connection-idle-timeout-seconds

<td>

30

<td>

유레카 서버에 대한 HTTP 연결이 닫히기 전에 유휴 상태를 유지할 수있는 시간 (초)을 나타냅니다.

AWS 환경에서는 Limbo에 연결이 끊긴 채로 몇 분이 지난 후에 방화벽이 연결 정보를 정리하므로 값을 30 초 이하로 설정하는 것이 좋습니다





<td>

eureka.client.eureka-server-connect-timeout-seconds

<td>

5

<td>

유레카 서버에 대한 연결이 시간 초과되어야하기까지 대기 할 시간 (초)을 나타냅니다. 클라이언트의 연결은 org.apache.http.client.HttpClient에 의해 풀링되며이 설정은 실제 연결 생성과 풀에서 연결을 기다리는 시간에 영향을줍니다.





<td>

eureka.client.eureka-server-dnsname

<td>

유레카 서버 목록을 가져 오기 위해 쿼리 할 DNS 이름을 가져옵니다. 계약서에서 serviceUrl을 구현하여 서비스 URL을 반환하면이 정보는 필요하지 않습니다.

DNS 메커니즘은 useDnsForFetchingServiceUrls가 true로 설정되고 유레카 클라이언트가 변경 유레카 서버를 동적으로 가져올 수 있도록 DNS가 특정 방식으로 구성 될 것을 기대할 때 사용됩니다.

변경 사항은 런타임에 효과적입니다.





<td>

eureka.client.eureka-server-port

<td>

유레카 서버 목록이 DNS에서 왔을 때 유레카 서버에 접속할 서비스 URL을 구성하는 데 사용할 포트를 가져옵니다. 계약서에서 서비스 URL 인 eurekaServerServiceUrls (String)를 반환하는 경우이 정보는 필요하지 않습니다.

DNS 메커니즘은 useDnsForFetchingServiceUrls가 true로 설정되고 유레카 클라이언트가 변경 유레카 서버를 동적으로 가져올 수 있도록 DNS가 특정 방식으로 구성 될 것을 기대할 때 사용됩니다.

변경 사항은 런타임에 효과적입니다.





<td>

eureka.client.eureka-server-read-timeout-seconds

<td>

8

<td>

유레카 서버에서 읽는 시간이 초과되기까지 대기 할 시간 (초)을 나타냅니다.





<td>

eureka.client.eureka-server-total-connections

<td>

200

<td>

eureka 클라이언트에서 모든 eureka 서버로 허용되는 총 연결 수를 가져옵니다.





<td>

eureka.client.eureka-server-total-connections-per-host

<td>

50

<td>

eureka 클라이언트에서 eureka 서버 호스트로 허용되는 총 연결 수를 가져옵니다.





<td>

eureka.client.eureka-server-urlcontext

<td>

유레카 서버 목록이 DNS에서 왔을 때 eureka 서버에 접속할 서비스 url을 생성하는 데 사용할 URL 컨텍스트를 가져옵니다. 계약서가 eurekaServerServiceUrls에서 서비스 URL을 반환하는 경우이 정보는 필요하지 않습니다.

DNS 메커니즘은 useDnsForFetchingServiceUrls가 true로 설정되고 유레카 클라이언트가 변경 유레카 서버를 동적으로 가져올 수 있도록 DNS가 특정 방식으로 구성 될 것을 기대할 때 사용됩니다. 변경 사항은 런타임에 효과적입니다.





<td>

eureka.client.eureka-service-url-poll-interval-seconds

<td>

0

<td>

유레카 서버 정보의 변경 사항을 폴링하는 빈도 (초)를 나타냅니다. 유레카 서버를 추가하거나 제거 할 수 있으며이 설정은 유레카 클라이언트가 얼마나 빨리 그 사실을 알아야 할지를 제어합니다.





<td>

eureka.client.fetch-registry

<td>

참된

<td>

이 클라이언트가 eureka 서버에서 eureka 레지스트리 정보를 가져와야하는지 여부를 나타냅니다.





<td>

eureka.client.fetch-remote-regions-registry

<td>

유레카 레지스트리 정보를 가져올 영역의 쉼표로 구분 된 목록입니다. availabilityZones가 반환 한 각 영역의 가용성 영역을 정의하는 것이 필수입니다. 그렇게하지 않으면 검색 클라이언트가 시작되지 않습니다.





<td>

eureka.client.filter-only-up-instances

<td>

참된

<td>

InstanceStatus UP 상태 만있는 인스턴스에 대해 응용 프로그램을 필터링 한 후 응용 프로그램을 가져올 지 여부를 나타냅니다.





<td>

eureka.client.g-zip-content

<td>

참된

<td>

eureka 서버에서 가져온 내용을 서버에서 지원할 때마다 압축해야하는지 여부를 나타냅니다. 최적의 네트워크 트래픽을 위해 유레카 서버의 레지스트리 정보가 압축됩니다.





<td>

eureka.client.heartbeat-executor-exponential-back-off-bound

<td>

10

<td>

하트 비트 실행 프로그램 지수 관련 기능을 다시 시작합니다. 일련의 시간 초과가 발생한 경우 재시도 지연에 대한 최대 배율 값입니다.





<td>

eureka.client.heartbeat-executor-thread-pool-size

<td>

2

<td>

heartbeatExecutor가 초기화 할 스레드 풀 크기





<td>

eureka.client.initial-instance-info-replication-interval-seconds

<td>

40

<td>

인스턴스 정보를 유레카 서버에 복제하는 데 걸리는 시간 (초)을 나타냅니다.





<td>

eureka.client.instance-info-replication-interval-seconds

<td>

30

<td>

유레카 서버에 복제본을 복제하는 빈도 (초)를 나타냅니다.





<td>

eureka.client.log-delta-diff

<td>

그릇된

<td>

레지스트리 정보의 관점에서 유레카 서버와 유레카 클라이언트 간의 차이를 기록할지 여부를 나타냅니다.

유레카 클라이언트는 네트워크 트래픽을 최소화하기 위해 유레카 서버에서 델타 변경 사항 만 검색하려고합니다. 델타를받은 후, 유레카 클라이언트는 서버에서 정보를 조정하여 정보가 누락되지 않았 음을 확인합니다. 조정 실패는 클라이언트가 서버와 통신하는 네트워크 문제를 가지고있을 때 발생할 수 있습니다. 조정이 실패하면 유레카 클라이언트는 전체 레지스트리 정보를 가져옵니다.

전체 레지스트리 정보를 얻는 동안 유레카 클라이언트는 클라이언트와 서버 간의 차이점을 기록 할 수 있으며이 설정은이를 제어합니다.

변경 사항은 registryFetchIntervalSecondsr에 지정된 다음 레지스트리 페치 사이클에서 런타임에 유효합니다.





<td>

eureka.client.on-demand-update-status-change

<td>

참된

<td>

true로 설정하면 ApplicationInfoManager를 통한 로컬 상태 업데이트가 원격 유레카 서버에 대한 주문형 (속도 제한적) 등록 / 업데이트를 트리거합니다





<td>

eureka.client.prefer-same-zone-eureka

<td>

참된

<td>

이 인스턴스가 대기 시간 및 / 또는 다른 이유로 같은 영역에서 유레카 서버를 사용하려고 시도해야하는지 여부를 나타냅니다.

이상적으로 유레카 클라이언트는 동일한 영역에있는 서버와 통신하도록 구성됩니다.

변경 사항은 런타임에 registryFetchIntervalSeconds에 지정된 다음 레지스트리 페치 사이클에서 유효합니다.





<td>

eureka.client.property-resolver





<td>

eureka.client.proxy-host

<td>

존재하는 경우 유레카 서버에 대한 프록시 호스트를 가져옵니다.





<td>

eureka.client.proxy-password

<td>

프록시 암호가 있으면 가져옵니다.





<td>

eureka.client.proxy-port

<td>

존재하는 경우 유레카 서버에 대한 프록시 포트를 가져옵니다.





<td>

eureka.client.proxy-user-name

<td>

프록시 사용자 이름이 있으면 가져옵니다.





<td>

eureka.client.region

<td>

우리 동쪽 1

<td>

이 인스턴스가있는 지역 (AWS 데이터 센터에서 사용됨)을 가져옵니다.





<td>

eureka.client.register-with-eureka

<td>

참된

<td>

이 인스턴스가 다른 사용자가 발견 할 수 있도록 유레카 서버에 정보를 등록해야하는지 여부를 나타냅니다.

경우에 따라 인스턴스를 검색하는 대신 다른 인스턴스를 검색하기를 원할 수도 있습니다.





<td>

eureka.client.registry-fetch-interval-seconds

<td>

30

<td>

유레카 서버에서 레지스트리 정보를 가져 오는 빈도 (초)를 나타냅니다.





<td>

eureka.client.registry-refresh-single-vip-address

<td>

클라이언트가 단일 VIP에 대한 레지스트리 정보에만 관심이 있는지 여부를 나타냅니다.





<td>

eureka.client.service-url

<td>

유레카 서버와 통신 할 수있는 완전한 URL 목록에 가용 영역을 매핑합니다. 각 값은 단일 URL이거나 쉼표로 구분 된 대체 위치 목록 일 수 있습니다.

일반적으로 유레카 서버 URL은 프로토콜, 호스트, 포트, 컨텍스트 및 버전 정보 (있을 경우)를 전달합니다. 예 : [http://ec2-256-156-243-129.compute-1.amazonaws.com:7001/eureka/](http://ec2-256-156-243-129.compute-1.amazonaws.com:7001/eureka/)

변경 사항은 eurekaServiceUrlPollIntervalSeconds에 지정된 다음 서비스 URL 새로 고침주기에서 런타임에 유효합니다.





<td>

eureka.client.transport





<td>

eureka.client.use-dns-for-fetching-service-urls

<td>

그릇된

<td>

유레카 클라이언트가 DNS 메커니즘을 사용하여 대화 할 유레카 서버 목록을 가져와야하는지 여부를 나타냅니다. DNS 이름이 추가 서버를 갖도록 업데이트되면 eurekaServiceUrlPollIntervalSeconds에 지정된대로 해당 정보를 유레카 클라이언트가 폴링 한 직후에 해당 정보가 사용됩니다.

또는 service url이 serviceUrls로 반환 될 수 있지만 변경 사항이 발생할 경우 업데이트 된 목록을 반환하는 자체 메커니즘을 구현해야합니다.

변경 사항은 런타임에 효과적입니다.





<td>

eureka.dashboard.enabled

<td>

참된

<td>

유레카 대시 보드를 사용하도록 설정합니다. 기본값은 true입니다.





<td>

eureka.dashboard.path

<td>

/

<td>

유레카 대시 보드에 대한 경로입니다 (서블릿 경로 기준). 기본값은 "/"입니다.





<td>

eureka.instance.a-sgname

<td>

이 인스턴스에 연결된 AWS 자동 확장 그룹 이름을 가져옵니다. 이 정보는 AWS 환경에서 인스턴스가 시작된 후 자동으로 인스턴스를 서비스에 넣고 트래픽이 비활성화 된 경우에 사용됩니다.





<td>

eureka.instance.app-group-name

<td>

eureka에 등록 할 응용 프로그램 그룹의 이름을 가져옵니다.





<td>

eureka.instance.appname

<td>

알 수 없는

<td>

eureka에 등록 할 신청서의 이름을 받으십시오.





<td>

eureka.instance.data-center-info

<td>

이 인스턴스가 배치 된 데이터 센터를 반환합니다. 이 정보는 인스턴스가 AWS에 배포 된 경우 AWS 특정 인스턴스 정보를 가져 오는 데 사용됩니다.





<td>

eureka.instance.default-address-resolution-order

<td>

[]





<td>

eureka.instance.health-check-url

<td>

이 인스턴스의 절대 상태 확인 페이지 URL을 가져옵니다. 상태 확인 페이지가 유레카와 동일한 인스턴스에있는 경우 사용자가 healthCheckUrlPath를 제공 할 수 있습니다. 인스턴스가 다른 서버의 프록시 인 경우 사용자가 전체 URL을 제공 할 수 있습니다. 전체 URL이 제공되면 우선 순위가 부여됩니다.

<p> 일반적으로 인스턴스의 상태에 따라 의사 결정을 내리는 데 사용됩니다. 예를 들어 전체 팜에 배포를 진행할지 또는 더 이상 손상을주지 않고 배포를 중지할지 여부를 결정하는 데 사용할 수 있습니다. 전체 URL은 [http : // $ {eureka.hostname} : 7001 /](http://%24%7Beureka.hostname%7D:7001/) 형식을 따라야합니다 [.](http://%24%7Beureka.hostname%7D:7001/) 여기서 $ {eureka.hostname} 값은 런타임에 대체됩니다.





<td>

eureka.instance.health-check-url-path

<td>

/건강

<td>

이 인스턴스의 상대 상태 확인 URL 경로를 가져옵니다. 그런 다음 상태 확인 페이지 URL은 securePort 및 nonSecurePort에 지정된대로 보안 또는 비보안 인 호스트 이름 및 통신 유형으로 구성됩니다.

이는 일반적으로 인스턴스의 상태에 따라 교육 된 의사 결정을 내리는 데 사용됩니다. 예를 들어 전체 팜에 배포를 진행할지 또는 더 이상 손상을주지 않고 배포를 중지할지 여부를 결정하는 데 사용할 수 있습니다.





<td>

eureka.instance.home-page-url

<td>

이 인스턴스의 절대 홈 페이지 URL을 가져옵니다. 사용자가 홈 페이지가 eureka와 동일한 인스턴스에있는 경우 homePageUrlPath를 제공 할 수 있습니다. 인스턴스가 다른 서버의 프록시 인 경우 사용자가 전체 URL을 제공 할 수 있습니다. 전체 URL이 제공되면 우선 순위가 부여됩니다.

일반적으로 다른 서비스에서 방문 페이지로 사용하기 위해 정보 용도로 사용됩니다. 전체 URL은 [http : // $ {eureka.hostname} : 7001 /](http://%24%7Beureka.hostname%7D:7001/) 형식을 따라야하며 여기서 $ {eureka.hostname} 값은 런타임에 대체됩니다.





<td>

eureka.instance.home-page-url-path

<td>

/

<td>

이 인스턴스의 상대적 홈 페이지 URL 경로를 가져옵니다. 홈 페이지 URL은 hostName 및 통신 유형 (안전 또는 비보안)으로 구성됩니다.

일반적으로 다른 서비스에서 방문 페이지로 사용하기 위해 정보 용도로 사용됩니다.





<td>

eureka.instance.host-info





<td>

eureka.instance.hostname

<td>

구성 시간에 결정될 수있는 경우 호스트 이름입니다 (그렇지 않으면 OS 프리미티브에서 추측됩니다).





<td>

eureka.instance.inet-utils





<td>

eureka.instance.initial-status

<td>

rmeote 유레카 서버에 등록 할 초기 상태입니다.





<td>

eureka.instance.instance-enabled-onit

<td>

그릇된

<td>

eureka에 등록 된 즉시 인스턴스를 사용할 수 있는지 여부를 나타냅니다. 경우에 따라 트래픽을 처리 할 준비가되기 전에 애플리케이션에서 사전 처리 작업을 수행해야하는 경우가 있습니다.





<td>

eureka.instance.instance-id

<td>

eureka에 등록 할이 인스턴스의 고유 ID (appName 범위 내에 있음)를 가져옵니다.





<td>

eureka.instance.ip-address

<td>

인스턴스의 IPAdress를 가져옵니다. 이 정보는 다른 인스턴스의 통신이 주로 {@link #getHostName (boolean)}에 제공된 정보를 사용하여 발생하기 때문에 학업 목적으로 만 사용됩니다.





<td>

eureka.instance.lease-expiration-duration-in-seconds

<td>

90

<td>

뷰에서이 인스턴스를 제거하기 전에 마지막 하트 비트를 수신 한 이후 유레카 서버가 대기하는 시간 (초)을 나타내며이 인스턴스에 대한 트래픽을 허용하지 않음으로써 시간을 나타냅니다.

이 값을 너무 길게 설정하면 인스턴스가 활성 상태가 아니더라도 트래픽이 인스턴스로 라우팅 될 수 있습니다. 이 값을 너무 작게 설정하면 임시 네트워크 결함으로 인해 인스턴스가 트래픽에서 벗어날 수 있습니다.이 값은 leaseRenewalIntervalInSeconds에 지정된 값보다 적어도 더 높게 설정해야합니다.





<td>

eureka.instance.lease-renewal-interval-in-seconds

<td>

30

<td>

유레카 클라이언트가 아직 살아 있음을 나타 내기 위해 유레카 서버에 하트 비트를 보내는 빈도 (초)를 나타냅니다. leaseExpirationDurationInSeconds에 지정된 기간 동안 하트 비트가 수신되지 않으면 eureka 서버는이 인스턴스에 대한 트래픽을 허용하지 않음으로써 뷰에서 해당 인스턴스를 제거합니다.

HealthCheckCallback을 구현하고 인스턴스를 사용할 수 없도록 결정하면 인스턴스에서 트래픽을 가져올 수 없습니다.





<td>

eureka.instance.metadata-map

<td>

이 인스턴스와 관련된 메타 데이터 이름 / 값 쌍을 가져옵니다. 이 정보는 eureka 서버로 전송되며 다른 인스턴스에서 사용할 수 있습니다.





<td>

eureka.instance.namespace

<td>

유레카

<td>

속성을 찾는 데 사용되는 네임 스페이스를 가져옵니다. Spring Cloud에서는 무시됩니다.





<td>

eureka.instance.non-secure-port

<td>

80

<td>

인스턴스가 트래픽을 수신해야하는 비보안 포트를 가져옵니다.





<td>

eureka.instance.non-secure-port-enabled

<td>

참된

<td>

비보안 포트를 트래픽에 사용할 수 있는지 여부를 나타냅니다.





<td>

eureka.instance.prefer-ip-address

<td>

그릇된

<td>

호스트 이름을 추측 할 때 서버의 IP 주소를 OS가보고하는 호스트 이름을 기준으로 사용해야한다고 말하는 플래그입니다.





<td>

eureka.instance.secure-health-check-url

<td>

이 인스턴스의 절대 보안 상태 확인 페이지 URL을 가져옵니다. 사용자는 health check 페이지가 eureka와 통신하는 동일한 인스턴스에 상주하는 경우 secureHealthCheckUrl을 제공 할 수 있으며 인스턴스가 다른 서버의 프록시 인 경우 사용자가 전체 URL을 제공 할 수 있습니다. 전체 URL이 제공되면 우선 순위가 부여됩니다.

<p> 일반적으로 인스턴스의 상태에 따라 의사 결정을 내리는 데 사용됩니다. 예를 들어 전체 팜에 배포를 진행할지 또는 더 이상 손상을주지 않고 배포를 중지할지 여부를 결정하는 데 사용할 수 있습니다. 전체 URL은 [http : // $ {eureka.hostname} : 7001 /](http://%24%7Beureka.hostname%7D:7001/) 형식을 따라야합니다 [.](http://%24%7Beureka.hostname%7D:7001/) 여기서 $ {eureka.hostname} 값은 런타임에 대체됩니다.





<td>

eureka.instance.secure-port

<td>

443

<td>

인스턴스가 트래픽을 수신해야하는 보안 포트를 가져옵니다.





<td>

eureka.instance.secure-port-enabled

<td>

그릇된

<td>

보안 포트가 트래픽에 대해 활성화되어야하는지 여부를 나타냅니다.





<td>

eureka.instance.secure-virtual-host-name

<td>

이 인스턴스에 대해 정의 된 보안 가상 호스트 이름을 가져옵니다.

이것은 일반적으로 다른 인스턴스가 보안 가상 호스트 이름을 사용하여이 인스턴스를 찾는 방식입니다. 정규화 된 도메인 이름과 유사하게 서비스 사용자가이 인스턴스를 찾아야합니다.





<td>

eureka.instance.status-page-url

<td>

이 인스턴스의 절대 상태 페이지 URL 경로를 가져옵니다. 상태 페이지가 유레카와 동일한 인스턴스에있는 경우 사용자가 statusPageUrlPath를 제공 할 수 있습니다. 인스턴스가 다른 서버의 프록시 인 경우 사용자가 전체 URL을 제공 할 수 있습니다. 전체 URL이 제공되면 우선 순위가 부여됩니다.

이것은 일반적으로 다른 서비스가이 인스턴스의 상태를 찾기 위해 정보를 제공하기 위해 사용됩니다. 사용자는 인스턴스의 현재 상태를 나타내는 간단한 HTML을 제공 할 수 있습니다.





<td>

eureka.instance.status-page-url-path

<td>

/ 정보

<td>

이 인스턴스의 상대 상태 페이지 URL 경로를 가져옵니다. 상태 페이지 URL은 hostName 및 통신 유형 (securePort 및 nonSecurePort에 지정된대로 보안 또는 비보안)으로 구성됩니다.

이것은 일반적으로 다른 서비스가이 인스턴스의 상태를 찾기 위해 정보를 제공하기 위해 사용됩니다. 사용자는 인스턴스의 현재 상태를 나타내는 간단한 HTML을 제공 할 수 있습니다.





<td>

eureka.instance.virtual-host-name

<td>

이 인스턴스에 대해 정의 된 가상 호스트 이름을 가져옵니다.

이것은 일반적으로 다른 인스턴스가 가상 호스트 이름을 사용하여이 인스턴스를 찾는 방식입니다. 정규화 된 도메인 이름과 비슷한 것으로 생각하면 서비스 사용자가이 인스턴스를 찾아야합니다.





<td>

eureka.server.a-sgcache-expiry-timeout-ms

<td>

0





<td>

eureka.server.a-sgquery-timeout-ms

<td>

300





<td>

eureka.server.a-sgupdate-interval-ms

<td>

0





<td>

eureka.server.a-wsaccess-id





<td>

eureka.server.a-wssecret-key





<td>

eureka.server.batch-replication

<td>

그릇된





<td>

eureka.server.binding-strategy





<td>

eureka.server.delta-retention-timer-interval-in-ms

<td>

0





<td>

eureka.server.disable-delta

<td>

그릇된





<td>

eureka.server.disable-delta-for-remote-regions

<td>

그릇된





<td>

eureka.server.disable-transparent-fallback-to-other-region

<td>

그릇된





<td>

eureka.server.e-ipbind-rebind-retries

<td>

삼





<td>

eureka.server.e-ipbinding-retry-interval-ms

<td>

0





<td>

eureka.server.e-ipbinding-retry-interval-ms-when-unbound

<td>

0





<td>

eureka.server.enable-replicated-request-compression

<td>

그릇된





<td>

eureka.server.enable-self-preservation

<td>

참된





<td>

eureka.server.eviction-interval-timer-in-ms

<td>

0





<td>

eureka.server.g-zip-content-from-remote-region

<td>

참된





<td>

eureka.server.json-codec-name





<td>

eureka.server.list-auto-scaling-groups-role-name

<td>

ListAutoScalingGroups





<td>

eureka.server.log-identity-headers

<td>

참된





<td>

eureka.server.max-elements-in-peer-replication-pool

<td>

10000





<td>

eureka.server.max-elements-in-status-replication-pool

<td>

10000





<td>

eureka.server.max-idle-thread-age-in-peer-replication을위한 시간

<td>

15 명





<td>

eureka.server.max-idle-thread-in-minutes-status-for-status-replication

<td>

10





<td>

eureka.server.max-threads-for-peer-replication

<td>

20





<td>

eureka.server.max-status-replication 용 스레드

<td>

1





<td>

eureka.server.max-time-for-replication

<td>

30000





<td>

eureka.server.min-threads-for-peer-replication

<td>

5





<td>

eureka.server.min-threads-status-replication

<td>

1





<td>

eureka.server.number-of-replication-retries

<td>

5





<td>

eureka.server.peer-eureka-nodes-update-interval-ms

<td>

0





<td>

eureka.server.peer-eureka-status-refresh-time-interval-ms

<td>

0





<td>

eureka.server.peer-node-connect-timeout-ms

<td>

200





<td>

eureka.server.peer-node-connection-idle-timeout-seconds

<td>

30





<td>

eureka.server.peer-node-read-timeout-ms

<td>

200





<td>

eureka.server.peer-node-total-connections

<td>

1000





<td>

eureka.server.peer-node-total-connections-per-host

<td>

500





<td>

eureka.server.prime-aws-replica-connections

<td>

참된





<td>

eureka.server.property-resolver





<td>

eureka.server.rate-limiter-burst-size

<td>

10





<td>

eureka.server.rate-limiter-enabled

<td>

그릇된





<td>

eureka.server.rate-limiter-full-fetch-average-rate

<td>

100





<td>

eureka.server.rate-limiter-privileged-clients





<td>

eureka.server.rate-limiter-registry-fetch-average-rate

<td>

500





<td>

eureka.server.rate-limiter-throttle-standard-clients

<td>

그릇된





<td>

eureka.server.registry-sync-retries

<td>

0





<td>

eureka.server.registry-sync-retry-wait-ms

<td>

0





<td>

eureka.server.remote-region-app-whitelist





<td>

eureka.server.remote-region-connect-timeout-ms

<td>

1000





<td>

eureka.server.remote-region-connection-idle-timeout-seconds

<td>

30





<td>

eureka.server.remote-region-fetch-thread-pool-size

<td>

20





<td>

eureka.server.remote-region-read-timeout-ms

<td>

1000





<td>

eureka.server.remote-region-registry-fetch-interval

<td>

30





<td>

eureka.server.remote-region-total-connections

<td>

1000





<td>

eureka.server.remote-region-total-connections-per-host

<td>

500





<td>

eureka.server.remote-region-trust-store





<td>

eureka.server.remote-region-trust-store-password

<td>

changeit





<td>

eureka.server.remote-region-urls





<td>

eureka.server.remote-region-urls-with-name





<td>

eureka.server.renewal-percent-threshold

<td>

0.85





<td>

eureka.server.renewal-threshold-update-interval-ms

<td>

0





<td>

eureka.server.response-cache-auto-expiration-in-seconds

<td>

180





<td>

eureka.server.response-cache-update-interval-ms

<td>

0





<td>

eureka.server.retention-time-in-msin-delta-queue

<td>

0





<td>

eureka.server.route53-bind-rebind-retries

<td>

삼





<td>

eureka.server.route53-binding-retry-interval-ms

<td>

0





<td>

eureka.server.route53-domain-ttl

<td>

30





<td>

eureka.server.sync-when-timestamp-different

<td>

참된





<td>

eureka.server.use-read-only-response-cache

<td>

참된





<td>

eureka.server.wait-time-in-ms-when-sync-empty

<td>

0





<td>

eureka.server.xml-codec-name





<td>

feign.compression.request.mime-types

<td>

[text / xml, application / xml, application / json]

<td>

지원되는 MIME 유형 목록.





<td>

feign.compression.request.min-request-size

<td>

2048

<td>

최소 임계 값 콘텐츠 크기





<td>

health.config.enabled

<td>

그릇된

<td>

구성 서버 상태 표시기를 설치해야 함을 표시하는 플래그.





<td>

health.hystrix.enabled

<td>

그릇된

<td>

hystrix 상태 표시기가 설치되어 있는지 확인하십시오.





<td>

netflix.atlas.batch-size

<td>

10000





<td>

netflix.atlas.enabled

<td>

참된





<td>

netflix.atlas.uri





<td>

proxy.auth.load-balanced

<td>

그릇된





<td>

프록시 .auth.routes

<td>

경로 별 인증 전략.





<td>

spring.cloud.bus.ack.destination-service

<td>

멍청한 말을 듣고 싶어하는 서비스. 기본적으로 null입니다 (모든 서비스를 의미 함).





<td>

spring.cloud.bus.ack.enabled

<td>

참된

<td>

acks를 끄기위한 플래그 (기본값은 켜짐).





<td>

spring.cloud.bus.destination

<td>

springCloudBus

<td>

메시지에 대한 Spring Cloud Stream 대상의 이름.





<td>

spring.cloud.bus.enabled

<td>

참된

<td>

버스가 활성화되었음을 나타내는 플래그입니다.





<td>

spring.cloud.bus.env.enabled

<td>

참된

<td>

환경 변경 이벤트를 끄기위한 플래그입니다 (기본값은 켜짐).





<td>

spring.cloud.bus.refresh.enabled

<td>

참된

<td>

새로 고침 이벤트를 끄기 위해 플래그를 설정합니다 (기본 설정).





<td>

spring.cloud.bus.trace.enabled

<td>

그릇된

<td>

acks의 추적을 켜기 위해 플래그를 설정합니다 (기본값은 off).





<td>

spring.cloud.cloudfoundry.discovery.email

<td>

인증 할 사용자의 전자 메일 주소입니다.





<td>

spring.cloud.cloudfoundry.discovery.enabled

<td>

참된

<td>

발견이 가능함을 나타내는 플래그.





<td>

spring.cloud.cloudfoundry.discovery.password

<td>

사용자가 토큰을 인증하고 획득하기위한 암호입니다.





<td>

spring.cloud.cloudfoundry.discovery.url

<td>

[https://api.run.pivotal.io](https://api.run.pivotal.io/)

<td>

Cloud Foundry API (Cloud Controller)의 URL입니다.





<td>

spring.cloud.config.allow-override

<td>

참된

<td>

{isSystemPropertiesOverride () systemPropertiesOverride}를 사용할 수있는 것을 나타내는 플래그입니다. 사용자가 실수로 기본값을 변경하지 못하게하려면 false로 설정하십시오. 기본값은 true입니다.





<td>

spring.cloud.config.discovery.enabled

<td>

그릇된

<td>

설정 서버 검색이 활성화되었음을 나타 내기 위해 플래그를 지정합니다 (검색을 통해 구성 서버 URL이 조회됩니다).





<td>

spring.cloud.config.discovery.service-id

<td>

CONFIGSERVER

<td>

구성 서버를 찾기위한 서비스 ID.





<td>

spring.cloud.config.enabled

<td>

참된

<td>

원격 구성이 활성화되었다고 알리는 플래그. 기본값은 true입니다.





<td>

spring.cloud.config.fail-fast

<td>

그릇된

<td>

서버에 연결하지 못하는 것이 치명적임을 나타내는 플래그입니다 (기본값은 false).





<td>

spring.cloud.config.label

<td>

원격 구성 등록 정보를 가져 오는 데 사용할 레이블 이름입니다. 기본값은 서버에서 설정됩니다 (일반적으로 자식 기반 서버의 경우 "마스터").





<td>

spring.cloud.config.name

<td>

원격 등록 정보를 가져 오는 데 사용되는 응용 프로그램의 이름입니다.





<td>

spring.cloud.config.override-none

<td>

그릇된

<td>

#setAllowOverride (boolean) allowOverride}가 true의 경우, 외부 프로퍼티의 우선 순위는 낮아, 기존의 프로퍼티 소스 (로컬 설정 파일을 포함한다)는 오버라이드 (override)하지 말아주세요. 기본값은 false입니다.





<td>

overclock.config -override-system-properties

<td>

참된

<td>

외부 프로퍼티가 시스템 프로퍼티를 오버라이드 (override)하는 것을 나타내는 플래그입니다. 기본값은 true입니다.





<td>

spring.cloud.config.password

<td>

원격 서버에 연결할 때 사용할 암호 (HTTP 기본)입니다.





<td>

spring.cloud.config.profile

<td>

태만

<td>

원격 구성을 가져올 때 사용할 기본 프로파일 (쉼표로 구분). 기본값은 "default"입니다.





<td>

spring.cloud.config.retry.initial-interval

<td>

1000

<td>

초기 재시도 간격 (밀리 초).





<td>

spring.cloud.config.retry.max-attempts

<td>

6

<td>

최대 시도 횟수.





<td>

spring.cloud.config.retry.max-interval

<td>

2000 년

<td>

백 오프의 최대 간격.





<td>

spring.cloud.config.retry.multiplier

<td>

1.1

<td>

다음 간격의 배율입니다.





<td>

spring.cloud.config.uri

<td>

[http : // localhost : 8888](http://localhost:8888/)

<td>

원격 서버의 URI (기본값 [http : // localhost : 8888](http://localhost:8888/) ).





<td>

spring.cloud.config.username

<td>

원격 서버에 연결할 때 사용할 사용자 이름 (HTTP 기본)입니다.





<td>

spring.cloud.consul.config.acl-token





<td>

spring.cloud.consul.config.data-key

<td>

데이터

<td>

형식이 Format.PROPERTIES 또는 Format.YAML 인 경우 다음 필드가 구성 용 영사를 조회하는 키로 사용됩니다.





<td>

spring.cloud.consul.config.default-context

<td>

신청





<td>

spring.cloud.consul.config.enabled

<td>

참된





<td>

spring.cloud.consul.config.fail-fast

<td>

참된

<td>

true이면 설정 조회 중에 예외를 던지고, 그렇지 않으면 경고를 남깁니다.





<td>

spring.cloud.consul.config.format





<td>

spring.cloud.consul.config.prefix

<td>

구성





<td>

spring.cloud.consul.config.profile-separator

<td>

,





<td>

spring.cloud.consul.config.watch.delay

<td>

10





<td>

spring.cloud.consul.config.watch.enabled

<td>

참된





<td>

spring.cloud.consul.config.watch.wait-time

<td>

2





<td>

spring.cloud.consul.discovery.acl-token





<td>

spring.cloud.consul.discovery.catalog-services-watch-delay

<td>

10





<td>

spring.cloud.consul.discovery.catalog-services-watch-timeout

<td>

2





<td>

spring.cloud.consul.discovery.enabled

<td>

참된

<td>

서비스 검색이 활성화되어 있습니까?





<td>

health.chealth- check- interval.consul.discovery.health-check-interval

<td>

10 대

<td>

상태 확인을 수행하는 빈도 (예 : 10 초)





<td>

건강 검진을위한 spring.cloud.consul.discovery.health-check-path

<td>

/건강

<td>

상태 확인을 위해 호출 할 대체 서버 경로





<td>

health.chealth- check-timeout

<td>

상태 확인 제한 시간 (예 : 10 초)





<td>

health.chealth-check-url

<td>

기본 설정을 무시할 수있는 사용자 정의 상태 확인 URL





<td>

spring.cloud.consul.discovery.heartbeat.enabled

<td>

그릇된





<td>

봄. 클라우드. 회의. 디스커버리. 하트 비트. 하트 비트 인터벌





<td>

spring.cloud.consul.discovery.heartbeat.interval-ratio





<td>

하트 비트 .ttl- 유닛

<td>

에스





<td>

심장 박동. 심박계. 심장 박동. 가치 - 가치

<td>

30





<td>

spring.cloud.consul.discovery.host-info





<td>

spring.cloud.consul.discovery.hostname

<td>

서버에 액세스 할 때 사용할 호스트 이름





<td>

spring.cloud.consul.discovery.instance-id

<td>

고유 서비스 인스턴스 ID





<td>

spring.cloud.consul.discovery.ip-address

<td>

서비스에 액세스 할 때 사용할 IP 주소 (사용하려면 preferIpAddress도 설정해야 함)





<td>

spring.cloud.consul.discovery.lifecycle.enabled

<td>

참된





<td>

spring.cloud.consul.discovery.management-suffix

<td>

조치

<td>

관리 서비스 등록시 사용할 접미사





<td>

spring.cloud.consul.discovery.management-tags

<td>

관리 서비스를 등록 할 때 사용할 태그





<td>

spring.cloud.consul.discovery.port

<td>

서비스를 등록 할 포트 (기본값은 수신 대기 포트)





<td>

spring.cloud.consul.discovery.prefer-agent-address

<td>

그릇된

<td>

사용할 주소를 결정하는 방법의 출처





<td>

spring.cloud.consul.discovery.prefer-ip-address

<td>

그릇된

<td>

등록하는 동안 호스트 이름 대신 IP 주소 사용





<td>

질문. 통과.

<td>

그릇된

<td>

/ v1 / health / service / serviceName에 'passing'매개 변수를 추가하십시오. 이렇게하면 상태 검사가 서버로 전달됩니다.





<td>

spring.cloud.consul.discovery.register

<td>

참된

<td>

영사 서비스에 등록하십시오.





<td>

spring.cloud.consul.discovery.register-health-check

<td>

참된

<td>

영사관에 건강 검진을 등록하십시오. 서비스 개발 중에 유용합니다.





<td>

spring.cloud.consul.discovery.scheme

<td>

http

<td>

http 또는 https 서비스 등록 여부





<td>

spring.cloud.consul.discovery.server-list-query-tags

<td>

serviceId의 → 서버 목록에서 쿼리 할 태그. 이를 통해 단일 태그로 서비스를 필터링 할 수 있습니다.





<td>

spring.cloud.consul.discovery.service-name

<td>

서비스 이름





<td>

spring.cloud.consul.discovery.tags

<td>

서비스 등록시 사용할 태그





<td>

spring.cloud.consul.enabled

<td>

참된

<td>

봄 구름 영사가 가능합니까?





<td>

spring.cloud.consul.host

<td>

로컬 호스트

<td>

총영사관 호스트 이름. 기본값은 'localhost'입니다.





<td>

spring.cloud.consul.port

<td>

8500

<td>

영사관 요원. 기본값은 '8500'입니다.





<td>

봄철. 초. 중. 재시별 - 간격

<td>

1000

<td>

초기 재시도 간격 (밀리 초).





<td>

spring.cloud.consul.retry.max-attempts

<td>

6

<td>

최대 시도 횟수.





<td>

spring.cloud.consul.retry.max-interval

<td>

2000 년

<td>

백 오프의 최대 간격.





<td>

.retry.multiplier

<td>

1.1

<td>

다음 간격의 배율입니다.





<td>

spring.cloud.hypermedia.refresh.fixed-delay

<td>

5000





<td>

초기 지연 - spring.cloud.hypermedia.refresh.it

<td>

10000





<td>

spring.cloud.inetutils.default-hostname

<td>

로컬 호스트

<td>

기본 호스트 이름. 오류가 발생한 경우에 사용됩니다.





<td>

spring.cloud.inetutils.default-ip-address

<td>

127.0.0.1

<td>

기본 ipaddress입니다. 오류가 발생한 경우에 사용됩니다.





<td>

spring.cloud.inetutils.ignored-interfaces

<td>

무시 될 네트워크 인터페이스의 Java 정규 표현식 목록입니다.





<td>

spring.cloud.inetutils.timeout-seconds

<td>

1

<td>

호스트 이름을 계산하기위한 시간 제한 (초).





<td>

spring.cloud.stream.binders





<td>

spring.cloud.stream.bindings





<td>

spring.cloud.stream.consumer-defaults





<td>

spring.cloud.stream.default-binder





<td>

spring.cloud.stream.dynamic-destinations

<td>

[]





<td>

Spring.cloud.stream.ignore-unknown-properties

<td>

참된





<td>

spring.cloud.stream.instance-count

<td>

1





<td>

spring.cloud.stream.instance-index

<td>

0





<td>

spring.cloud.stream.producer-defaults





<td>

spring.cloud.stream.rabbit.binder.addresses

<td>

[]





<td>

spring.cloud.stream.rabbit.binder.admin-adresses

<td>

[]





<td>

spring.cloud.stream.rabbit.binder.com 노출 수준

<td>

0





<td>

spring.cloud.stream.rabbit.binder.nodes

<td>

[]





<td>

spring.cloud.stream.rabbit.binder.password





<td>

spring.cloud.stream.rabbit.binder.ssl-properties-location





<td>

spring.cloud.stream.rabbit.binder.use-ssl

<td>

그릇된





<td>

spring.cloud.stream.rabbit.binder.username





<td>

spring.cloud.stream.rabbit.binder.vhost





<td>

spring.cloud.stream.rabbit.bindings





<td>

spring.cloud.zookeeper.default-health-endpoint

<td>

종속성이 있는지 확인하기 위해 검사 할 기본 상태 종점





<td>

스프링클러. 주키퍼.

<td>

ZookeeperDependency에 대한 별칭 매핑. Ribbon은 serviceID에 중첩 된 구조를 허용 할 수 없기 때문에 실제로 별칭은 serviceID입니다.





<td>

spring.cloud.zookeeper.dependency-configurations





<td>

spring.cloud.zookeeper.dependency-names





<td>

spring.cloud.zookeeper.discovery.enabled

<td>

참된





<td>

spring.cloud.zookeeper.discovery.instance-host





<td>

spring.cloud.zookeeper.discovery.metadata

<td>

이 인스턴스와 관련된 메타 데이터 이름 / 값 쌍을 가져옵니다. 이 정보는 사육사에게 보내어 다른 인스턴스에서 사용할 수 있습니다.





<td>

spring.cloud.zookeeper.discovery.root

<td>

/서비스





<td>

spring.cloud.zookeeper.discovery.uri-spec

<td>

{scheme} : // {address} : {port}





<td>

spring.cloud.zookeeper.prefix

<td>

모든 사육사 의존성 경로에 적용되는 공통 접두사





<td>

spring.integration.poller.fixed-delay

<td>

1000

<td>

기본 폴러에 대한 고정 지연.





<td>

spring.integration.poller.max-poll-poll

<td>

1

<td>

기본 폴러에 대한 폴링 당 최대 메시지 수.





<td>

spring.sleuth.keys.async.class-name-key

<td>

수업

<td>

비동기 프로세스가 시작된 @Async} 주석이있는 메소드가있는 클래스의 단순한 이름입니다.

@see org.springframework.scheduling.annotation.Async를 참조하십시오.





<td>

spring.sleuth.keys.async.method-name-key

<td>

방법

<td>

@Async}로 주석 첨부 된 메소드의 이름

@see org.springframework.scheduling.annotation.Async를 참조하십시오.





<td>

spring.sleuth.keys.async.prefix

<td>

헤더 이름이 태그로 추가되는 경우 접두사.





<td>

spring.sleuth.keys.async.thread-name-key

<td>

실

<td>

비동기 메소드를 실행 한 스레드의 이름입니다.

@see org.springframework.scheduling.annotation.Async를 참조하십시오.





<td>

spring.sleuth.keys.http.headers

<td>

태그가 있으면 추가해야하는 추가 헤더입니다. 헤더 값이 여러 값인 경우 태그 값은 쉼표로 구분 된 작은 따옴표 목록입니다.





<td>

spring.sleuth.keys.http.host

<td>

http.host

<td>

URL 또는 호스트 헤더의 도메인 부분. 예 : "mybucket.s3.amazonaws.com". IP 주소와 대조적으로 호스트별로 필터링하는 데 사용됩니다.





<td>

spring.sleuth.keys.http.method

<td>

http.method

<td>

HTTP 메소드 또는 동사 (예 : "GET"또는 "POST"). http 경로를 기준으로 필터링하는 데 사용됩니다.





<td>

spring.sleuth.keys.http.path

<td>

http.path

<td>

쿼리 매개 변수없이 절대 http 경로. 예 : "/ objects / abcd-ff". zipkin v1을 사용하여 http 경로에 대해 필터링하는 데 사용됩니다. zipkin v1에서는 equals 필터 만 지원됩니다. 쿼리 매개 변수를 삭제하면 고유 URI 수가 줄어 듭니다. 예를 들어, 쿼리 라인에 인코딩 된 서명 매개 변수와 상관없이 동일한 리소스를 쿼리 할 수 ​​있습니다. 이렇게하면 HTTP 단일 경로의 카디널리티가 줄어들지 않습니다. 예를 들어 경로를 "/ resource / {resource_id}"와 같은 http URI 템플릿으로 표현하는 것이 일반적입니다. equals 쿼리 만 사용할 수있는 시스템에서는 실제 요청이 "/ resource / abcd-ff"인 경우 http.uri = / resource}을 검색하는 것이 일치하지 않습니다. 기록 참고 사항 : 이것은 흔히 zipkin에서 "http.uri"로 표현되었지만 대부분 경로 일뿐입니다.





<td>

spring.sleuth.keys.http.prefix

<td>

http.

<td>

헤더 이름이 태그로 추가되는 경우 접두사.





<td>

spring.sleuth.keys.http.request-size

<td>

http.request.size

<td>

비어 있지 않은 HTTP 요청 본문의 크기 (바이트)입니다. 전의. "16384"

<p> 큰 업로드는 한도를 초과하거나 대기 시간에 직접적으로 기여할 수 있습니다.





<td>

spring.sleuth.keys.http.response-size

<td>

http.response.size

<td>

비어 있지 않은 HTTP 응답 본문의 크기 (바이트)입니다. 전의. "16384"

<p> 큰 다운로드는 한도를 초과하거나 대기 시간에 직접적으로 기여할 수 있습니다.





<td>

spring.sleuth.keys.http.status-code

<td>

http.status_code

<td>

2xx 범위가 아닌 HTTP 응답 코드입니다. 전의. "503"오류 상태를 필터링하는 데 사용됩니다. 2xx 범위는 성공 코드가 대기 시간 문제 해결에 덜 흥미 롭기 때문에 기록되지 않습니다. 생략하면 범위 당 최소 20 바이트가 절약됩니다.





<td>

spring.sleuth.keys.http.url

<td>

http.url

<td>

가능한 경우 스키마, 호스트 및 쿼리 매개 변수를 포함한 전체 URL입니다. 전의. "https://mybucket.s3.amazonaws.com/objects/abcd-ff?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Algorithm=AWS4-HMAC-SHA256..."{@link #method }를 사용하면 정규화 된 요청 행을 이해할 수 있습니다. 개인 정보가 포함되거나 상당한 기간이 소요될 수 있으므로 선택 사항입니다.





<td>

spring.sleuth.keys.hystrix.command-group

<td>

commandGroup

<td>

명령 그룹의 이름. Hystrix는 명령 그룹 키를 사용하여보고, 경고, 대시 보드 또는 팀 / 라이브러리 소유권과 같은 명령을 그룹화합니다.

@see com.netflix.hystrix.HystrixCommandGroupKey





<td>

spring.sleuth.keys.hystrix.command-key

<td>

commandKey

<td>

명령 키의 이름. 주어진 명령의 이름을 설명합니다. 모니터링, 회로 차단기, 메트릭 게시, 캐싱 및 기타 용도로 {@link com.netflix.hystrix.HystrixCommand}를 나타내는 키입니다.

@see com.netflix.hystrix.HystrixCommandKey





<td>

spring.sleuth.keys.hystrix.prefix

<td>

헤더 이름이 태그로 추가되는 경우 접두사.





<td>

spring.sleuth.keys.hystrix.thread-pool-key

<td>

threadPoolKey

<td>

스레드 풀 키의 이름입니다. 스레드 풀 키는 모니터링, 메트릭 게시, 캐싱 및 기타 용도를위한 com.netflix.hystrix.HystrixThreadPool을 나타냅니다. com.netflix.hystrix.HystrixCommand}는, com.netflix.hystrix.HystrixThreadPoolKey}에 의해 취득 된 단일의 com.netflix.hystrix.HystrixThreadPool와 관련 지을 수있어 디폴트로 설정됩니다. 에 의해 작성된 com.netflix.hystrix.HystrixCommandGroupKey를 사용해 작성된 것을 돌려줍니다.

@see com.netflix.hystrix.HystrixThreadPoolKey





<td>

spring.sleuth.keys.message.headers

<td>

태그가 있으면 추가해야하는 추가 헤더입니다. 헤더 치가 String가 아닌 경우, toString () Methods를 사용해 String에 변환됩니다.





<td>

spring.sleuth.keys.message.payload.size

<td>

메시지 / 페이로드 크기

<td>

가능한 경우 페이로드의 크기 추정입니다.





<td>

spring.sleuth.keys.message.payload.type

<td>

메시지 / 페이로드 유형

<td>

페이로드 유형입니다.





<td>

spring.sleuth.keys.message.prefix

<td>

메시지/

<td>

헤더 이름이 태그로 추가되는 경우 접두사.





<td>

spring.sleuth.metric.span.accepted-name

<td>

counter.span.accepted





<td>

spring.sleuth.metric.span.dropped-name

<td>

Counter.span.dropped





<td>

spring.sleuth.sampler.percentage

<td>

0.1

<td>

샘플링해야하는 요청의 백분율. 예 : 1.0 - 100 % 요청을 샘플링해야합니다. 정밀도는 전체 수만입니다 (즉, 추적의 0.1 %는 지원되지 않습니다).





<td>

zuul.add-proxy-headers

<td>

참된





<td>

zuul.host.max-per-route-connections

<td>

20





<td>

zuul.host.max-total-connections

<td>

200





<td>

zuul.ignore-local-service

<td>

참된





<td>

zuul.ignored-headers





<td>

zuul.ignored-patterns





<td>

zuul.ignored-services





<td>

zuul.prefix





<td>

zuul.remove-semicolon-content

<td>

참된





<td>

zuul.retryable





<td>

zuul.routes





<td>

zuul.security_headers





<td>

zuul.servlet-path



<td>

/ zuul







<td>

zuul.strip-prefix

<td>

참된





<td>

zuul.trace-request-body

<td>

참된













<script>/* <![CDATA[ */(function(d,s,a,i,j,r,l,m,t){try{l=d.getElementsByTagName('a');t=d.createElement('textarea');for(i=0;l.length-i;i++){try{a=l[i].href;s=a.indexOf('/cdn-cgi/l/email-protection');m=a.length;if(a&&s>-1&&m>28){j=28+s;s='';if(j<m){r='0x'+a.substr(j,2)|0;for(j+=2;j<m&&a.charAt(j)!='X';j+=2)s+='%'+('0'+('0x'+a.substr(j,2)^r).toString(16)).slice(-2);j++;s=decodeURIComponent(s)+a.substr(j,m-j)}t.innerHTML=s.replace(/</g,'&lt;').replace(/\>/g,'&gt;');l[i].href='mailto:'+t.value}}catch(e){}}}catch(e){}})(document);/* ]]> */</script>







![Google 번역](./spring-cloud-doc-resources/translate_24dp.png)







# 원본 텍스트





Provides an abstraction over common distributed tracing data models: traces, spans (forming a DAG), annotations, key-value annotations.









* * *
