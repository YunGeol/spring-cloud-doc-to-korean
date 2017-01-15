<div id="header">

# Spring Cloud

<div id="toc" class="toc2">

<div id="toctitle">Table of Contents</div>

*   [Features](http://projects.spring.io/spring-cloud/spring-cloud.html#_features)
*   [Cloud Native Applications](http://projects.spring.io/spring-cloud/spring-cloud.html#_cloud_native_applications)
    *   [Spring Cloud Context: Application Context Services](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_context_application_context_services)
        *   [The Bootstrap Application Context](http://projects.spring.io/spring-cloud/spring-cloud.html#_the_bootstrap_application_context)
        *   [Application Context Hierarchies](http://projects.spring.io/spring-cloud/spring-cloud.html#_application_context_hierarchies)
        *   [Changing the Location of Bootstrap Properties](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-properties)
        *   [Customizing the Bootstrap Configuration](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_bootstrap_configuration)
        *   [Customizing the Bootstrap Property Sources](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-property-sources)
        *   [Environment Changes](http://projects.spring.io/spring-cloud/spring-cloud.html#_environment_changes)
        *   [Refresh Scope](http://projects.spring.io/spring-cloud/spring-cloud.html#_refresh_scope)
        *   [Encryption and Decryption](http://projects.spring.io/spring-cloud/spring-cloud.html#_encryption_and_decryption)
        *   [Endpoints](http://projects.spring.io/spring-cloud/spring-cloud.html#_endpoints)
    *   [Spring Cloud Commons: Common Abstractions](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_commons_common_abstractions)
        *   [Spring RestTemplate as a Load Balancer Client](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_resttemplate_as_a_load_balancer_client)
        *   [Multiple RestTemplate objects](http://projects.spring.io/spring-cloud/spring-cloud.html#_multiple_resttemplate_objects)
        *   [Ignore Network Interfaces](http://projects.spring.io/spring-cloud/spring-cloud.html#ignore-network-interfaces)
*   [Spring Cloud Config](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_config)
    *   [Quick Start](http://projects.spring.io/spring-cloud/spring-cloud.html#_quick_start)
        *   [Client Side Usage](http://projects.spring.io/spring-cloud/spring-cloud.html#_client_side_usage)
    *   [Spring Cloud Config Server](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_config_server)
        *   [Environment Repository](http://projects.spring.io/spring-cloud/spring-cloud.html#_environment_repository)
        *   [Health Indicator](http://projects.spring.io/spring-cloud/spring-cloud.html#_health_indicator)
        *   [Security](http://projects.spring.io/spring-cloud/spring-cloud.html#_security)
        *   [Encryption and Decryption](http://projects.spring.io/spring-cloud/spring-cloud.html#_encryption_and_decryption_2)
        *   [Key Management](http://projects.spring.io/spring-cloud/spring-cloud.html#_key_management)
        *   [Creating a Key Store for Testing](http://projects.spring.io/spring-cloud/spring-cloud.html#_creating_a_key_store_for_testing)
        *   [Using Multiple Keys and Key Rotation](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_multiple_keys_and_key_rotation)
    *   [Serving Plain Text](http://projects.spring.io/spring-cloud/spring-cloud.html#_serving_plain_text)
    *   [Embedding the Config Server](http://projects.spring.io/spring-cloud/spring-cloud.html#_embedding_the_config_server)
    *   [Push Notifications and Spring Cloud Bus](http://projects.spring.io/spring-cloud/spring-cloud.html#_push_notifications_and_spring_cloud_bus)
    *   [Spring Cloud Config Client](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_config_client)
        *   [Config First Bootstrap](http://projects.spring.io/spring-cloud/spring-cloud.html#config-first-bootstrap)
        *   [Eureka First Bootstrap](http://projects.spring.io/spring-cloud/spring-cloud.html#eureka-first-bootstrap)
        *   [Config Client Fail Fast](http://projects.spring.io/spring-cloud/spring-cloud.html#config-client-fail-fast)
        *   [Config Client Retry](http://projects.spring.io/spring-cloud/spring-cloud.html#config-client-retry)
        *   [Locating Remote Configuration Resources](http://projects.spring.io/spring-cloud/spring-cloud.html#_locating_remote_configuration_resources)
        *   [Security](http://projects.spring.io/spring-cloud/spring-cloud.html#_security_2)
*   [Spring Cloud Netflix](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_netflix)
    *   [Service Discovery: Eureka Clients](http://projects.spring.io/spring-cloud/spring-cloud.html#_service_discovery_eureka_clients)
        *   [Registering with Eureka](http://projects.spring.io/spring-cloud/spring-cloud.html#_registering_with_eureka)
        *   [Status Page and Health Indicator](http://projects.spring.io/spring-cloud/spring-cloud.html#_status_page_and_health_indicator)
        *   [Registering a Secure Application](http://projects.spring.io/spring-cloud/spring-cloud.html#_registering_a_secure_application)
        *   [Eureka’s Health Checks](http://projects.spring.io/spring-cloud/spring-cloud.html#_eureka_s_health_checks)
        *   [Eureka Metadata for Instances and Clients](http://projects.spring.io/spring-cloud/spring-cloud.html#_eureka_metadata_for_instances_and_clients)
        *   [Using the EurekaClient](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_the_eurekaclient)
        *   [Alternatives to the native Netflix EurekaClient](http://projects.spring.io/spring-cloud/spring-cloud.html#_alternatives_to_the_native_netflix_eurekaclient)
        *   [Why is it so Slow to Register a Service?](http://projects.spring.io/spring-cloud/spring-cloud.html#_why_is_it_so_slow_to_register_a_service)
    *   [Service Discovery: Eureka Server](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-eureka-server)
        *   [High Availability, Zones and Regions](http://projects.spring.io/spring-cloud/spring-cloud.html#_high_availability_zones_and_regions)
        *   [Standalone Mode](http://projects.spring.io/spring-cloud/spring-cloud.html#_standalone_mode)
        *   [Peer Awareness](http://projects.spring.io/spring-cloud/spring-cloud.html#_peer_awareness)
        *   [Prefer IP Address](http://projects.spring.io/spring-cloud/spring-cloud.html#_prefer_ip_address)
    *   [Circuit Breaker: Hystrix Clients](http://projects.spring.io/spring-cloud/spring-cloud.html#_circuit_breaker_hystrix_clients)
        *   [Propagating the Security Context or using Spring Scopes](http://projects.spring.io/spring-cloud/spring-cloud.html#_propagating_the_security_context_or_using_spring_scopes)
        *   [Health Indicator](http://projects.spring.io/spring-cloud/spring-cloud.html#_health_indicator_2)
        *   [Hystrix Metrics Stream](http://projects.spring.io/spring-cloud/spring-cloud.html#_hystrix_metrics_stream)
    *   [Circuit Breaker: Hystrix Dashboard](http://projects.spring.io/spring-cloud/spring-cloud.html#_circuit_breaker_hystrix_dashboard)
        *   [Turbine](http://projects.spring.io/spring-cloud/spring-cloud.html#_turbine)
        *   [Turbine AMQP](http://projects.spring.io/spring-cloud/spring-cloud.html#_turbine_amqp)
    *   [Customizing the AMQP ConnectionFactory](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_amqp_connectionfactory)
    *   [Client Side Load Balancer: Ribbon](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon)
        *   [Customizing the Ribbon Client](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_ribbon_client)
        *   [Using Ribbon with Eureka](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_ribbon_with_eureka)
        *   [Example: How to Use Ribbon Without Eureka](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon-without-eureka)
        *   [Example: Disable Eureka use in Ribbon](http://projects.spring.io/spring-cloud/spring-cloud.html#_example_disable_eureka_use_in_ribbon)
        *   [Using the Ribbon API Directly](http://projects.spring.io/spring-cloud/spring-cloud.html#_using_the_ribbon_api_directly)
    *   [Declarative REST Client: Feign](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign)
        *   [Overriding Feign Defaults](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-overriding-defaults)
        *   [Feign Hystrix Support](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-hystrix)
        *   [Feign Hystrix Fallbacks](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-hystrix-fallback)
        *   [Feign Inheritance Support](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign-inheritance)
        *   [Feign request/response compression](http://projects.spring.io/spring-cloud/spring-cloud.html#_feign_request_response_compression)
        *   [Feign logging](http://projects.spring.io/spring-cloud/spring-cloud.html#_feign_logging)
    *   [External Configuration: Archaius](http://projects.spring.io/spring-cloud/spring-cloud.html#_external_configuration_archaius)
    *   [Router and Filter: Zuul](http://projects.spring.io/spring-cloud/spring-cloud.html#_router_and_filter_zuul)
        *   [Embedded Zuul Reverse Proxy](http://projects.spring.io/spring-cloud/spring-cloud.html#netflix-zuul-reverse-proxy)
        *   [Strangulation Patterns and Local Forwards](http://projects.spring.io/spring-cloud/spring-cloud.html#_strangulation_patterns_and_local_forwards)
        *   [Uploading Files through Zuul](http://projects.spring.io/spring-cloud/spring-cloud.html#_uploading_files_through_zuul)
        *   [Plain Embedded Zuul](http://projects.spring.io/spring-cloud/spring-cloud.html#_plain_embedded_zuul)
        *   [Disable Zuul Filters](http://projects.spring.io/spring-cloud/spring-cloud.html#_disable_zuul_filters)
        *   [Polyglot support with Sidecar](http://projects.spring.io/spring-cloud/spring-cloud.html#_polyglot_support_with_sidecar)
    *   [Metrics: Spectator, Servo, and Atlas](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_spectator_servo_and_atlas)
        *   [Dimensional vs. Hierarchical Metrics](http://projects.spring.io/spring-cloud/spring-cloud.html#_dimensional_vs_hierarchical_metrics)
        *   [Default Metrics Collection](http://projects.spring.io/spring-cloud/spring-cloud.html#_default_metrics_collection)
        *   [Metrics Collection: Spectator](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_collection_spectator)
        *   [Metrics Collection: Servo](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_collection_servo)
        *   [Metrics Backend: Atlas](http://projects.spring.io/spring-cloud/spring-cloud.html#_metrics_backend_atlas)
*   [Spring Cloud Bus](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_bus)
    *   [Quick Start](http://projects.spring.io/spring-cloud/spring-cloud.html#_quick_start_2)
    *   [Addressing an Instance](http://projects.spring.io/spring-cloud/spring-cloud.html#_addressing_an_instance)
    *   [Addressing all instances of a service](http://projects.spring.io/spring-cloud/spring-cloud.html#_addressing_all_instances_of_a_service)
    *   [Application Context ID must be unique](http://projects.spring.io/spring-cloud/spring-cloud.html#_application_context_id_must_be_unique)
    *   [Customizing the Message Broker](http://projects.spring.io/spring-cloud/spring-cloud.html#_customizing_the_message_broker)
    *   [Tracing Bus Events](http://projects.spring.io/spring-cloud/spring-cloud.html#_tracing_bus_events)
*   [Spring Boot Cloud CLI](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_boot_cloud_cli)
    *   [Installation](http://projects.spring.io/spring-cloud/spring-cloud.html#_installation)
    *   [Writing Groovy Scripts and Running Applications](http://projects.spring.io/spring-cloud/spring-cloud.html#_writing_groovy_scripts_and_running_applications)
    *   [Encryption and Decryption](http://projects.spring.io/spring-cloud/spring-cloud.html#_encryption_and_decryption_3)
*   [Spring Cloud Security](http://projects.spring.io/spring-cloud/spring-cloud.html#_spring_cloud_security)
    *   [Quickstart](http://projects.spring.io/spring-cloud/spring-cloud.html#_quickstart)
        *   [OAuth2 Single Sign On](http://projects.spring.io/spring-cloud/spring-cloud.html#_oauth2_single_sign_on)
        *   [OAuth2 Protected Resource](http://projects.spring.io/spring-cloud/spring-cloud.html#_oauth2_protected_resource)
    *   [More Detail](http://projects.spring.io/spring-cloud/spring-cloud.html#_more_detail)
        *   [Single Sign On](http://projects.spring.io/spring-cloud/spring-cloud.html#_single_sign_on)
        *   [Token Relay](http://projects.spring.io/spring-cloud/spring-cloud.html#_token_relay)
    *   [Configuring Authentication Downstream of a Zuul Proxy](http://projects.spring.io/spring-cloud/spring-cloud.html#_configuring_authentication_downstream_of_a_zuul_proxy)

</div>

</div>

<div id="content">

<div id="preamble">

<div class="sectionbody">

<div class="paragraph">

Spring Cloud provides tools for developers to quickly build some of the common patterns in distributed systems (e.g. configuration management, service discovery, circuit breakers, intelligent routing, micro-proxy, control bus, one-time tokens, global locks, leadership election, distributed sessions, cluster state). Coordination of distributed systems leads to boiler plate patterns, and using Spring Cloud developers can quickly stand up services and applications that implement those patterns. They will work well in any distributed environment, including the developer’s own laptop, bare metal data centres, and managed platforms such as Cloud Foundry.

</div>

</div>

</div>

<div class="sect1">

## Features

<div class="sectionbody">

<div class="paragraph">

Spring Cloud focuses on providing good out of box experience for typical use cases and extensibility mechanism to cover others.

</div>

<div class="ulist">

*   Distributed/versioned configuration

*   Service registration and discovery

*   Routing

*   Service-to-service calls

*   Load balancing

*   Circuit Breakers

*   Global locks

*   Leadership election and cluster state

*   Distributed messaging

</div>

</div>

</div>

# Cloud Native Applications

<div class="openblock partintro">

<div class="content">

<div class="paragraph">

[Cloud Native](https://pivotal.io/platform-as-a-service/migrating-to-cloud-native-application-architectures-ebook) is a style of application development that encourages easy adoption of best practices in the areas of continuous delivery and value-driven development. A related discipline is that of building [12-factor Apps](http://12factor.net/) in which development practices are aligned with delivery and operations goals, for instance by using declarative programming and management and monitoring. Spring Cloud facilitates these styles of development in a number of specific ways and the starting point is a set of features that all components in a distributed system either need or need easy access to when required.

</div>

<div class="paragraph">

Many of those features are covered by [Spring Boot](http://projects.spring.io/spring-boot), which we build on in Spring Cloud. Some more are delivered by Spring Cloud as two libraries: Spring Cloud Context and Spring Cloud Commons. Spring Cloud Context provides utilities and special services for the `ApplicationContext` of a Spring Cloud application (bootstrap context, encryption, refresh scope and environment endpoints). Spring Cloud Commons is a set of abstractions and common classes used in different Spring Cloud implementations (eg. Spring Cloud Netflix vs. Spring Cloud Consul).

</div>

<div class="paragraph">

If you are getting an exception due to "Illegal key size" and you are using Sun’s JDK, you need to install the Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files. See the following links for more information:

</div>

<div class="ulist">

*   [Java 6 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-6-download-429243.html)

*   [Java 7 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html)

*   [Java 8 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html)

</div>

<div class="paragraph">

Extract files into JDK/jre/lib/security folder (whichever version of JRE/JDK x64/x86 you are using).

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">Spring Cloud is released under the non-restrictive Apache 2.0 license. If you would like to contribute to this section of the documentation or if you find an error, please find the source code and issue trackers in the project at {githubmaster}/docs/src/main/asciidoc[github].</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

<div class="sect1">

## Spring Cloud Context: Application Context Services

<div class="sectionbody">

<div class="paragraph">

Spring Boot has an opinionated view of how to build an application with Spring: for instance it has conventional locations for common configuration file, and endpoints for common management and monitoring tasks. Spring Cloud builds on top of that and adds a few features that probably all components in a system would use or occasionally need.

</div>

<div class="sect2">

### The Bootstrap Application Context

<div class="paragraph">

A Spring Cloud application operates by creating a "bootstrap" context, which is a parent context for the main application. Out of the box it is responsible for loading configuration properties from the external sources, and also decrypting properties in the local external configuration files. The two contexts share an `Environment` which is the source of external properties for any Spring application. Bootstrap properties are added with high precedence, so they cannot be overridden by local configuration.

</div>

<div class="paragraph">

The bootstrap context uses a different convention for locating external configuration than the main application context, so instead of `application.yml` (or `.properties`) you use `bootstrap.yml`, keeping the external configuration for bootstrap and main context nicely separate. Example:

</div>

<div class="listingblock">

<div class="title">bootstrap.yml</div>

<div class="content">

<pre>spring:
  application:
    name: foo
  cloud:
    config:
      uri: ${SPRING_CONFIG_URI:http://localhost:8888}</pre>

</div>

</div>

<div class="paragraph">

It is a good idea to set the `spring.application.name` (in `bootstrap.yml` or `application.yml`) if your application needs any application-specific configuration from the server.

</div>

<div class="paragraph">

You can disable the bootstrap process completely by setting `spring.cloud.bootstrap.enabled=false` (e.g. in System properties).

</div>

</div>

<div class="sect2">

### Application Context Hierarchies

<div class="paragraph">

If you build an application context from `SpringApplication` or `SpringApplicationBuilder`, then the Bootstrap context is added as a parent to that context. It is a feature of Spring that child contexts inherit property sources and profiles from their parent, so the "main" application context will contain additional property sources, compared to building the same context without Spring Cloud Config. The additional property sources are:

</div>

<div class="ulist">

*   "bootstrap": an optional `CompositePropertySource` appears with high priority if any `PropertySourceLocators` are found in the Bootstrap context, and they have non-empty properties. An example would be properties from the Spring Cloud Config Server. See [below](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-property-sources) for instructions on how to customize the contents of this property source.

*   "applicationConfig: [classpath:bootstrap.yml]" (and friends if Spring profiles are active). If you have a `bootstrap.yml` (or properties) then those properties are used to configure the Bootstrap context, and then they get added to the child context when its parent is set. They have lower precedence than the `application.yml` (or properties) and any other property sources that are added to the child as a normal part of the process of creating a Spring Boot application. See [below](http://projects.spring.io/spring-cloud/spring-cloud.html#customizing-bootstrap-properties) for instructions on how to customize the contents of these property sources.

</div>

<div class="paragraph">

Because of the ordering rules of property sources the "bootstrap" entries take precedence, but note that these do not contain any data from `bootstrap.yml`, which has very low precedence, but can be used to set defaults.

</div>

<div class="paragraph">

You can extend the context hierarchy by simply setting the parent context of any `ApplicationContext` you create, e.g. using its own interface, or with the `SpringApplicationBuilder` convenience methods (`parent()`, `child()` and `sibling()`). The bootstrap context will be the parent of the most senior ancestor that you create yourself. Every context in the hierarchy will have its own "bootstrap" property source (possibly empty) to avoid promoting values inadvertently from parents down to their descendants. Every context in the hierarchy can also (in principle) have a different `spring.application.name` and hence a different remote property source if there is a Config Server. Normal Spring application context behaviour rules apply to property resolution: properties from a child context override those in the parent, by name and also by property source name (if the child has a property source with the same name as the parent, the one from the parent is not included in the child).

</div>

<div class="paragraph">

Note that the `SpringApplicationBuilder` allows you to share an `Environment` amongst the whole hierarchy, but that is not the default. Thus, sibling contexts in particular do not need to have the same profiles or property sources, even though they will share common things with their parent.

</div>

</div>

<div class="sect2">

### Changing the Location of Bootstrap Properties

<div class="paragraph">

The `bootstrap.yml` (or `.properties`) location can be specified using `spring.cloud.bootstrap.name` (default "bootstrap") or `spring.cloud.bootstrap.location` (default empty), e.g. in System properties. Those properties behave like the `spring.config.*` variants with the same name, in fact they are used to set up the bootstrap `ApplicationContext` by setting those properties in its `Environment`. If there is an active profile (from `spring.profiles.active` or through the `Environment` API in the context you are building) then properties in that profile will be loaded as well, just like in a regular Spring Boot app, e.g. from `bootstrap-development.properties` for a "development" profile.

</div>

</div>

<div class="sect2">

### Customizing the Bootstrap Configuration

<div class="paragraph">

The bootstrap context can be trained to do anything you like by adding entries to `/META-INF/spring.factories` under the key `org.springframework.cloud.bootstrap.BootstrapConfiguration`. This is a comma-separated list of Spring `@Configuration` classes which will be used to create the context. Any beans that you want to be available to the main application context for autowiring can be created here, and also there is a special contract for `@Beans` of type `ApplicationContextInitializer`. Classes can be marked with an `@Order` if you want to control the startup sequence (the default order is "last").

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">Be careful when adding custom `BootstrapConfiguration` that the classes you add are not `@ComponentScanned` by mistake into your "main" application context, where they might not be needed. Use a separate package name for boot configuration classes that is not already covered by your `@ComponentScan` or `@SpringBootApplication` annotated configuration classes.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

The bootstrap process ends by injecting initializers into the main `SpringApplication` instance (i.e. the normal Spring Boot startup sequence, whether it is running as a standalone app or deployed in an application server). First a bootstrap context is created from the classes found in `spring.factories` and then all `@Beans` of type `ApplicationContextInitializer` are added to the main `SpringApplication` before it is started.

</div>

</div>

<div class="sect2">

### Customizing the Bootstrap Property Sources

<div class="paragraph">

The default property source for external configuration added by the bootstrap process is the Config Server, but you can add additional sources by adding beans of type `PropertySourceLocator` to the bootstrap context (via `spring.factories`). You could use this to insert additional properties from a different server, or from a database, for instance.

</div>

<div class="paragraph">

As an example, consider the following trivial custom locator:

</div>

<div class="listingblock">

<div class="content">

    @Configuration
    public class CustomPropertySourceLocator implements PropertySourceLocator {

        @Override
        public PropertySource<?> locate(Environment environment) {
            return new MapPropertySource("customProperty",
                    Collections.<String, Object>singletonMap("property.from.sample.custom.source", "worked as intended"));
        }

    }

</div>

</div>

<div class="paragraph">

The `Environment` that is passed in is the one for the `ApplicationContext` about to be created, i.e. the one that we are supplying additional property sources for. It will already have its normal Spring Boot-provided property sources, so you can use those to locate a property source specific to this `Environment` (e.g. by keying it on the `spring.application.name`, as is done in the default Config Server property source locator).

</div>

<div class="paragraph">

If you create a jar with this class in it and then add a `META-INF/spring.factories` containing:

</div>

<div class="listingblock">

<div class="content">

<pre>org.springframework.cloud.bootstrap.BootstrapConfiguration=sample.custom.CustomPropertySourceLocator</pre>

</div>

</div>

<div class="paragraph">

then the "customProperty" `PropertySource` will show up in any application that includes that jar on its classpath.

</div>

</div>

<div class="sect2">

### Environment Changes

<div class="paragraph">

The application will listen for an `EnvironmentChangedEvent` and react to the change in a couple of standard ways (additional `ApplicationListeners` can be added as `@Beans` by the user in the normal way). When an `EnvironmentChangedEvent` is observed it will have a list of key values that have changed, and the application will use those to:

</div>

<div class="ulist">

*   Re-bind any `@ConfigurationProperties` beans in the context

*   Set the logger levels for any properties in `logging.level.*`

</div>

<div class="paragraph">

Note that the Config Client does not by default poll for changes in the `Environment`, and generally we would not recommend that approach for detecting changes (although you could set it up with a `@Scheduled` annotation). If you have a scaled-out client application then it is better to broadcast the `EnvironmentChangedEvent` to all the instances instead of having them polling for changes (e.g. using the [Spring Cloud Bus](https://github.com/spring-cloud/spring-cloud-bus)).

</div>

<div class="paragraph">

The `EnvironmentChangedEvent` covers a large class of refresh use cases, as long as you can actually make a change to the `Environment` and publish the event (those APIs are public and part of core Spring). You can verify the changes are bound to `@ConfigurationProperties` beans by visiting the `/configprops` endpoint (normal Spring Boot Actuator feature). For instance a `DataSource` can have its `maxPoolSize` changed at runtime (the default `DataSource` created by Spring Boot is an `@ConfigurationProperties` bean) and grow capacity dynamically. Re-binding `@ConfigurationProperties` does not cover another large class of use cases, where you need more control over the refresh, and where you need a change to be atomic over the whole `ApplicationContext`. To address those concerns we have `@RefreshScope`.

</div>

</div>

<div class="sect2">

### Refresh Scope

<div class="paragraph">

A Spring `@Bean` that is marked as `@RefreshScope` will get special treatment when there is a configuration change. This addresses the problem of stateful beans that only get their configuration injected when they are initialized. For instance if a `DataSource` has open connections when the database URL is changed via the `Environment`, we probably want the holders of those connections to be able to complete what they are doing. Then the next time someone borrows a connection from the pool he gets one with the new URL.

</div>

<div class="paragraph">

Refresh scope beans are lazy proxies that initialize when they are used (i.e. when a method is called), and the scope acts as a cache of initialized values. To force a bean to re-initialize on the next method call you just need to invalidate its cache entry.

</div>

<div class="paragraph">

The `RefreshScope` is a bean in the context and it has a public method `refreshAll()` to refresh all beans in the scope by clearing the target cache. There is also a `refresh(String)` method to refresh an individual bean by name. This functionality is exposed in the `/refresh` endpoint (over HTTP or JMX).

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">`@RefreshScope` works (technically) on an `@Configuration` class, but it might lead to surprising behaviour: e.g. it does **not** mean that all the `@Beans` defined in that class are themselves `@RefreshScope`. Specifically, anything that depends on those beans cannot rely on them being updated when a refresh is initiated, unless it is itself in `@RefreshScope` (in which it will be rebuilt on a refresh and its dependencies re-injected, at which point they will be re-initialized from the refreshed `@Configuration`).</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Encryption and Decryption

<div class="paragraph">

The Config Client has an `Environment` pre-processor for decrypting property values locally. It follows the same rules as the Config Server, and has the same external configuration via `encrypt.*`. Thus you can use encrypted values in the form `{cipher}*` and as long as there is a valid key then they will be decrypted before the main application context gets the `Environment`. To use the encryption features in a client you need to include Spring Security RSA in your classpath (Maven co-ordinates "org.springframework.security:spring-security-rsa") and you also need the full strength JCE extensions in your JVM.

</div>

<div class="paragraph">

If you are getting an exception due to "Illegal key size" and you are using Sun’s JDK, you need to install the Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files. See the following links for more information:

</div>

<div class="ulist">

*   [Java 6 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-6-download-429243.html)

*   [Java 7 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html)

*   [Java 8 JCE](http://www.oracle.com/technetwork/java/javase/downloads/jce8-download-2133166.html)

</div>

<div class="paragraph">

Extract files into JDK/jre/lib/security folder (whichever version of JRE/JDK x64/x86 you are using).

</div>

</div>

<div class="sect2">

### Endpoints

<div class="paragraph">

For a Spring Boot Actuator application there are some additional management endpoints:

</div>

<div class="ulist">

*   POST to `/env` to update the `Environment` and rebind `@ConfigurationProperties` and log levels

*   `/refresh` for re-loading the boot strap context and refreshing the `@RefreshScope` beans

*   `/restart` for closing the `ApplicationContext` and restarting it (disabled by default)

*   `/pause` and `/resume` for calling the `Lifecycle` methods (`stop()` and `start()` on the `ApplicationContext`)

</div>

</div>

</div>

</div>

<div class="sect1">

## Spring Cloud Commons: Common Abstractions

<div class="sectionbody">

<div class="paragraph">

Patterns such as service discovery, load balancing and circuit breakers lend themselves to a common abstraction layer that can be consumed by all Spring Cloud clients, independent of the implementation (e.g. discovery via Eureka or Consul).

</div>

<div class="sect2">

### Spring RestTemplate as a Load Balancer Client

<div class="paragraph">

You can use Ribbon indirectly via an autoconfigured `RestTemplate` when RestTemplate is on the classpath and a `LoadBalancerClient` bean is defined):

</div>

<div class="listingblock">

<div class="content">

    public class MyClass {
        @Autowired
        private RestTemplate restTemplate;

        public String doOtherStuff() {
            String results = restTemplate.getForObject("http://stores/stores", String.class);
            return results;
        }
    }

</div>

</div>

<div class="paragraph">

The URI needs to use a virtual host name (ie. service name, not a host name). The Ribbon client is used to create a full physical address. See [RibbonAutoConfiguration](https://github.com/spring-cloud/spring-cloud-netflix/blob/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/ribbon/RibbonAutoConfiguration.java) for details of how the `RestTemplate` is set up.

</div>

</div>

<div class="sect2">

### Multiple RestTemplate objects

<div class="paragraph">

If you want a `RestTemplate` that is not load balanced, create a `RestTemplate` bean and inject it as normal. To access the load balanced `RestTemplate use the provided `@LoadBalanced` `Qualifier`:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

</div>

<div class="sect2">

### Ignore Network Interfaces

<div class="paragraph">

Sometimes it is useful to ignore certain named network interfaces so they can be excluded from Service Discovery registration (eg. running in a Docker container). A list of regular expressions can be set that will cause the desired network interfaces to be ignored. The following configuration will ignore the "docker0" interface and all interfaces that start with "veth".

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>spring:
  cloud:
    inetutils:
      ignoredInterfaces:
        - docker0
        - veth.*</pre>

</div>

</div>

</div>

</div>

</div>

# Spring Cloud Config

<div class="openblock partintro">

<div class="content">Spring Cloud Config provides server and client-side support for externalized configuration in a distributed system. With the Config Server you have a central place to manage external properties for applications across all environments. The concepts on both client and server map identically to the Spring `Environment` and `PropertySource` abstractions, so they fit very well with Spring applications, but can be used with any application running in any language. As an application moves through the deployment pipeline from dev to test and into production you can manage the configuration between those environments and be certain that applications have everything they need to run when they migrate. The default implementation of the server storage backend uses git so it easily supports labelled versions of configuration environments, as well as being accessible to a wide range of tooling for managing the content. It is easy to add alternative implementations and plug them in with Spring configuration.</div>

</div>

<div class="sect1">

## Quick Start

<div class="sectionbody">

<div class="paragraph">

Start the server:

</div>

<div class="listingblock">

<div class="content">

<pre>$ cd spring-cloud-config-server
$ mvn spring-boot:run</pre>

</div>

</div>

<div class="paragraph">

The server is a Spring Boot application so you can run it from your IDE instead if you prefer (the main class is `ConfigServerApplication`). Then try it out a client:

</div>

<div class="listingblock">

<div class="content">

<pre>$ curl localhost:8888/foo/development
{"name":"development","label":"master","propertySources":[
  {"name":"https://github.com/scratches/config-repo/foo-development.properties","source":{"bar":"spam"}},
  {"name":"https://github.com/scratches/config-repo/foo.properties","source":{"foo":"bar"}}
]}</pre>

</div>

</div>

<div class="paragraph">

The default strategy for locating property sources is to clone a git repository (at `spring.cloud.config.server.git.uri`) and use it to initialize a mini `SpringApplication`. The mini-application’s `Environment` is used to enumerate property sources and publish them via a JSON endpoint.

</div>

<div class="paragraph">

The HTTP service has resources in the form:

</div>

<div class="listingblock">

<div class="content">

<pre>/{application}/{profile}[/{label}]
/{application}-{profile}.yml
/{label}/{application}-{profile}.yml
/{application}-{profile}.properties
/{label}/{application}-{profile}.properties</pre>

</div>

</div>

<div class="paragraph">

where the "application" is injected as the `spring.config.name` in the `SpringApplication` (i.e. what is normally "application" in a regular Spring Boot app), "profile" is an active profile (or comma-separated list of properties), and "label" is an optional git label (defaults to "master".)

</div>

<div class="paragraph">

The YAML and properties forms are coalesced into a single map, even if the origin of the values (reflected in the "propertySources" of the "standard" form) has multiple sources.

</div>

<div class="paragraph">

Spring Cloud Config Server pulls configuration for remote clients from a git repository (which must be provided):

</div>

<div class="listingblock">

<div class="content">

    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo

</div>

</div>

<div class="sect2">

### Client Side Usage

<div class="paragraph">

To use these features in an application, just build it as a Spring Boot application that depends on spring-cloud-config-client (e.g. see the test cases for the config-client, or the sample app). The most convenient way to add the dependency is via a Spring Boot starter `org.springframework.cloud:spring-cloud-starter-config`. There is also a parent pom and BOM (`spring-cloud-starter-parent`) for Maven users and a Spring IO version management properties file for Gradle and Spring CLI users. Example Maven configuration:

</div>

<div class="listingblock">

<div class="title">pom.xml</div>

<div class="content">

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

</div>

</div>

<div class="paragraph">

Then you can create a standard Spring Boot application, like this simple HTTP server:

</div>

<div class="listingblock">

<div class="content">

<pre>@SpringBootApplication
@RestController
public class Application {

    @RequestMapping("/")
    public String home() {
        return "Hello World!";
    }

    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }

}</pre>

</div>

</div>

<div class="paragraph">

When it runs it will pick up the external configuration from the default local config server on port 8888 if it is running. To modify the startup behaviour you can change the location of the config server using `bootstrap.properties` (like `application.properties` but for the bootstrap phase of an application context), e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>spring.cloud.config.uri: http://myconfigserver.com</pre>

</div>

</div>

<div class="paragraph">

The bootstrap properties will show up in the `/env` endpoint as a high-priority property source, e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>$ curl localhost:8080/env
{
  "profiles":[],
  "configService:https://github.com/spring-cloud-samples/config-repo/bar.properties":{"foo":"bar"},
  "servletContextInitParams":{},
  "systemProperties":{...},
  ...
}</pre>

</div>

</div>

<div class="paragraph">

(a property source called "configService:<URL of remote repository>/<file name>" contains the property "foo" with value "bar" and is highest priority).

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">the URL in the property source name is the git repository not the config server URL.</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

</div>

<div class="sect1">

## Spring Cloud Config Server

<div class="sectionbody">

<div class="paragraph">

The Server provides an HTTP, resource-based API for external configuration (name-value pairs, or equivalent YAML content). The server is easily embeddable in a Spring Boot application using the `@EnableConfigServer` annotation. So this app is a config server:

</div>

<div class="listingblock">

<div class="title">ConfigServer.java</div>

<div class="content">

    @SpringBootApplication
    @EnableConfigServer
    public class ConfigServer {
      public static void main(String[] args) {
        SpringApplication.run(ConfigServer.class, args);
      }
    }

</div>

</div>

<div class="paragraph">

Like all Spring Boot apps it runs on port 8080 by default, but you can switch it to the conventional port 8888 in various ways. The easiest, which also sets a default configuration repository, is by launching it with `spring.config.name=configserver` (there is a `configserver.yml` in the Config Server jar). Another is to use your own `application.properties`, e.g.

</div>

<div class="listingblock">

<div class="title">application.properties</div>

<div class="content">

    server.port: 8888
    spring.cloud.config.server.git.uri: file://${user.home}/config-repo

</div>

</div>

<div class="paragraph">

where `${user.home}/config-repo` is a git repository containing YAML and properties files.

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">in Windows you need an extra "/" in the file URL if it is absolute with a drive prefix, e.g. `[file:///${user.home}/config-repo](file:///$%7Buser.home%7D/config-repo)`.</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">

<div class="paragraph">

Here’s a recipe for creating the git repository in the example above:

</div>

<div class="listingblock">

<div class="content">

<pre>$ cd $HOME
$ mkdir config-repo
$ cd config-repo
$ git init .
$ echo info.foo: bar > application.properties
$ git add -A .
$ git commit -m "Add application.properties"</pre>

</div>

</div>

</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">using the local filesystem for your git repository is intended for testing only. Use a server to host your configuration repositories in production.</td>

</tr>

</tbody>

</table>

</div>

<div class="sect2">

### Environment Repository

<div class="paragraph">

Where do you want to store the configuration data for the Config Server? The strategy that governs this behaviour is the `EnvironmentRepository`, serving `Environment` objects. This `Environment` is a shallow copy of the domain from the Spring `Environment` (including `propertySources` as the main feature). The `Environment` resources are parametrized by three variables:

</div>

<div class="ulist">

*   `{application}` maps to "spring.application.name" on the client side;

*   `{profile}` maps to "spring.active.profiles" on the client (comma separated list); and

*   `{label}` which is a server side feature labelling a "versioned" set of config files.

</div>

<div class="paragraph">

Repository implementations generally behave just like a Spring Boot application loading configuration files from a "spring.config.name" equal to the `{application}` parameter, and "spring.profiles.active" equal to the `{profiles}` parameter. Precedence rules for profiles are also the same as in a regular Boot application: active profiles take precedence over defaults, and if there are multiple profiles the last one wins (like adding entries to a `Map`).

</div>

<div class="paragraph">

Example: a client application has this bootstrap configuration:

</div>

<div class="listingblock">

<div class="title">bootstrap.yml</div>

<div class="content">

    spring:
      application:
        name: foo
      profiles:
        active: dev,mysql

</div>

</div>

<div class="paragraph">

(as usual with a Spring Boot application, these properties could also be set as environment variables or command line arguments).

</div>

<div class="paragraph">

If the repository is file-based, the server will create an `Environment` from `application.yml` (shared between all clients), and `foo.yml` (with `foo.yml` taking precedence). If the YAML files have documents inside them that point to Spring profiles, those are applied with higher precendence (in order of the profiles listed), and if there are profile-specific YAML (or properties) files these are also applied with higher precedence than the defaults. Higher precendence translates to a `PropertySource` listed earlier in the `Environment`. (These are the same rules as apply in a standalone Spring Boot application.)

</div>

<div class="sect3">

#### Git Backend

<div class="paragraph">

The default implementation of `EnvironmentRepository` uses a Git backend, which is very convenient for managing upgrades and physical environments, and also for auditing changes. To change the location of the repository you can set the "spring.cloud.config.server.git.uri" configuration property in the Config Server (e.g. in `application.yml`). If you set it with a `file:` prefix it should work from a local repository so you can get started quickly and easily without a server, but in that case the server operates directly on the local repository without cloning it (it doesn’t matter if it’s not bare because the Config Server never makes changes to the "remote" repository). To scale the Config Server up and make it highly available, you would need to have all instances of the server pointing to the same repository, so only a shared file system would work. Even in that case it is better to use the `ssh:` protocol for a shared filesystem repository, so that the server can clone it and use a local working copy as a cache.

</div>

<div class="paragraph">

This repository implementation maps the `{label}` parameter of the HTTP resource to a git label (commit id, branch name or tag). If the git branch or tag name contains a slash ("/") then the label in the HTTP URL should be specified with the special string "(_)" instead (to avoid ambiguity with other URL paths). Be careful with the brackets in the URL if you are using a command line client like curl (e.g. escape them from the shell with quotes '').

</div>

<div class="sect4">

##### Placeholders in Git URI

<div class="paragraph">

Spring Cloud Config Server supports a git repository URL with placeholders for the `{application}` and `{profile}` (and `{label}` if you need it, but remember that the label is applied as a git label anyway). So you can easily support a "one repo per application" policy using (for example):

</div>

<div class="listingblock">

<div class="content">

    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/myorg/{application}

</div>

</div>

<div class="paragraph">

or a "one repo per profile" policy using a similar pattern but with `{profile}`.

</div>

</div>

<div class="sect4">

##### Pattern Matching and Multiple Repositories

<div class="paragraph">

There is also support for more complex requirements with pattern matching on the application and profile name. The pattern format is a comma-separated list of `{application}/{profile}` names with wildcards (where a pattern beginning with a wildcard may need to be quoted). Example:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="paragraph">

If `{application}/{profile}` does not match any of the patterns, it will use the default uri defined under "spring.cloud.config.server.git.uri". In the above example, for the "simple" repository, the pattern is `simple/*` (i.e. it only matches one application named "simple" in all profiles). The "local" repository matches all application names beginning with "local" in all profiles (the `/*` suffix is added automatically to any pattern that doesn’t have a profile matcher).

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">the "one-liner" short cut used in the "simple" example above can only be used if the only property to be set is the URI. If you need to set anything else (credentials, pattern, etc.) you need to use the full form.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

The `pattern` property in the repo is actually an array, so you can use a YAML array (or `[0]`, `[1]`, etc. suffixes in properties files) to bind to multiple patterns. You may need to do this if you are going to run apps with multiple profiles. Example:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">Spring Cloud will guess that a pattern containing a profile that doesn’t end in `*` implies that you actually want to match a list of profiles starting with this pattern (so `*/staging` is a shortcut for `["*/staging", "*/staging,*"]`). This is common where you need to run apps in the "development" profile locally but also the "cloud" profile remotely, for instance.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

Every repository can also optionally store config files in sub-directories, and patterns to search for those directories can be specified as `searchPaths`. For example at the top level:

</div>

<div class="listingblock">

<div class="content">

    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              searchPaths: foo,bar*

</div>

</div>

<div class="paragraph">

In this example the server searches for config files in the top level and in the "foo/" sub-directory and also any sub-directory whose name begins with "bar".

</div>

<div class="paragraph">

By default the server clones remote repositories when configuration is first requested. The server can be configured to clone the repositories at startup. For example at the top level:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="paragraph">

In this example the server clones team-a’s config-repo on startup before it accepts any requests. All other repositories will not be cloned until configuration from the repository is requested.

</div>

<div class="paragraph">

To use HTTP basic authentication on the remote repository add the "username" and "password" properties separately (not in the URL), e.g.

</div>

<div class="listingblock">

<div class="content">

    spring:
      cloud:
        config:
          server:
            git:
              uri: https://github.com/spring-cloud-samples/config-repo
              username: trolley
              password: strongpassword

</div>

</div>

<div class="paragraph">

If you don’t use HTTPS and user credentials, SSH should also work out of the box when you store keys in the default directories (`~/.ssh`) and the uri points to an SSH location, e.g. "[git@github.com](mailto:git@github.com):configuration/cloud-configuration". The repository is accessed using JGit, so any documentation you find on that should be applicable. HTTPS proxy settings can be set in `~/.git/config` or in the same way as for any other JVM process via system properties (`-Dhttps.proxyHost` and `-Dhttps.proxyPort`).

</div>

</div>

</div>

<div class="sect3">

#### File System Backend

<div class="paragraph">

There is also a "native" profile in the Config Server that doesn’t use Git, but just loads the config files from the local classpath or file system (any static URL you want to point to with "spring.cloud.config.server.native.searchLocations"). To use the native profile just launch the Config Server with "spring.profiles.active=native".

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">Remember to use the `file:` prefix for file resources (the default without a prefix is usually the classpath). Just as with any Spring Boot configuration you can embed `${}`-style environment placeholders, but remember that absolute paths in Windows require an extra "/", e.g. `[file:///${user.home}/config-repo](file:///$%7Buser.home%7D/config-repo)`</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">The default value of the `searchLocations` is identical to a local Spring Boot application (so `[classpath:/, classpath:/config, file:./, file:./config]`). This does not expose the `application.properties` from the server to all clients because any property sources present in the server are removed before being sent to the client.</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">A filesystem backend is great for getting started quickly and for testing. To use it in production you need to be sure that the file system is reliable, and shared across all instances of the Config Server.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

The search locations can contain placeholders for `{application}`, `{profile}` and `{label}`. In this way you can segregate the directories in the path, and choose a strategy that makes sense for you (e.g. sub-directory per application, or sub-directory per profile).

</div>

<div class="paragraph">

If you don’t use placeholders in the search locations, this repository also appends the `{label}` parameter of the HTTP resource to a suffix on the search path, so properties files are loaded from each search location **and** a subdirectory with the same name as the label (the labelled properties take precedence in the Spring Environment). Thus the default behaviour with no placeholders is the same as adding a search location ending with `/{label}/. For example `file:/tmp/config` is the same as `file:/tmp/config,file:/tmp/config/{label}`

</div>

</div>

<div class="sect3">

#### Sharing Configiration With All Applications

<div class="paragraph">

With file-based (i.e. git, svn and native) repositories, resources with file names in `application*` are shared between all client applications (so `application.properties`, `application.yml`, `application-*.properties` etc.). You can use resources with these file names to configure global defaults and have them overridden by application-specific files as necessary.

</div>

<div class="paragraph">

The #_property_overrides[property overrides] feature can also be used for setting global defaults, and with placeholders applications are allowed to override them locally.

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">With the "native" profile (local file system backend) it is recommended that you use an explicit search location that isn’t part of the server’s own configuration. Otherwise the `application*` resources in the default search locations are removed because they are part of the server.</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect3">

#### Property Overrides

<div class="paragraph">

The Config Server has an "overrides" feature that allows the operator to provide configuration properties to all applications that cannot be accidentally changed by the application using the normal Spring Boot hooks. To declare overrides just add a map of name-value pairs to `spring.cloud.config.server.overrides`. For example

</div>

<div class="listingblock">

<div class="content">

    spring:
      cloud:
        config:
          server:
            overrides:
              foo: bar

</div>

</div>

<div class="paragraph">

will cause all applications that are config clients to read `foo=bar` independent of their own configuration. (Of course an application can use the data in the Config Server in any way it likes, so overrides are not enforceable, but they do provide useful default behaviour if they are Spring Cloud Config clients.)

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">Normal, Spring environment placeholders with "${}" can be escaped (and resolved on the client) by using backslash ("\") to escape the "$" or the "{", e.g. `\${app.foo:bar}` resolves to "bar" unless the app provides its own "app.foo". Note that in YAML you don’t need to escape the backslash itself, but in properties files you do, when you configure the overrides on the server.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

You can change the priority of all overrides in the client to be more like default values, allowing applications to supply their own values in environment variables or System properties, by setting the flag `

</div>

</div>

</div>

<div class="sect2">

### Health Indicator

<div class="paragraph">

Config Server comes with a Health Indicator that checks if the configured `EnvironmentRepository` is working. By default it asks the `EnvironmentRepository` for an application named `app`, the `default` profile and the default label provided by the `EnvironmentRepository` implementation.

</div>

<div class="paragraph">

You can configure the Health Indicator to check more applications along with custom profiles and custom labels, e.g.

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="paragraph">

You can disable the Health Indicator by setting `spring.cloud.config.server.health.enabled=false`.

</div>

</div>

<div class="sect2">

### Security

<div class="paragraph">

You are free to secure your Config Server in any way that makes sense to you (from physical network security to OAuth2 bearer tokens), and Spring Security and Spring Boot make it easy to do pretty much anything.

</div>

<div class="paragraph">

To use the default Spring Boot configured HTTP Basic security, just include Spring Security on the classpath (e.g. through `spring-boot-starter-security`). The default is a username of "user" and a randomly generated password, which isn’t going to be very useful in practice, so we recommend you configure the password (via `security.user.password`) and encrypt it (see below for instructions on how to do that).

</div>

</div>

<div class="sect2">

### Encryption and Decryption

<div class="admonitionblock important">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Important</div>

</td>

<td class="content">**Prerequisites:** to use the encryption and decryption features you need the full-strength JCE installed in your JVM (it’s not there by default). You can download the "Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files" from Oracle, and follow instructions for installation (essentially replace the 2 policy files in the JRE lib/security directory with the ones that you downloaded).</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

If the remote property sources contain encrypted content (values starting with `{cipher}`) they will be decrypted before sending to clients over HTTP. The main advantage of this set up is that the property values don’t have to be in plain text when they are "at rest" (e.g. in a git repository). If a value cannot be decrypted it is removed from the property source and an additional property is added with the same key, but prefixed with "invalid." and a value that means "not applicable" (usually "<n/a>"). This is largely to prevent cipher text being used as a password and accidentally leaking.

</div>

<div class="paragraph">

If you are setting up a remote config repository for config client applications it might contain an `application.yml` like this, for instance:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

    spring:
      datasource:
        username: dbuser
        password: '{cipher}FKSAJDFGYOS8F7GLHAKERGFHLSAJ'

</div>

</div>

<div class="paragraph">

Encrypted values in a .properties file must not be wrapped in quotes, otherwise the value will not be decrypted:

</div>

<div class="listingblock">

<div class="title">application.properties</div>

<div class="content">

<pre>spring.datasource.username: dbuser
spring.datasource.password: {cipher}FKSAJDFGYOS8F7GLHAKERGFHLSAJ</pre>

</div>

</div>

<div class="paragraph">

You can safely push this plain text to a shared git repository and the secret password is protected.

</div>

<div class="paragraph">

The server also exposes `/encrypt` and `/decrypt` endpoints (on the assumption that these will be secured and only accessed by authorized agents). If you are editing a remote config file you can use the Config Server to encrypt values by POSTing to the `/encrypt` endpoint, e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>$ curl localhost:8888/encrypt -d mysecret
682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda</pre>

</div>

</div>

<div class="paragraph">

The inverse operation is also available via `/decrypt` (provided the server is configured with a symmetric key or a full key pair):

</div>

<div class="listingblock">

<div class="content">

<pre>$ curl localhost:8888/decrypt -d 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
mysecret</pre>

</div>

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">If you are testing like this with curl, then use `--data-urlencode` (instead of `-d`) or set an explicit `Content-Type: text/plain` to make sure curl encodes the data correctly when there are special characters ('+' is particularly tricky).</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

Take the encrypted value and add the `{cipher}` prefix before you put it in the YAML or properties file, and before you commit and push it to a remote, potentially insecure store.

</div>

<div class="paragraph">

The `/encrypt` and `/decrypt` endpoints also both accept paths of the form `/*/{name}/{profiles}` which can be used to control cryptography per application (name) and profile when clients call into the main Environment resource.

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">to control the cryptography in this granular way you must also provide a `@Bean` of type `TextEncryptorLocator` that creates a different encryptor per name and profiles. The one that is provided by default does not do this (so all encryptions use the same key).</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

The `spring` command line client (with Spring Cloud CLI extensions installed) can also be used to encrypt and decrypt, e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>$ spring encrypt mysecret --key foo
682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
$ spring decrypt --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
mysecret</pre>

</div>

</div>

<div class="paragraph">

To use a key in a file (e.g. an RSA public key for encryption) prepend the key value with "@" and provide the file path, e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>$ spring encrypt mysecret --key @${HOME}/.ssh/id_rsa.pub
AQAjPgt3eFZQXwt8tsHAVv/QHiY5sI2dRcR+...</pre>

</div>

</div>

<div class="paragraph">

The key argument is mandatory (despite having a `--` prefix).

</div>

</div>

<div class="sect2">

### Key Management

<div class="paragraph">

The Config Server can use a symmetric (shared) key or an asymmetric one (RSA key pair). The asymmetric choice is superior in terms of security, but it is often more convenient to use a symmetric key since it is just a single property value to configure.

</div>

<div class="paragraph">

To configure a symmetric key you just need to set `encrypt.key` to a secret String (or use an enviroment variable `ENCRYPT_KEY` to keep it out of plain text configuration files).

</div>

<div class="paragraph">

To configure an asymmetric key you can either set the key as a PEM-encoded text value (in `encrypt.key`), or via a keystore (e.g. as created by the `keytool` utility that comes with the JDK). The keystore properties are `encrypt.keyStore.*` with `*` equal to

</div>

<div class="ulist">

*   `location` (a `Resource` location),

*   `password` (to unlock the keystore) and

*   `alias` (to identify which key in the store is to be used).

</div>

<div class="paragraph">

The encryption is done with the public key, and a private key is needed for decryption. Thus in principle you can configure only the public key in the server if you only want to do encryption (and are prepared to decrypt the values yourself locally with the private key). In practice you might not want to do that because it spreads the key management process around all the clients, instead of concentrating it in the server. On the other hand it’s a useful option if your config server really is relatively insecure and only a handful of clients need the encrypted properties.

</div>

</div>

<div class="sect2">

### Creating a Key Store for Testing

<div class="paragraph">

To create a keystore for testing you can do something like this:

</div>

<div class="listingblock">

<div class="content">

<pre>$ keytool -genkeypair -alias mytestkey -keyalg RSA \
  -dname "CN=Web Server,OU=Unit,O=Organization,L=City,S=State,C=US" \
  -keypass changeme -keystore server.jks -storepass letmein</pre>

</div>

</div>

<div class="paragraph">

Put the `server.jks` file in the classpath (for instance) and then in your `application.yml` for the Config Server:

</div>

<div class="listingblock">

<div class="content">

    encrypt:
      keyStore:
        location: classpath:/server.jks
        password: letmein
        alias: mytestkey
        secret: changeme

</div>

</div>

</div>

<div class="sect2">

### Using Multiple Keys and Key Rotation

<div class="paragraph">

In addition to the `{cipher}` prefix in encrypted property values, the Config Server looks for `{name:value}` prefixes (zero or many) before the start of the (Base64 encoded) cipher text. The keys are passed to a `TextEncryptorLocator` which can do whatever logic it needs to locate a `TextEncryptor` for the cipher. If you have configured a keystore (`encrypt.keystore.location`) the default locator will look for keys in the store with aliases as supplied by the "key" prefix, i.e. with a cipher text like this:

</div>

<div class="listingblock">

<div class="content">

    foo:
      bar: `{cipher}{key:testkey}...`

</div>

</div>

<div class="paragraph">

the locator will look for a key named "testkey". A secret can also be supplied via a `{secret:…​}` value in the prefix, but if it is not the default is to use the keystore password (which is what you get when you build a keytore and don’t specify a secret). If you **do** supply a secret it is recommended that you also encrypt the secrets using a custom `SecretLocator`.

</div>

<div class="paragraph">

Key rotation is hardly ever necessary on cryptographic grounds if the keys are only being used to encrypt a few bytes of configuration data (i.e. they are not being used elsewhere), but occasionally you might need to change the keys if there is a security breach for instance. In that case all the clients would need to change their source config files (e.g. in git) and use a new `{key:…​}` prefix in all the ciphers, checking beforehand of course that the key alias is available in the Config Server keystore.

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">the `{name:value}` prefixes can also be added to plaintext posted to the `/encrypt` endpoint, if you want to let the Config Server handle all encryption as well as decryption.</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

</div>

<div class="sect1">

## Serving Plain Text

<div class="sectionbody">

<div class="paragraph">

Instead of using the `Environment` abstraction (or one of the alternative representations of it in YAML or properties format) your applications might need generic plain text configuration files, tailored to their environment. The Config Server provides these through an additional endpoint at `/{name}/{profile}/{label}/{path}` where "name", "profile" and "label" have the same meaning as the regular environment endpoint, but "path" is a file name (e.g. `log.xml`). The source files for this endpoint are located in the same way as for the environment endpoints: the same search path is used as for properties or YAML files, but instead of aggregating all matching resources, only the first one to match is returned.

</div>

<div class="paragraph">

After a resource is located, placeholders in the normal format (`${…​}`) are resolved using the effective `Environment` for the application name, profile and label supplied. In this way the resource endpoint is tightly integrated with the environment endpoints. Example, if you have this layout for a GIT (or SVN) repository:

</div>

<div class="listingblock">

<div class="content">

<pre>application.yml
nginx.conf</pre>

</div>

</div>

<div class="paragraph">

where `nginx.conf` looks like this:

</div>

<div class="listingblock">

<div class="content">

<pre>server {
    listen              80;
    server_name         ${nginx.server.name};
}</pre>

</div>

</div>

<div class="paragraph">

and `application.yml` like this:

</div>

<div class="listingblock">

<div class="content">

    nginx:
      server:
        name: example.com
    ---
    spring:
      profiles: development
    nginx:
      server:
        name: develop.com

</div>

</div>

<div class="paragraph">

then the `/foo/default/master/nginx.conf` resource looks like this:

</div>

<div class="listingblock">

<div class="content">

<pre>server {
    listen              80;
    server_name         example.com;
}</pre>

</div>

</div>

<div class="paragraph">

and `/foo/development/master/nginx.conf` like this:

</div>

<div class="listingblock">

<div class="content">

<pre>server {
    listen              80;
    server_name         develop.com;
}</pre>

</div>

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">just like the source files for environment configuration, the "profile" is used to resolve the file name, so if you want a profile-specific file then `/*/development/*/logback.xml` will be resolved by a file called `logback-development.xml` (in preference to `logback.xml`).</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

<div class="sect1">

## Embedding the Config Server

<div class="sectionbody">

<div class="paragraph">

The Config Server runs best as a standalone application, but if you need to you can embed it in another application. Just use the `@EnableConfigServer` annotation. An optional property that can be useful in this case is `spring.cloud.config.server.bootstrap` which is a flag to indicate that the server should configure itself from its own remote repository. The flag is off by default because it can delay startup, but when embedded in another application it makes sense to initialize the same way as any other application.

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">It should be obvious, but remember that if you use the bootstrap flag the config server will need to have its name and repository URI configured in `bootstrap.yml`.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

To change the location of the server endpoints you can (optionally) set `spring.cloud.config.server.prefix`, e.g. "/config", to serve the resources under a prefix. The prefix should start but not end with a "/". It is applied to the `@RequestMappings` in the Config Server (i.e. underneath the Spring Boot prefixes `server.servletPath` and `server.contextPath`).

</div>

<div class="paragraph">

If you want to read the configuration for an application directly from the backend repository (instead of from the config server) that’s basically an embedded config server with no endpoints. You can switch off the endpoints entirely if you don’t use the `@EnableConfigServer` annotation (just set `spring.cloud.config.server.bootstrap=true`).

</div>

</div>

</div>

<div class="sect1">

## Push Notifications and Spring Cloud Bus

<div class="sectionbody">

<div class="paragraph">

Many source code repository providers (like Github, Gitlab or Bitbucket for instance) will notify you of changes in a repository through a webhook. You can configure the webhook via the provider’s user interface as a URL and a set of events in which you are interested. For instance [Github](https://developer.github.com/v3/activity/events/types/#pushevent) will POST to the webhook with a JSON body containing a list of commits, and a header "X-Github-Event" equal to "push". If you add a dependency on the `spring-cloud-config-monitor` library and activate the Spring Cloud Bus in your Config Server, then a "/monitor" endpoint is enabled.

</div>

<div class="paragraph">

When the webhook is activated the Config Server will send a `RefreshRemoteApplicationEvent` targeted at the applications it thinks might have changed. The change detection can be strategized, but by default it just looks for changes in files that match the application name (e.g. "foo.properties" is targeted at the "foo" application, and "application.properties" is targeted at all applications). The strategy if you want to override the behaviour is `PropertyPathNotificationExtractor` which accepts the request headers and body as parameters and returns a list of file paths that changed.

</div>

<div class="paragraph">

The default configuration works out of the box with Github, Gitlab or Bitbucket. In addition to the JSON notifications from Github, Gitlab or Bitbucket you can trigger a change notification by POSTing to "/monitor" with a form-encoded body parameters `path={name}`. This will broadcast to applications matching the "{name}" pattern (can contain wildcards).

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">the `RefreshRemoteApplicationEvent` will only be transmitted if the `spring-cloud-bus` is activated in the Config Server and in the client application.</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">the default configuration also detects filesystem changes in local git repositories (the webhook is not used in that case but as soon as you edit a config file a refresh will be broadcast).</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

<div class="sect1">

## Spring Cloud Config Client

<div class="sectionbody">

<div class="paragraph">

A Spring Boot application can take immediate advantage of the Spring Config Server (or other external property sources provided by the application developer), and it will also pick up some additional useful features related to `Environment` change events.

</div>

<div class="sect2">

### Config First Bootstrap

<div class="paragraph">

This is the default behaviour for any application which has the Spring Cloud Config Client on the classpath. When a config client starts up it binds to the Config Server (via the bootstrap configuration property `spring.cloud.config.uri`) and initializes Spring `Environment` with remote property sources.

</div>

<div class="paragraph">

The net result of this is that all client apps that want to consume the Config Server need a `bootstrap.yml` (or an environment variable) with the server address in `spring.cloud.config.uri` (defaults to "http://localhost:8888").

</div>

</div>

<div class="sect2">

### Eureka First Bootstrap

<div class="paragraph">

If you are using Spring Cloud Netflix and Eureka Service Discovery, then you can have the Config Server register with Eureka if you want to, but in the default "Config First" mode, clients won’t be able to take advantage of the registration.

</div>

<div class="paragraph">

If you prefer to use Eureka to locate the Config Server, you can do that by setting `spring.cloud.config.discovery.enabled=true` (default "false"). The net result of that is that client apps all need a `bootstrap.yml` (or an environment variable) with the Eureka server address, e.g. in `eureka.client.serviceUrl.defaultZone`. The price for using this option is an extra network round trip on start up to locate the service registration. The benefit is that the Config Server can change its co-ordinates, as long as Eureka is a fixed point. The default service id is "CONFIGSERVER" but you can change that on the client with `spring.cloud.config.discovery.serviceId` (and on the server in the usual way for a service, e.g. by setting `spring.application.name`).

</div>

<div class="paragraph">

The discovery client implementations all support some kind of metadata map (e.g. for Eureka we have `eureka.instance.metadataMap`). Some additional properties of the Config Server may need to be configured in its service registration metadata so that clients can connect correctly. If the Config Server is secured with HTTP Basic you can configure the credentials as "username" and "password". And if the Config Server has a context path you can set "configPath". Example, for a Config Server that is a Eureka client:

</div>

<div class="listingblock">

<div class="title">bootstrap.yml</div>

<div class="content">

    eureka:
      instance:
        ...
        metadataMap:
          username: osufhalskjrtl
          password: lviuhlszvaorhvlo5847
          configPath: /config

</div>

</div>

</div>

<div class="sect2">

### Config Client Fail Fast

<div class="paragraph">

In some cases, it may be desirable to fail startup of a service if it cannot connect to the Config Server. If this is the desired behavior, set the bootstrap configuration property `spring.cloud.config.failFast=true` and the client will halt with an Exception.

</div>

</div>

<div class="sect2">

### Config Client Retry

<div class="paragraph">

If you expect that the config server may occasionally be unavailable when your app starts, you can ask it to keep trying after a failure. First you need to set `spring.cloud.config.failFast=true`, and then you need to add `spring-retry` and `spring-boot-starter-aop` to your classpath. The default behaviour is to retry 6 times with an initial backoff interval of 1000ms and an exponential multiplier of 1.1 for subsequent backoffs. You can configure these properties (and others) using `spring.cloud.config.retry.*` configuration properties.

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">To take full control of the retry add a `@Bean` of type `RetryOperationsInterceptor` with id "configServerRetryInterceptor". Spring Retry has a `RetryInterceptorBuilder` that makes it easy to create one.</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Locating Remote Configuration Resources

<div class="paragraph">

The Config Service serves property sources from `/{name}/{profile}/{label}`, where the default bindings in the client app are

</div>

<div class="ulist">

*   "name" = `${spring.application.name}`

*   "profile" = `${spring.profiles.active}` (actually `Environment.getActiveProfiles()`)

*   "label" = "master"

</div>

<div class="paragraph">

All of them can be overridden by setting `spring.cloud.config.*` (where `*` is "name", "profile" or "label"). The "label" is useful for rolling back to previous versions of configuration; with the default Config Server implementation it can be a git label, branch name or commit id. Label can also be provided as a comma-separated list, in which case the items in the list are tried on-by-one until one succeeds. This can be useful when working on a feature branch, for instance, when you might want to align the config label with your branch, but make it optional (e.g. `spring.cloud.config.label=myfeature,develop`).

</div>

</div>

<div class="sect2">

### Security

<div class="paragraph">

If you use HTTP Basic security on the server then clients just need to know the password (and username if it isn’t the default). You can do that via the config server URI, or via separate username and password properties, e.g.

</div>

<div class="listingblock">

<div class="title">bootstrap.yml</div>

<div class="content">

    spring:
      cloud:
        config:
         uri: https://user:secret@myconfig.mycompany.com

</div>

</div>

<div class="paragraph">

or

</div>

<div class="listingblock">

<div class="title">bootstrap.yml</div>

<div class="content">

    spring:
      cloud:
        config:
         uri: https://myconfig.mycompany.com
         username: user
         password: secret

</div>

</div>

<div class="paragraph">

The `spring.cloud.config.password` and `spring.cloud.config.username` values override anything that is provided in the URI.

</div>

<div class="paragraph">

If you deploy your apps on Cloud Foundry then the best way to provide the password is through service credentials, e.g. in the URI, since then it doesn’t even need to be in a config file. An example which works locally and for a user-provided service on Cloud Foundry named "configserver":

</div>

<div class="listingblock">

<div class="title">bootstrap.yml</div>

<div class="content">

    spring:
      cloud:
        config:
         uri: ${vcap.services.configserver.credentials.uri:http://user:password@localhost:8888}

</div>

</div>

<div class="paragraph">

If you use another form of security you might need to provide a `RestTemplate` to the `ConfigServicePropertySourceLocator` (e.g. by grabbing it in the bootstrap context and injecting one).

</div>

</div>

</div>

</div>

# Spring Cloud Netflix

<div class="openblock partintro">

<div class="content">This project provides Netflix OSS integrations for Spring Boot apps through autoconfiguration and binding to the Spring Environment and other Spring programming model idioms. With a few simple annotations you can quickly enable and configure the common patterns inside your application and build large distributed systems with battle-tested Netflix components. The patterns provided include Service Discovery (Eureka), Circuit Breaker (Hystrix), Intelligent Routing (Zuul) and Client Side Load Balancing (Ribbon).</div>

</div>

<div class="sect1">

## Service Discovery: Eureka Clients

<div class="sectionbody">

<div class="paragraph">

Service Discovery is one of the key tenets of a microservice based architecture. Trying to hand configure each client or some form of convention can be very difficult to do and can be very brittle. Eureka is the Netflix Service Discovery Server and Client. The server can be configured and deployed to be highly available, with each server replicating state about the registered services to the others.

</div>

<div class="sect2">

### Registering with Eureka

<div class="paragraph">

When a client registers with Eureka, it provides meta-data about itself such as host and port, health indicator URL, home page etc. Eureka receives heartbeat messages from each instance belonging to a service. If the heartbeat fails over a configurable timetable, the instance is normally removed from the registry.

</div>

<div class="paragraph">

Example eureka client:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="paragraph">

(i.e. utterly normal Spring Boot app). In this example we use `@EnableEurekaClient` explicitly, but with only Eureka available you could also use `@EnableDiscoveryClient`. Configuration is required to locate the Eureka server. Example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>eureka:
  client:
    serviceUrl:
      defaultZone: http://localhost:8761/eureka/</pre>

</div>

</div>

<div class="paragraph">

where "defaultZone" is a magic string fallback value that provides the service URL for any client that doesn’t express a preference (i.e. it’s a useful default).

</div>

<div class="paragraph">

The default application name (service ID), virtual host and non-secure port, taken from the `Environment`, are `${spring.application.name}`, `${spring.application.name}` and `${server.port}` respectively.

</div>

<div class="paragraph">

`@EnableEurekaClient` makes the app into both a Eureka "instance" (i.e. it registers itself) and a "client" (i.e. it can query the registry to locate other services). The instance behaviour is driven by `eureka.instance.*` configuration keys, but the defaults will be fine if you ensure that your application has a `spring.application.name` (this is the default for the Eureka service ID, or VIP).

</div>

<div class="paragraph">

See [EurekaInstanceConfigBean](https://github.com/%7Bgithub-repo%7D/tree/%7Bgithub-tag%7D/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java) and [EurekaClientConfigBean](https://github.com/%7Bgithub-repo%7D/tree/%7Bgithub-tag%7D/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/eureka/EurekaClientConfigBean.java) for more details of the configurable options.

</div>

</div>

<div class="sect2">

### Status Page and Health Indicator

<div class="paragraph">

The status page and health indicators for a Eureka instance default to "/info" and "/health" respectively, which are the default locations of useful endpoints in a Spring Boot Actuator application. You need to change these, even for an Actuator application if you use a non-default context path or servlet path (e.g. `server.servletPath=/foo`) or management endpoint path (e.g. `management.contextPath=/admin`). Example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>eureka:
  instance:
    statusPageUrlPath: ${management.context-path}/info
    healthCheckUrlPath: ${management.context-path}/health</pre>

</div>

</div>

<div class="paragraph">

These links show up in the metadata that is consumed by clients, and used in some scenarios to decide whether to send requests to your application, so it’s helpful if they are accurate.

</div>

</div>

<div class="sect2">

### Registering a Secure Application

<div class="paragraph">

If your app wants to be contacted over HTTPS you can set two flags in the `EurekaInstanceConfig`, _viz_ `eureka.instance.[nonSecurePortEnabled,securePortEnabled]=[false,true]` respectively. This will make Eureka publish instance information showing an explicit preference for secure communication. The Spring Cloud `DiscoveryClient` will always return an `[https://…​](https://%E2%80%A6%E2%80%8B/);` URI for a service configured this way, and the Eureka (native) instance information will have a secure health check URL.

</div>

<div class="paragraph">

Because of the way Eureka works internally, it will still publish a non-secure URL for status and home page unless you also override those explicitly. You can use placeholders to configure the eureka instance urls, e.g.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>eureka:
  instance:
    statusPageUrl: https://${eureka.hostname}/info
    healthCheckUrl: https://${eureka.hostname}/health
    homePageUrl: https://${eureka.hostname}/</pre>

</div>

</div>

<div class="paragraph">

(Note that `${eureka.hostname}` is a native placeholder only available in later versions of Eureka. You could achieve the same thing with Spring placeholders as well, e.g. using `${eureka.instance.hostName}`.)

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">If your app is running behind a proxy, and the SSL termination is in the proxy (e.g. if you run in Cloud Foundry or other platforms as a service) then you will need to ensure that the proxy "forwarded" headers are intercepted and handled by the application. An embedded Tomcat container in a Spring Boot app does this automatically if it has explicit configuration for the 'X-Forwarded-\*` headers. A sign that you got this wrong will be that the links rendered by your app to itself will be wrong (the wrong host, port or protocol).</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Eureka’s Health Checks

<div class="paragraph">

By default, Eureka uses the client heartbeat to determine if a client is up. Unless specified otherwise the Discovery Client will not propagate the current health check status of the application per the Spring Boot Actuator. Which means that after successful registration Eureka will always announce that the application is in 'UP' state. This behaviour can be altered by enabling Eureka health checks, which results in propagating application status to Eureka. As a consequence every other application won’t be sending traffic to application in state other then 'UP'.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>eureka:
  client:
    healthcheck:
      enabled: true</pre>

</div>

</div>

<div class="paragraph">

If you require more control over the health checks, you may consider implementing your own `com.netflix.appinfo.HealthCheckHandler`.

</div>

</div>

<div class="sect2">

### Eureka Metadata for Instances and Clients

<div class="paragraph">

It’s worth spending a bit of time understanding how the Eureka metadata works, so you can use it in a way that makes sense in your platform. There is standard metadata for things like hostname, IP address, port numbers, status page and health check. These are published in the service registry and used by clients to contact the services in a straightforward way. Additional metadata can be added to the instance registration in the `eureka.instance.metadataMap`, and this will be accessible in the remote clients, but in general will not change the behaviour of the client, unless it is made aware of the meaning of the metadata. There are a couple of special cases described below where Spring Cloud already assigns meaning to the metadata map.

</div>

<div class="sect3">

#### Using Eureka on Cloudfoundry

<div class="paragraph">

Cloudfoundry has a global router so that all instances of the same app have the same hostname (it’s the same in other PaaS solutions with a similar architecture). This isn’t necessarily a barrier to using Eureka, but if you use the router (recommended, or even mandatory depending on the way your platform was set up), you need to explicitly set the hostname and port numbers (secure or non-secure) so that they use the router. You might also want to use instance metadata so you can distinguish between the instances on the client (e.g. in a custom load balancer). By default, the `eureka.instance.instanceId` is `vcap.application.instance_id`. For example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>eureka:
  instance:
    hostname: ${vcap.application.uris[0]}
    nonSecurePort: 80</pre>

</div>

</div>

<div class="paragraph">

Depending on the way the security rules are set up in your Cloudfoundry instance, you might be able to register and use the IP address of the host VM for direct service-to-service calls. This feature is not (yet) available on Pivotal Web Services ([PWS](https://run.pivotal.io/)).

</div>

</div>

<div class="sect3">

#### Using Eureka on AWS

<div class="paragraph">

If the application is planned to be deployed to an AWS cloud, then the Eureka instance will have to be configured to be Amazon aware and this can be done by customizing the [EurekaInstanceConfigBean](https://github.com/%7Bgithub-repo%7D/tree/%7Bgithub-tag%7D/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/eureka/EurekaInstanceConfigBean.java) the following way:

</div>

<div class="listingblock">

<div class="content">

    @Bean
    @Profile("!default")
    public EurekaInstanceConfigBean eurekaInstanceConfig() {
      EurekaInstanceConfigBean b = new EurekaInstanceConfigBean();
      AmazonInfo info = AmazonInfo.Builder.newBuilder().autoBuild("eureka");
      b.setDataCenterInfo(info);
      return b;
    }

</div>

</div>

</div>

<div class="sect3">

#### Changing the Eureka Instance ID

<div class="paragraph">

A vanilla Netflix Eureka instance is registered with an ID that is equal to its host name (i.e. only one service per host). Spring Cloud Eureka provides a sensible default that looks like this: `${spring.cloud.client.hostname}:${spring.application.name}:${spring.application.instance_id:${server.port}}}`. For example `myhost:myappname:8080`.

</div>

<div class="paragraph">

Using Spring Cloud you can override this by providing a unique identifier in `eureka.instance.instanceId`. For example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>eureka:
  instance:
    instanceId: ${spring.application.name}:${spring.application.instance_id:${random.value}}</pre>

</div>

</div>

<div class="paragraph">

With this metadata, and multiple service instances deployed on localhost, the random value will kick in there to make the instance unique. In Cloudfoundry the `spring.application.instance_id` will be populated automatically in a Spring Boot Actuator application, so the random value will not be needed.

</div>

</div>

</div>

<div class="sect2">

### Using the EurekaClient

<div class="paragraph">

Once you have an app that is `@EnableDiscoveryClient` (or `@EnableEurekaClient`) you can use it to discover service instances from the [Eureka Server](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-eureka-server). One way to do that is to use the native `com.netflix.discovery.EurekaClient` (as opposed to the Spring Cloud `DiscoveryClient`), e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>@Autowired
private EurekaClient discoveryClient;

public String serviceUrl() {
    InstanceInfo instance = discoveryClient.getNextServerFromEureka("STORES", false);
    return instance.getHomePageUrl();
}</pre>

</div>

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">

<div class="paragraph">

Don’t use the `EurekaClient` in `@PostConstruct` method or in a `@Scheduled` method (or anywhere where the `ApplicationContext` might not be started yet). It is initialized in a `SmartLifecycle` (with `phase=0`) so the earliest you can rely on it being available is in another `SmartLifecycle` with higher phase.

</div>

</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Alternatives to the native Netflix EurekaClient

<div class="paragraph">

You don’t have to use the raw Netflix `EurekaClient` and usually it is more convenient to use it behind a wrapper of some sort. Spring Cloud has support for [Feign](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-feign) (a REST client builder) and also [Spring `RestTemplate`](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon) using the logical Eureka service identifiers (VIPs) instead of physical URLs. To configure Ribbon with a fixed list of physical servers you can simply set `<client>.ribbon.listOfServers` to a comma-separated list of physical addresses (or hostnames), where `<client>` is the ID of the client.

</div>

<div class="paragraph">

You can also use the `org.springframework.cloud.client.discovery.DiscoveryClient` which provides a simple API for discovery clients that is not specific to Netflix, e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>@Autowired
private DiscoveryClient discoveryClient;

public String serviceUrl() {
    List<ServiceInstance> list = client.getInstances("STORES");
    if (list != null && list.size() > 0 ) {
        return list.get(0).getUri();
    }
    return null;
}</pre>

</div>

</div>

</div>

<div class="sect2">

### Why is it so Slow to Register a Service?

<div class="paragraph">

Being an instance also involves a periodic heartbeat to the registry (via the client’s `serviceUrl`) with default duration 30 seconds. A service is not available for discovery by clients until the instance, the server and the client all have the same metadata in their local cache (so it could take 3 hearbeats). You can change the period using `eureka.instance.leaseRenewalIntervalInSeconds` and this will speed up the process of getting clients connected to other services. In production it’s probably better to stick with the default because there are some computations internally in the server that make assumptions about the lease renewal period.

</div>

</div>

</div>

</div>

<div class="sect1">

## Service Discovery: Eureka Server

<div class="sectionbody">

<div class="paragraph">

Example eureka server (e.g. using spring-cloud-starter-eureka-server to set up the classpath):

</div>

<div class="listingblock">

<div class="content">

    @SpringBootApplication
    @EnableEurekaServer
    public class Application {

        public static void main(String[] args) {
            new SpringApplicationBuilder(Application.class).web(true).run(args);
        }

    }

</div>

</div>

<div class="paragraph">

The server has a home page with a UI, and HTTP API endpoints per the normal Eureka functionality under `/eureka/*`.

</div>

<div class="paragraph">

Eureka background reading: see [flux capacitor](https://github.com/cfregly/fluxcapacitor/wiki/NetflixOSS-FAQ#eureka-service-discovery-load-balancer) and [google group discussion](https://groups.google.com/forum/?fromgroups#!topic/eureka_netflix/g3p2r7gHnN0).

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">

<div class="paragraph">

Due to Gradle’s dependency resolution rules and the lack of a parent bom feature, simply depending on spring-cloud-starter-eureka-server can cause failures on application startup. To remedy this the Spring dependency management plugin must be added and the Spring cloud starter parent bom must be imported like so:

</div>

<div class="listingblock">

<div class="title">build.gradle</div>

<div class="content">

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

</div>

</div>

</td>

</tr>

</tbody>

</table>

</div>

<div class="sect2">

### High Availability, Zones and Regions

<div class="paragraph">

The Eureka server does not have a backend store, but the service instances in the registry all have to send heartbeats to keep their registrations up to date (so this can be done in memory). Clients also have an in-memory cache of eureka registrations (so they don’t have to go to the registry for every single request to a service).

</div>

<div class="paragraph">

By default every Eureka server is also a Eureka client and requires (at least one) service URL to locate a peer. If you don’t provide it the service will run and work, but it will shower your logs with a lot of noise about not being able to register with the peer.

</div>

<div class="paragraph">

See also [below for details of Ribbon support](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon) on the client side for Zones and Regions.

</div>

</div>

<div class="sect2">

### Standalone Mode

<div class="paragraph">

The combination of the two caches (client and server) and the heartbeats make a standalone Eureka server fairly resilient to failure, as long as there is some sort of monitor or elastic runtime keeping it alive (e.g. Cloud Foundry). In standalone mode, you might prefer to switch off the client side behaviour, so it doesn’t keep trying and failing to reach its peers. Example:

</div>

<div class="listingblock">

<div class="title">application.yml (Standalone Eureka Server)</div>

<div class="content">

<pre>server:
  port: 8761

eureka:
  instance:
    hostname: localhost
  client:
    registerWithEureka: false
    fetchRegistry: false
    serviceUrl:
      defaultZone: http://${eureka.instance.hostname}:${server.port}/eureka/</pre>

</div>

</div>

<div class="paragraph">

Notice that the `serviceUrl` is pointing to the same host as the local instance.

</div>

</div>

<div class="sect2">

### Peer Awareness

<div class="paragraph">

Eureka can be made even more resilient and available by running multiple instances and asking them to register with each other. In fact, this is the default behaviour, so all you need to do to make it work is add a valid `serviceUrl` to a peer, e.g.

</div>

<div class="listingblock">

<div class="title">application.yml (Two Peer Aware Eureka Servers)</div>

<div class="content">

<pre>---
spring:
  profiles: peer1
eureka:
  instance:
    hostname: peer1
  client:
    serviceUrl:
      defaultZone: http://peer2/eureka/

---
spring:
  profiles: peer2
eureka:
  instance:
    hostname: peer2
  client:
    serviceUrl:
      defaultZone: http://peer1/eureka/</pre>

</div>

</div>

<div class="paragraph">

In this example we have a YAML file that can be used to run the same server on 2 hosts (peer1 and peer2), by running it in different Spring profiles. You could use this configuration to test the peer awareness on a single host (there’s not much value in doing that in production) by manipulating `/etc/hosts` to resolve the host names. In fact, the `eureka.instance.hostname` is not needed if you are running on a machine that knows its own hostname (it is looked up using `java.net.InetAddress` by default).

</div>

<div class="paragraph">

You can add multiple peers to a system, and as long as they are all connected to each other by at least one edge, they will synchronize the registrations amongst themselves. If the peers are physically separated (inside a data centre or between multiple data centres) then the system can in principle survive split-brain type failures.

</div>

</div>

<div class="sect2">

### Prefer IP Address

<div class="paragraph">

In some cases, it is preferable for Eureka to advertise the IP Adresses of services rather than the hostname. Set `eureka.instance.preferIpAddress` to `true` and when the application registers with eureka, it will use its IP Address rather than its hostname.

</div>

</div>

</div>

</div>

<div class="sect1">

## Circuit Breaker: Hystrix Clients

<div class="sectionbody">

<div class="paragraph">

Netflix has created a library called [Hystrix](https://github.com/Netflix/Hystrix) that implements the [circuit breaker pattern](http://martinfowler.com/bliki/CircuitBreaker.html). In a microservice architecture it is common to have multiple layers of service calls.

</div>

<div class="imageblock">

<div class="content">![HystrixGraph](./Spring Cloud_EN_files/HystrixGraph.png)</div>

<div class="title">Figure 1\. Microservice Graph</div>

</div>

<div class="paragraph">

A service failure in the lower level of services can cause cascading failure all the way up to the user. When calls to a particular service reach a certain threshold (20 failures in 5 seconds is the default in Hystrix), the circuit opens and the call is not made. In cases of error and an open circuit a fallback can be provided by the developer.

</div>

<div class="imageblock">

<div class="content">![HystrixFallback](./Spring Cloud_EN_files/HystrixFallback.png)</div>

<div class="title">Figure 2\. Hystrix fallback prevents cascading failures</div>

</div>

<div class="paragraph">

Having an open circuit stops cascading failures and allows overwhelmed or failing services time to heal. The fallback can be another Hystrix protected call, static data or a sane empty value. Fallbacks may be chained so the first fallback makes some other business call which in turn falls back to static data.

</div>

<div class="paragraph">

Example boot app:

</div>

<div class="listingblock">

<div class="content">

<pre>@SpringBootApplication
@EnableCircuitBreaker
public class Application {

    public static void main(String[] args) {
        new SpringApplicationBuilder(Application.class).web(true).run(args);
    }

}

@Component
public class StoreIntegration {

    @HystrixCommand(fallbackMethod = "defaultStores")
    public Object getStores(Map<String, Object> parameters) {
        //do stuff that might fail
    }

    public Object defaultStores(Map<String, Object> parameters) {
        return /* something useful */;
    }
}</pre>

</div>

</div>

<div class="paragraph">

The `@HystrixCommand` is provided by a Netflix contrib library called ["javanica"](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica). Spring Cloud automatically wraps Spring beans with that annotation in a proxy that is connected to the Hystrix circuit breaker. The circuit breaker calculates when to open and close the circuit, and what to do in case of a failure.

</div>

<div class="paragraph">

To configure the `@HystrixCommand` you can use the `commandProperties` attribute with a list of `@HystrixProperty` annotations. See [here](https://github.com/Netflix/Hystrix/tree/master/hystrix-contrib/hystrix-javanica#configuration) for more details. See the [Hystrix wiki](https://github.com/Netflix/Hystrix/wiki/Configuration) for details on the properties available.

</div>

<div class="sect2">

### Propagating the Security Context or using Spring Scopes

<div class="paragraph">

If you want some thread local context to propagate into a `@HystrixCommand` the default declaration will not work because it executes the command in a thread pool (in case of timeouts). You can switch Hystrix to use the same thread as the caller using some configuration, or directly in the annotation, by asking it to use a different "Isolation Strategy". For example:

</div>

<div class="listingblock">

<div class="content">

    @HystrixCommand(fallbackMethod = "stubMyService",
        commandProperties = {
          @HystrixProperty(name="execution.isolation.strategy", value="SEMAPHORE")
        }
    )
    ...

</div>

</div>

<div class="paragraph">

The same thing applies if you are using `@SessionScope` or `@RequestScope`. You will know when you need to do this because of a runtime exception that says it can’t find the scoped context.

</div>

</div>

<div class="sect2">

### Health Indicator

<div class="paragraph">

The state of the connected circuit breakers are also exposed in the `/health` endpoint of the calling application.

</div>

<div class="listingblock">

<div class="content">

    {
        "hystrix": {
            "openCircuitBreakers": [
                "StoreIntegration::getStoresByLocationLink"
            ],
            "status": "CIRCUIT_OPEN"
        },
        "status": "UP"
    }

</div>

</div>

</div>

<div class="sect2">

### Hystrix Metrics Stream

<div class="paragraph">

To enable the Hystrix metrics stream include a dependency on `spring-boot-starter-actuator`. This will expose the `/hystrix.stream` as a management endpoint.

</div>

<div class="listingblock">

<div class="content">

        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-actuator</artifactId>
        </dependency>

</div>

</div>

</div>

</div>

</div>

<div class="sect1">

## Circuit Breaker: Hystrix Dashboard

<div class="sectionbody">

<div class="paragraph">

One of the main benefits of Hystrix is the set of metrics it gathers about each HystrixCommand. The Hystrix Dashboard displays the health of each circuit breaker in an efficient manner.

</div>

<div class="imageblock">

<div class="content">![Hystrix](./Spring Cloud_EN_files/Hystrix.png)</div>

<div class="title">Figure 3\. Hystrix Dashboard</div>

</div>

<div class="paragraph">

To run the Hystrix Dashboard annotate your Spring Boot main class with `@EnableHystrixDashboard`. You then visit `/hystrix` and point the dashboard to an individual instances `/hystrix.stream` endpoint in a Hystrix client application.

</div>

<div class="sect2">

### Turbine

<div class="paragraph">

Looking at an individual instances Hystrix data is not very useful in terms of the overall health of the system. [Turbine](https://github.com/Netflix/Turbine) is an application that aggregates all of the relevant `/hystrix.stream` endpoints into a combined `/turbine.stream` for use in the Hystrix Dashboard. Individual instances are located via Eureka. Running Turbine is as simple as annotating your main class with the `@EnableTurbine` annotation (e.g. using spring-cloud-starter-turbine to set up the classpath). All of the documented configuration properties from [the Turbine 1 wiki](https://github.com/Netflix/Turbine/wiki/Configuration-(1.x)) apply. The only difference is that the `turbine.instanceUrlSuffix` does not need the port prepended as this is handled automatically unless `turbine.instanceInsertPort=false`.

</div>

<div class="paragraph">

The configuration key `turbine.appConfig` is a list of eureka serviceIds that turbine will use to lookup instances. The turbine stream is then used in the Hystrix dashboard using a url that looks like: `[http://my.turbine.sever:8080/turbine.stream?cluster=<CLUSTERNAME>](http://my.turbine.sever:8080/turbine.stream?cluster=%3CCLUSTERNAME%3E);` (the cluster parameter can be omitted if the name is "default"). The `cluster` parameter must match an entry in `turbine.aggregator.clusterConfig`. Values returned from eureka are uppercase, thus we expect this example to work if there is an app registered with Eureka called "customers":

</div>

<div class="listingblock">

<div class="content">

<pre>turbine:
  aggregator:
    clusterConfig: CUSTOMERS
  appConfig: customers</pre>

</div>

</div>

<div class="paragraph">

The `clusterName` can be customized by a SPEL expression in `turbine.clusterNameExpression` with root an instance of `InstanceInfo`. The default value is `appName`, which means that the Eureka serviceId ends up as the cluster key (i.e. the `InstanceInfo` for customers has an `appName` of "CUSTOMERS"). A different example would be `turbine.clusterNameExpression=aSGName`, which would get the cluster name from the AWS ASG name. Another example:

</div>

<div class="listingblock">

<div class="content">

<pre>turbine:
  aggregator:
    clusterConfig: SYSTEM,USER
  appConfig: customers,stores,ui,admin
  clusterNameExpression: metadata['cluster']</pre>

</div>

</div>

<div class="paragraph">

In this case, the cluster name from 4 services is pulled from their metadata map, and is expected to have values that include "SYSTEM" and "USER".

</div>

<div class="paragraph">

To use the "default" cluster for all apps you need a string literal expression (with single quotes):

</div>

<div class="listingblock">

<div class="content">

<pre>turbine:
  appConfig: customers,stores
  clusterNameExpression: 'default'</pre>

</div>

</div>

<div class="paragraph">

Spring Cloud provides a `spring-cloud-starter-turbine` that has all the dependencies you need to get a Turbine server running. Just create a Spring Boot application and annotate it with `@EnableTurbine`.

</div>

</div>

<div class="sect2">

### Turbine AMQP

<div class="paragraph">

In some environments (e.g. in a PaaS setting), the classic Turbine model of pulling metrics from all the distributed Hystrix commands doesn’t work. In that case you might want to have your Hystrix commands push metrics to Turbine, and Spring Cloud enables that with AMQP messaging. All you need to do on the client is add a dependency to `spring-cloud-netflix-hystrix-amqp` and make sure there is a Rabbit broker available (see Spring Boot documentation for details on how to configure the client credentials, but it should work out of the box for a local broker or in Cloud Foundry).

</div>

<div class="paragraph">

On the server side Just create a Spring Boot application and annotate it with `@EnableTurbineAmqp` and by default it will come up on port 8989 (point your Hystrix dashboard to that port, any path). You can customize the port using either `server.port` or `turbine.amqp.port`. If you have `spring-boot-starter-web` and `spring-boot-starter-actuator` on the classpath as well, then you can open up the Actuator endpoints on a separate port (with Tomcat by default) by providing a `management.port` which is different.

</div>

<div class="paragraph">

You can then point the Hystrix Dashboard to the Turbine AMQP Server instead of individual Hystrix streams. If Turbine AMQP is running on port 8989 on myhost, then put `[http://myhost:8989](http://myhost:8989/)` in the stream input field in the Hystrix Dashboard. Circuits will be prefixed by their respective serviceId, followed by a dot, then the circuit name.

</div>

<div class="paragraph">

Spring Cloud provides a `spring-cloud-starter-turbine-amqp` that has all the dependencies you need to get a Turbine AMQP server running. You need Java 8 to run the app because it is Netty-based.

</div>

</div>

</div>

</div>

<div class="sect1">

## Customizing the AMQP ConnectionFactory

<div class="sectionbody">

<div class="paragraph">

If you are using AMQP there needs to be a `ConnectionFactory` (from Spring Rabbit) in the application context. If there is a single `ConnectionFactory` it will be used, or if there is a one qualified as `@HystrixConnectionFactory` (on the client) and `@TurbineConnectionFactory` (on the server) it will be preferred over others, otherwise the `@Primary` one will be used. If there are multiple unqualified connection factories there will be an error.

</div>

<div class="paragraph">

Note that Spring Boot (as of 1.2.2) creates a `ConnectionFactory` that is _not_ `@Primary`, so if you want to use one connection factory for the bus and another for business messages, you need to create both, and annotate them `@*ConnectionFactory` and `@Primary` respectively.

</div>

</div>

</div>

<div class="sect1">

## Client Side Load Balancer: Ribbon

<div class="sectionbody">

<div class="paragraph">

Ribbon is a client side load balancer which gives you a lot of control over the behaviour of HTTP and TCP clients. Feign already uses Ribbon, so if you are using `@FeignClient` then this section also applies.

</div>

<div class="paragraph">

A central concept in Ribbon is that of the named client. Each load balancer is part of an ensemble of components that work together to contact a remote server on demand, and the ensemble has a name that you give it as an application developer (e.g. using the `@FeignClient` annotation). Spring Cloud creates a new ensemble as an `ApplicationContext` on demand for each named client using `RibbonClientConfiguration`. This contains (amongst other things) an `ILoadBalancer`, a `RestClient`, and a `ServerListFilter`.

</div>

<div class="sect2">

### Customizing the Ribbon Client

<div class="paragraph">

You can configure some bits of a Ribbon client using external properties in `<client>.ribbon.*`, which is no different than using the Netflix APIs natively, except that you can use Spring Boot configuration files. The native options can be inspected as static fields in `CommonClientConfigKey` (part of ribbon-core).

</div>

<div class="paragraph">

Spring Cloud also lets you take full control of the client by declaring additional configuration (on top of the `RibbonClientConfiguration`) using `@RibbonClient`. Example:

</div>

<div class="listingblock">

<div class="content">

    @Configuration
    @RibbonClient(name = "foo", configuration = FooConfiguration.class)
    public class TestConfiguration {
    }

</div>

</div>

<div class="paragraph">

In this case the client is composed from the components already in `RibbonClientConfiguration` together with any in `FooConfiguration` (where the latter generally will override the former).

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">The `FooConfiguration` has to be `@Configuration` but take care that it is not in a `@ComponentScan` for the main application context, otherwise it will be shared by all the `@RibbonClients`. If you use `@ComponentScan` (or `@SpringBootApplication`) you need to take steps to avoid it being included (for instance put it in a separate, non-overlapping package, or specify the packages to scan explicitly in the `@ComponentScan`).</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

Spring Cloud Netflix provides the following beans by default for ribbon (`BeanType` beanName: `ClassName`):

</div>

<div class="ulist">

*   `IClientConfig` ribbonClientConfig: `DefaultClientConfigImpl`

*   `IRule` ribbonRule: `ZoneAvoidanceRule`

*   `IPing` ribbonPing: `NoOpPing`

*   `ServerList<Server>` ribbonServerList: `ConfigurationBasedServerList`

*   `ServerListFilter<Server>` ribbonServerListFilter: `ZonePreferenceServerListFilter`

*   `ILoadBalancer` ribbonLoadBalancer: `ZoneAwareLoadBalancer`

</div>

<div class="paragraph">

Creating a bean of one of those type and placing it in a `@RibbonClient` configuration (such as `FooConfiguration` above) allows you to override each one of the beans described. Example:

</div>

<div class="listingblock">

<div class="content">

    @Configuration
    public class FooConfiguration {
        @Bean
        public IPing ribbonPing(IClientConfig config) {
            return new PingUrl();
        }
    }

</div>

</div>

<div class="paragraph">

This replaces the `NoOpPing` with `PingUrl`.

</div>

</div>

<div class="sect2">

### Using Ribbon with Eureka

<div class="paragraph">

When Eureka is used in conjunction with Ribbon the `ribbonServerList` is overridden with an extension of `DiscoveryEnabledNIWSServerList` which populates the list of servers from Eureka. It also replaces the `IPing` interface with `NIWSDiscoveryPing` which delegates to Eureka to determine if a server is up. The `ServerList` that is installed by default is a `DomainExtractingServerList` and the purpose of this is to make physical metadata available to the load balancer without using AWS AMI metadata (which is what Netflix relies on). By default the server list will be constructed with "zone" information as provided in the instance metadata (so on the client set `eureka.instance.metadataMap.zone`), and if that is missing it can use the domain name from the server hostname as a proxy for zone (if the flag `approximateZoneFromHostname` is set). Once the zone information is available it can be used in a `ServerListFilter` (by default it will be used to locate a server in the same zone as the client because the default is a `ZonePreferenceServerListFilter`).

</div>

</div>

<div class="sect2">

### Example: How to Use Ribbon Without Eureka

<div class="paragraph">

Eureka is a convenient way to abstract the discovery of remote servers so you don’t have to hard code their URLs in clients, but if you prefer not to use it, Ribbon and Feign are still quite amenable. Suppose you have declared a `@RibbonClient` for "stores", and Eureka is not in use (and not even on the classpath). The Ribbon client defaults to a configured server list, and you can supply the configuration like this

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>stores:
  ribbon:
    listOfServers: example.com,google.com</pre>

</div>

</div>

</div>

<div class="sect2">

### Example: Disable Eureka use in Ribbon

<div class="paragraph">

Setting the property `ribbon.eureka.enabled = false` will explicitly disable the use of Eureka in Ribbon.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>ribbon:
  eureka:
   enabled: false</pre>

</div>

</div>

</div>

<div class="sect2">

### Using the Ribbon API Directly

<div class="paragraph">

You can also use the `LoadBalancerClient` directly. Example:

</div>

<div class="listingblock">

<div class="content">

    public class MyClass {
        @Autowired
        private LoadBalancerClient loadBalancer;

        public void doStuff() {
            ServiceInstance instance = loadBalancer.choose("stores");
            URI storesUri = URI.create(String.format("http://%s:%s", instance.getHost(), instance.getPort()));
            // ... do something with the URI
        }
    }

</div>

</div>

</div>

</div>

</div>

<div class="sect1">

## Declarative REST Client: Feign

<div class="sectionbody">

<div class="paragraph">

[Feign](https://github.com/Netflix/feign) is a declarative web service client. It makes writing web service clients easier. To use Feign create an interface and annotate it. It has pluggable annotation support including Feign annotations and JAX-RS annotations. Feign also supports pluggable encoders and decoders. Spring Cloud adds support for Spring MVC annotations and for using the same `HttpMessageConverters` used by default in Spring Web. Spring Cloud integrates Ribbon and Eureka to provide a load balanced http client when using Feign.

</div>

<div class="paragraph">

Example spring boot app

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="listingblock">

<div class="title">StoreClient.java</div>

<div class="content">

    @FeignClient("stores")
    public interface StoreClient {
        @RequestMapping(method = RequestMethod.GET, value = "/stores")
        List<Store> getStores();

        @RequestMapping(method = RequestMethod.POST, value = "/stores/{storeId}", consumes = "application/json")
        Store update(@PathVariable("storeId") Long storeId, Store store);
    }

</div>

</div>

<div class="paragraph">

In the `@FeignClient` annotation the String value ("stores" above) is an arbitrary client name, which is used to create a Ribbon load balancer (see [below for details of Ribbon support](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon)). You can also specify a URL using the `url` attribute (absolute value or just a hostname).

</div>

<div class="paragraph">

The Ribbon client above will want to discover the physical addresses for the "stores" service. If your application is a Eureka client then it will resolve the service in the Eureka service registry. If you don’t want to use Eureka, you can simply configure a list of servers in your external configuration (see [above for example](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon-without-eureka)).

</div>

<div class="sect2">

### Overriding Feign Defaults

<div class="paragraph">

A central concept in Spring Cloud’s Feign support is that of the named client. Each feign client is part of an ensemble of components that work together to contact a remote server on demand, and the ensemble has a name that you give it as an application developer using the `@FeignClient` annotation. Spring Cloud creates a new ensemble as an `ApplicationContext` on demand for each named client using `FeignClientsConfiguration`. This contains (amongst other things) an `feign.Decoder`, a `feign.Encoder`, and a `feign.Contract`.

</div>

<div class="paragraph">

Spring Cloud lets you take full control of the feign client by declaring additional configuration (on top of the `FeignClientsConfiguration`) using `@FeignClient`. Example:

</div>

<div class="listingblock">

<div class="content">

    @FeignClient(name = "stores", configuration = FooConfiguration.class)
    public interface StoreClient {
        //..
    }

</div>

</div>

<div class="paragraph">

In this case the client is composed from the components already in `FeignClientsConfiguration` together with any in `FooConfiguration` (where the latter will override the former).

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">The `FooConfiguration` has to be `@Configuration` but take care that it is not in a `@ComponentScan` for the main application context, otherwise it will be used for every `@FeignClient`. If you use `@ComponentScan` (or `@SpringBootApplication`) you need to take steps to avoid it being included (for instance put it in a separate, non-overlapping package, or specify the packages to scan explicitly in the `@ComponentScan`).</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">The `serviceId` attribute is now deprecated in favor of the `name` attribute.</td>

</tr>

</tbody>

</table>

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">Previously, using the `url` attribute, did not require the `name` attribute. Using `name` is now required.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

Placeholders are supported in the `name` and `url` attributes.

</div>

<div class="listingblock">

<div class="content">

    @FeignClient(name = "${feign.name}", url = "${feign.url}")
    public interface StoreClient {
        //..
    }

</div>

</div>

<div class="paragraph">

Spring Cloud Netflix provides the following beans by default for feign (`BeanType` beanName: `ClassName`):

</div>

<div class="ulist">

*   `Decoder` feignDecoder: `ResponseEntityDecoder` (which wraps a `SpringDecoder`)

*   `Encoder` feignEncoder: `SpringEncoder`

*   `Logger` feignLogger: `Slf4jLogger`

*   `Contract` feignContract: `SpringMvcContract`

*   `Feign.Builder` feignBuilder: `HystrixFeign.Builder`

</div>

<div class="paragraph">

Spring Cloud Netflix _does not_ provide the following beans by default for feign, but still looks up beans of these types from the application context to create the feign client:

</div>

<div class="ulist">

*   `Logger.Level`

*   `Retryer`

*   `ErrorDecoder`

*   `Request.Options`

*   `Collection<RequestInterceptor>`

</div>

<div class="paragraph">

Creating a bean of one of those type and placing it in a `@FeignClient` configuration (such as `FooConfiguration` above) allows you to override each one of the beans described. Example:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="paragraph">

This replaces the `SpringMvcContract` with `feign.Contract.Default` and adds a `RequestInterceptor` to the collection of `RequestInterceptor`.

</div>

<div class="paragraph">

Default configurations can be specified in the `@EnableFeignClients` attribute `defaultConfiguration` in a similar manner as described above. The difference is that this configuration will apply to _all_ feign clients.

</div>

</div>

<div class="sect2">

### Feign Hystrix Support

<div class="paragraph">

If Hystrix is on the classpath, by default Feign will wrap all methods with a circuit breaker. Returning a `com.netflix.hystrix.HystrixCommand` is also available. This lets you use reactive patterns (with a call to `.toObservable()` or `.observe()` or asynchronous use (with a call to `.queue()`).

</div>

<div class="paragraph">

To disable Hystrix support for Feign, set `feign.hystrix.enabled=false`.

</div>

<div class="paragraph">

To disable Hystrix support on a per-client basis create a vanilla `Feign.Builder` with the "prototype" scope, e.g.:

</div>

<div class="listingblock">

<div class="content">

    @Configuration
    public class FooConfiguration {
        @Bean
        @Scope("prototype")
        public Feign.Builder feignBuilder() {
            return Feign.builder();
        }
    }

</div>

</div>

</div>

<div class="sect2">

### Feign Hystrix Fallbacks

<div class="paragraph">

Hystrix supports the notion of a fallback: a default code path that is executed when they circuit is open or there is an error. To enable fallbacks for a given `@FeignClient` set the `fallback` attribute to the class name that implements the fallback.

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">There is a limitation with the implementation of fallbacks in Feign and how Hystrix fallbacks work. Fallbacks are currently not supported for methods that return `com.netflix.hystrix.HystrixCommand` and `rx.Observable`.</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Feign Inheritance Support

<div class="paragraph">

Feign supports boilerplate apis via single-inheritance interfaces. This allows grouping common operations into convenient base interfaces. Together with Spring MVC you can share the same contract for your REST endpoint and Feign client.

</div>

<div class="listingblock">

<div class="title">UserService.java</div>

<div class="content">

    public interface UserService {

        @RequestMapping(method = RequestMethod.GET, value ="/users/{id}")
        User getUser(@PathVariable("id") long id);
    }

</div>

</div>

<div class="listingblock">

<div class="title">UserResource.java</div>

<div class="content">

    @RestController
    public class UserResource implements UserService {

    }

</div>

</div>

<div class="listingblock">

<div class="title">UserClient.java</div>

<div class="content">

    package project.user;

    @FeignClient("users")
    public interface UserClient extends UserService {

    }

</div>

</div>

</div>

<div class="sect2">

### Feign request/response compression

<div class="paragraph">

You may consider enabling the request or response GZIP compression for your Feign requests. You can do this by enabling one of the properties:

</div>

<div class="listingblock">

<div class="content">

    feign.compression.request.enabled=true
    feign.compression.response.enabled=true

</div>

</div>

<div class="paragraph">

Feign request compression gives you settings similar to what you may set for your web server:

</div>

<div class="listingblock">

<div class="content">

    feign.compression.request.enabled=true
    feign.compression.request.mime-types=text/xml,application/xml,application/json
    feign.compression.request.min-request-size=2048

</div>

</div>

<div class="paragraph">

These properties allow you to be selective about the compressed media types and minimum request threshold length.

</div>

</div>

<div class="sect2">

### Feign logging

<div class="paragraph">

A logger is created for each Feign client created. By default the name of the logger is the full class name of the interface used to create the Feign client. Feign logging only responds to the `DEBUG` level.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

    logging.level.project.user.UserClient: DEBUG

</div>

</div>

<div class="paragraph">

The `Logger.Level` object that you may configure per client, tells Feign how much to log. Choices are:

</div>

<div class="ulist">

*   `NONE`, No logging (**DEFAULT**).

*   `BASIC`, Log only the request method and URL and the response status code and execution time.

*   `HEADERS`, Log the basic information along with request and response headers.

*   `FULL`, Log the headers, body, and metadata for both requests and responses.

</div>

<div class="paragraph">

For example, the following would set the `Logger.Level` to `FULL`:

</div>

<div class="listingblock">

<div class="content">

    @Configuration
    public class FooConfiguration {
        @Bean
        Logger.Level feignLoggerLevel() {
            return Logger.Level.FULL;
        }
    }

</div>

</div>

</div>

</div>

</div>

<div class="sect1">

## External Configuration: Archaius

<div class="sectionbody">

<div class="paragraph">

[Archaius](https://github.com/Netflix/archaius) is the Netflix client side configuration library. It is the library used by all of the Netflix OSS components for configuration. Archaius is an extension of the [Apache Commons Configuration](https://commons.apache.org/proper/commons-configuration) project. It allows updates to configuration by either polling a source for changes or for a source to push changes to the client. Archaius uses Dynamic<Type>Property classes as handles to properties.

</div>

<div class="listingblock">

<div class="title">Archaius Example</div>

<div class="content">

    class ArchaiusTest {
        DynamicStringProperty myprop = DynamicPropertyFactory
                .getInstance()
                .getStringProperty("my.prop");

        void doSomething() {
            OtherClass.someMethod(myprop.get());
        }
    }

</div>

</div>

<div class="paragraph">

Archaius has its own set of configuration files and loading priorities. Spring applications should generally not use Archaius directly, but the need to configure the Netflix tools natively remains. Spring Cloud has a Spring Environment Bridge so Archaius can read properties from the Spring Environment. This allows Spring Boot projects to use the normal configuration toolchain, while allowing them to configure the Netflix tools, for the most part, as documented.

</div>

</div>

</div>

<div class="sect1">

## Router and Filter: Zuul

<div class="sectionbody">

<div class="paragraph">

Routing in an integral part of a microservice architecture. For example, `/` may be mapped to your web application, `/api/users` is mapped to the user service and `/api/shop` is mapped to the shop service. [Zuul](https://github.com/Netflix/zuul) is a JVM based router and server side load balancer by Netflix.

</div>

<div class="paragraph">

[Netflix uses Zuul](http://www.slideshare.net/MikeyCohen1/edge-architecture-ieee-international-conference-on-cloud-engineering-32240146/27) for the following:

</div>

<div class="ulist">

*   Authentication

*   Insights

*   Stress Testing

*   Canary Testing

*   Dynamic Routing

*   Service Migration

*   Load Shedding

*   Security

*   Static Response handling

*   Active/Active traffic management

</div>

<div class="paragraph">

Zuul’s rule engine allows rules and filters to be written in essentially any JVM language, with built in support for Java and Groovy.

</div>

<div class="sect2">

### Embedded Zuul Reverse Proxy

<div class="paragraph">

Spring Cloud has created an embedded Zuul proxy to ease the development of a very common use case where a UI application wants to proxy calls to one or more back end services. This feature is useful for a user interface to proxy to the backend services it requires, avoiding the need to manage CORS and authentication concerns independently for all the backends.

</div>

<div class="paragraph">

To enable it, annotate a Spring Boot main class with `@EnableZuulProxy`, and this forwards local calls to the appropriate service. By convention, a service with the Eureka ID "users", will receive requests from the proxy located at `/users` (with the prefix stripped). The proxy uses Ribbon to locate an instance to forward to via Eureka, and all requests are executed in a hystrix command, so failures will show up in Hystrix metrics, and once the circuit is open the proxy will not try to contact the service.

</div>

<div class="paragraph">

To skip having a service automatically added, set `zuul.ignored-services` to a list of service id patterns. If a service matches a pattern that is ignored, but also included in the explicitly configured routes map, then it will be unignored. Example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      ignoredServices: '*'
      routes:
        users: /myusers/**

</div>

</div>

<div class="paragraph">

In this example, all services are ignored **except** "users".

</div>

<div class="paragraph">

To augment or change the proxy routes, you can add external configuration like the following:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      routes:
        users: /myusers/**

</div>

</div>

<div class="paragraph">

This means that http calls to "/myusers" get forwarded to the "users" service (for example "/myusers/101" is forwarded to "/101").

</div>

<div class="paragraph">

To get more fine-grained control over a route you can specify the path and the serviceId independently:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      routes:
        users:
          path: /myusers/**
          serviceId: users_service

</div>

</div>

<div class="paragraph">

This means that http calls to "/myusers" get forwarded to the "users_service" service. The route has to have a "path" which can be specified as an ant-style pattern, so "/myusers/*" only matches one level, but "/myusers/{asterisk}{asterisk}" matches hierarchically.

</div>

<div class="paragraph">

The location of the backend can be specified as either a "serviceId" (for a Eureka service) or a "url" (for a physical location), e.g.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      routes:
        users:
          path: /myusers/**
          url: http://example.com/users_service

</div>

</div>

<div class="paragraph">

These simple url-routes doesn’t get executed as HystrixCommand nor can you loadbalance multiple url with Ribbon. To achieve this specify a service-route and configure a Ribbon client for the serviceId (this currently requires disabling Eureka support in Ribbon: see [above for more information](http://projects.spring.io/spring-cloud/spring-cloud.html#spring-cloud-ribbon-without-eureka)), e.g.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

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

</div>

</div>

<div class="paragraph">

You can provide convention between serviceId and routes using regexmapper. It uses regular expression named group to extract variables from serviceId and inject them into a route pattern.

</div>

<div class="listingblock">

<div class="title">ApplicationConfiguration.java</div>

<div class="content">

    @Bean
    public PatternServiceRouteMapper serviceRouteMapper() {
        return new PatternServiceRouteMapper(
            "(?<name>^.+)-(?<version>v.+$)",
            "${version}/${name}");
    }

</div>

</div>

<div class="paragraph">

This means that a serviceId "myusers-v1" will be mapped to route "/v1/myusers/{asterisk}{asterisk}". Any regular expression is accepted but all named group must be present in both servicePattern and routePattern. If servicePattern do not match a serviceId, the default behavior is used. In exemple above, a serviceId "myusers" will be mapped to route "/myusers/{asterisk}{asterisk}" (no version detected) These feature is disable by default and is only applied to discovered services.

</div>

<div class="paragraph">

To add a prefix to all mappings, set `zuul.prefix` to a value, such as `/api`. The proxy prefix is stripped from the request before the request is forwarded by default (switch this behaviour off with `zuul.stripPrefix=false`). You can also switch off the stripping of the service-specific prefix from individual routes, e.g.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      routes:
        users:
          path: /myusers/**
          stripPrefix: false

</div>

</div>

<div class="paragraph">

In this example requests to "/myusers/101" will be forwarded to "/myusers/101" on the "users" service.

</div>

<div class="paragraph">

The `zuul.routes` entries actually bind to an object of type `ProxyRouteLocator`. If you look at the properties of that object you will see that it also has a "retryable" flag. Set that flag to "true" to have the Ribbon client automatically retry failed requests (and if you need to you can modify the parameters of the retry operations using the Ribbon client configuration).

</div>

<div class="paragraph">

The `X-Forwarded-Host` header is added to the forwarded requests by default. To turn it off set `zuul.addProxyHeaders = false`. The prefix path is stripped by default, and the request to the backend picks up a header "X-Forwarded-Prefix" ("/myusers" in the examples above).

</div>

<div class="paragraph">

An application with the `@EnableZuulProxy` could act as a standalone server if you set a default route ("/"), for example `zuul.route.home: /` would route all traffic (i.e. "/{asterisk}{asterisk}") to the "home" service.

</div>

<div class="paragraph">

If more fine-grained ignoring is needed, you can specify specific patterns to ignore. These patterns are being evaluated at the start of the route location process, which means prefixes should be included in the pattern to warrant a match. Ignored patterns span all services and supersede any other route specification.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      ignoredPatterns: /**/admin/**
      routes:
        users: /myusers/**

</div>

</div>

<div class="paragraph">

This means that all calls such as "/myusers/101" will be forwarded to "/101" on the "users" service. But calls including "/admin/" will not resolve.

</div>

</div>

<div class="sect2">

### Strangulation Patterns and Local Forwards

<div class="paragraph">

A common pattern when migrating an existing application or API is to "strangle" old endpoints, slowly replacing them with different implementations. The Zuul proxy is a useful tool for this because you can use it to handle all traffic from clients of the old endpoints, but redirect some of the requests to new ones.

</div>

<div class="paragraph">

Example configuration:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

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

</div>

</div>

<div class="paragraph">

In this example we are strangling the "legacy" app which is mapped to all requests that do not match one of the other patterns. Paths in `/first/{asterisk}{asterisk}` have been extracted into a new service with an external URL. And paths in `/second/{asterisk}{asterisk}` are forwared so they can be handled locally, e.g. with a normal Spring `@RequestMapping`. Paths in `/third/{asterisk}{asterisk}` are also forwarded, but with a different prefix (i.e. `/third/foo` is forwarded to `/3rd/foo`).

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">The ignored pattterns aren’t completely ignored, they just aren’t handled by the proxy (so they are also effectively forwarded locally).</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Uploading Files through Zuul

<div class="paragraph">

If you `@EnableZuulProxy` you can use the proxy paths to upload files and it should just work as long as the files are small. For large files there is an alternative path which bypasses the Spring `DispatcherServlet` (to avoid multipart processing) in "/zuul/*". I.e. if `zuul.routes.customers=/customers/{asterisk}{asterisk}` then you can POST large files to "/zuul/customers/*". The servlet path is externalized via `zuul.servletPath`. Extremely large files will also require elevated timeout settings if the proxy route takes you through a Ribbon load balancer, e.g.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

    hystrix.command.default.execution.isolation.thread.timeoutInMilliseconds: 60000
    ribbon:
      ConnectTimeout: 3000
      ReadTimeout: 60000

</div>

</div>

<div class="paragraph">

Note that for streaming to work with large files, you need to use chunked encoding in the request (which some browsers do not do by default). E.g. on the command line:

</div>

<div class="listingblock">

<div class="content">

<pre>$ curl -v -H "Transfer-Encoding: chunked" \
    -F "file=@mylarge.iso" localhost:9999/zuul/simple/file</pre>

</div>

</div>

</div>

<div class="sect2">

### Plain Embedded Zuul

<div class="paragraph">

You can also run a Zuul server without the proxying, or switch on parts of the proxying platform selectively, if you use `@EnableZuulServer` (instead of `@EnableZuulProxy`). Any beans that you add to the application of type `ZuulFilter` will be installed automatically, as they are with `@EnableZuulProxy`, but without any of the proxy filters being added automatically.

</div>

<div class="paragraph">

In this case the routes into the Zuul server are still specified by configuring "zuul.routes.*", but there is no service discovery and no proxying, so the "serviceId" and "url" settings are ignored. For example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

     zuul:
      routes:
        api: /api/**

</div>

</div>

<div class="paragraph">

maps all paths in "/api/{asterisk}{asterisk}" to the Zuul filter chain.

</div>

</div>

<div class="sect2">

### Disable Zuul Filters

<div class="paragraph">

Zuul for Spring Cloud comes with a number of `ZuulFilter` beans enabled by default in both proxy and server mode. See [the zuul filters package](https://github.com/spring-cloud/spring-cloud-netflix/tree/master/spring-cloud-netflix-core/src/main/java/org/springframework/cloud/netflix/zuul/filters) for the possible filters that are enabled. If you want to disable one, simply set `zuul.<SimpleClassName>.<filterType>.disable=true`. By convention, the package after `filters` is the Zuul filter type. For example to disable `org.springframework.cloud.netflix.zuul.filters.post.SendResponseFilter` set `zuul.SendResponseFilter.post.disable=true`.

</div>

</div>

<div class="sect2">

### Polyglot support with Sidecar

<div class="paragraph">

Do you have non-jvm languages you want to take advantage of Eureka, Ribbon and Config Server? The Spring Cloud Netflix Sidecar was inspired by [Netflix Prana](https://github.com/Netflix/Prana). It includes a simple http api to get all of the instances (ie host and port) for a given service. You can also proxy service calls through an embedded Zuul proxy which gets its route entries from Eureka. The Spring Cloud Config Server can be accessed directly via host lookup or through the Zuul Proxy. The non-jvm app should implement a health check so the Sidecar can report to eureka if the app is up or down.

</div>

<div class="paragraph">

To enable the Sidecar, create a Spring Boot application with `@EnableSidecar`. This annotation includes `@EnableCircuitBreaker`, `@EnableDiscoveryClient`, and `@EnableZuulProxy`. Run the resulting application on the same host as the non-jvm application.

</div>

<div class="paragraph">

To configure the side car add `sidecar.port` and `sidecar.health-uri` to `application.yml`. The `sidecar.port` property is the port the non-jvm app is listening on. This is so the Sidecar can properly register the app with Eureka. The `sidecar.health-uri` is a uri accessible on the non-jvm app that mimicks a Spring Boot health indicator. It should return a json document like the following:

</div>

<div class="listingblock">

<div class="title">health-uri-document</div>

<div class="content">

    {
      "status":"UP"
    }

</div>

</div>

<div class="paragraph">

Here is an example application.yml for a Sidecar application:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

    server:
      port: 5678
    spring:
      application:
        name: sidecar

    sidecar:
      port: 8000
      health-uri: http://localhost:8000/health.json

</div>

</div>

<div class="paragraph">

The api for the `DiscoveryClient.getInstances()` method is `/hosts/{serviceId}`. Here is an example response for `/hosts/customers` that returns two instances on different hosts. This api is accessible to the non-jvm app (if the sidecar is on port 5678) at `[http://localhost:5678/hosts/{serviceId}](http://localhost:5678/hosts/%7BserviceId%7D)`.

</div>

<div class="listingblock">

<div class="title">/hosts/customers</div>

<div class="content">

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

</div>

</div>

<div class="paragraph">

The Zuul proxy automatically adds routes for each service known in eureka to `/<serviceId>`, so the customers service is available at `/customers`. The Non-jvm app can access the customer service via `[http://localhost:5678/customers](http://localhost:5678/customers)` (assuming the sidecar is listening on port 5678).

</div>

<div class="paragraph">

If the Config Server is registered with Eureka, non-jvm application can access it via the Zuul proxy. If the serviceId of the ConfigServer is `configserver` and the Sidecar is on port 5678, then it can be accessed at [http://localhost:5678/configserver](http://localhost:5678/configserver)

</div>

<div class="paragraph">

Non-jvm app can take advantage of the Config Server’s ability to return YAML documents. For example, a call to [http://sidecar.local.spring.io:5678/configserver/default-master.yml](http://sidecar.local.spring.io:5678/configserver/default-master.yml) might result in a YAML document like the following

</div>

<div class="listingblock">

<div class="content">

    eureka:
      client:
        serviceUrl:
          defaultZone: http://localhost:8761/eureka/
      password: password
    info:
      description: Spring Cloud Samples
      url: https://github.com/spring-cloud-samples

</div>

</div>

</div>

</div>

</div>

<div class="sect1">

## Metrics: Spectator, Servo, and Atlas

<div class="sectionbody">

<div class="paragraph">

When used together, Spectator/Servo and Atlas provide a near real-time operational insight platform.

</div>

<div class="paragraph">

Spectator and Servo are Netflix’s metrics collection libraries. Atlas is a Netflix metrics backend to manage dimensional time series data.

</div>

<div class="paragraph">

Servo served Netflix for several years and is still usable, but is gradually being phased out in favor of Spectator, which is only designed to work with Java 8\. Spring Cloud Netflix provides support for both, but Java 8 based applications are encouraged to use Spectator.

</div>

<div class="sect2">

### Dimensional vs. Hierarchical Metrics

<div class="paragraph">

Spring Boot Actuator metrics are hierarchical and metrics are separated only by name. These names often follow a naming convention that embeds key/value attribute pairs (dimensions) into the name separated by periods. Consider the following metrics for two endpoints, root and star-star:

</div>

<div class="listingblock">

<div class="content">

    {
        "counter.status.200.root": 20,
        "counter.status.400.root": 3,
        "counter.status.200.star-star": 5,
    }

</div>

</div>

<div class="paragraph">

The first metric gives us a normalized count of successful requests against the root endpoint per unit of time. But what if the system had 20 endpoints and you want to get a count of successful requests against all the endpoints? Some hierarchical metrics backends would allow you to specify a wild card such as `counter.status.200.` **that would read all 20 metrics and aggregate the results. Alternatively, you could provide a `HandlerInterceptorAdapter` that intercepts and records a metric like `counter.status.200.all` for all successful requests irrespective of the endpoint, but now you must write 20+1 different metrics. Similarly if you want to know the total number of successful requests for all endpoints in the service, you could specify a wild card such as `counter.status.2`**`.*`.

</div>

<div class="paragraph">

Even in the presence of wildcarding support on a hierarchical metrics backend, naming consistency can be difficult. Specifically the position of these tags in the name string can slip with time, breaking queries. For example, suppose we add an additional dimension to the hierarchical metrics above for HTTP method. Then `counter.status.200.root` becomes `counter.status.200.method.get.root`, etc. Our `counter.status.200.*` suddenly no longer has the same semantic meaning. Furthermore, if the new dimension is not applied uniformly across the codebase, certain queries may become impossible. This can quickly get out of hand.

</div>

<div class="paragraph">

Netflix metrics are tagged (a.k.a. dimensional). Each metric has a name, but this single named metric can contain multiple statistics and 'tag' key/value pairs that allows more querying flexibility. In fact, the statistics themselves are recorded in a special tag.

</div>

<div class="paragraph">

Recorded with Netflix Servo or Spectator, a timer for the root endpoint described above contains 4 statistics per status code, where the count statistic is identical to Spring Boot Actuator’s counter. In the event that we have encountered an HTTP 200 and 400 thus far, there will be 8 available data points:

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

</div>

<div class="sect2">

### Default Metrics Collection

<div class="paragraph">

Without any additional dependencies or configuration, a Spring Cloud based service will autoconfigure a Servo `MonitorRegistry` and begin collecting metrics on every Spring MVC request. By default, a Servo timer with the name `rest` will be recorded for each MVC request which is tagged with:

</div>

<div class="olist arabic">

1.  HTTP method

2.  HTTP status (e.g. 200, 400, 500)

3.  URI (or "root" if the URI is empty), sanitized for Atlas

4.  The exception class name, if the request handler threw an exception

5.  The caller, if a request header with a key matching `netflix.metrics.rest.callerHeader` is set on the request. There is no default key for `netflix.metrics.rest.callerHeader`. You must add it to your application properties if you wish to collect caller information.

</div>

<div class="paragraph">

Set the `netflix.metrics.rest.metricName` property to change the name of the metric from `rest` to a name you provide.

</div>

<div class="paragraph">

If Spring AOP is enabled and `org.aspectj:aspectjweaver` is present on your runtime classpath, Spring Cloud will also collect metrics on every client call made with `RestTemplate`. A Servo timer with the name of `restclient` will be recorded for each MVC request which is tagged with:

</div>

<div class="olist arabic">

1.  HTTP method

2.  HTTP status (e.g. 200, 400, 500), "CLIENT_ERROR" if the response returned null, or "IO_ERROR" if an `IOException` occurred during the execution of the `RestTemplate` method

3.  URI, sanitized for Atlas

4.  Client name

</div>

</div>

<div class="sect2">

### Metrics Collection: Spectator

<div class="paragraph">

To enable Spectator metrics, include a dependency on `spring-boot-starter-spectator`:

</div>

<div class="listingblock">

<div class="content">

        <dependency>
            <groupId>org.springframework.cloud</groupId>
            <artifactId>spring-cloud-starter-spectator</artifactId>
        </dependency>

</div>

</div>

<div class="paragraph">

In Spectator parlance, a meter is a named, typed, and tagged configuration and a metric represents the value of a given meter at a point in time. Spectator meters are created and controlled by a registry, which currently has several different implementations. Spectator provides 4 meter types: counter, timer, gauge, and distribution summary.

</div>

<div class="paragraph">

Spring Cloud Spectator integration configures an injectable `com.netflix.spectator.api.Registry` instance for you. Specifically, it configures a `ServoRegistry` instance in order to unify the collection of REST metrics and the exporting of metrics to the Atlas backend under a single Servo API. Practically, this means that your code may use a mixture of Servo monitors and Spectator meters and both will be scooped up by Spring Boot Actuator `MetricReader` instances and both will be shipped to the Atlas backend.

</div>

<div class="sect3">

#### Spectator Counter

<div class="paragraph">

A counter is used to measure the rate at which some event is occurring.

</div>

<div class="listingblock">

<div class="content">

    // create a counter with a name and a set of tags
    Counter counter = registry.counter("counterName", "tagKey1", "tagValue1", ...);
    counter.increment(); // increment when an event occurs
    counter.increment(10); // increment by a discrete amount

</div>

</div>

<div class="paragraph">

The counter records a single time-normalized statistic.

</div>

</div>

<div class="sect3">

#### Spectator Timer

<div class="paragraph">

A timer is used to measure how long some event is taking. Spring Cloud automatically records timers for Spring MVC requests and conditionally `RestTemplate` requests, which can later be used to create dashboards for request related metrics like latency:

</div>

<div class="paragraph">

<div class="title">Request Latency</div>

image::RequestLatency.png []

</div>

<div class="listingblock">

<div class="content">

    // create a timer with a name and a set of tags
    Timer timer = registry.timer("timerName", "tagKey1", "tagValue1", ...);

    // execute an operation and time it at the same time
    T result = timer.record(() -> fooReturnsT());

    // alternatively, if you must manually record the time
    Long start = System.nanoTime();
    T result = fooReturnsT();
    timer.record(System.nanoTime() - start, TimeUnit.NANOSECONDS);

</div>

</div>

<div class="paragraph">

The timer simultaneously records 4 statistics: count, max, totalOfSquares, and totalTime. The count statistic will always match the single normalized value provided by a counter if you had called `increment()` once on the counter for each time you recorded a timing, so it is rarely necessary to count and time separately for a single operation.

</div>

<div class="paragraph">

For [long running operations](https://github.com/Netflix/spectator/wiki/Timer-Usage#longtasktimer), Spectator provides a special `LongTaskTimer`.

</div>

</div>

<div class="sect3">

#### Spectator Gauge

<div class="paragraph">

Gauges are used to determine some current value like the size of a queue or number of threads in a running state. Since gauges are sampled, they provide no information about how these values fluctuate between samples.

</div>

<div class="paragraph">

The normal use of a gauge involves registering the gauge once in initialization with an id, a reference to the object to be sampled, and a function to get or compute a numeric value based on the object. The reference to the object is passed in separately and the Spectator registry will keep a weak reference to the object. If the object is garbage collected, then Spectator will automatically drop the registration. See [the note](https://github.com/Netflix/spectator/wiki/Gauge-Usage#using-lambda) in Spectator’s documentation about potential memory leaks if this API is misused.

</div>

<div class="listingblock">

<div class="content">

    // the registry will automatically sample this gauge periodically
    registry.gauge("gaugeName", pool, Pool::numberOfRunningThreads);

    // manually sample a value in code at periodic intervals -- last resort!
    registry.gauge("gaugeName", Arrays.asList("tagKey1", "tagValue1", ...), 1000);

</div>

</div>

</div>

<div class="sect3">

#### Spectator Distribution Summaries

<div class="paragraph">

A distribution summary is used to track the distribution of events. It is similar to a timer, but more general in that the size does not have to be a period of time. For example, a distribution summary could be used to measure the payload sizes of requests hitting a server.

</div>

<div class="listingblock">

<div class="content">

    // the registry will automatically sample this gauge periodically
    DistributionSummary ds = registry.distributionSummary("dsName", "tagKey1", "tagValue1", ...);
    ds.record(request.sizeInBytes());

</div>

</div>

</div>

</div>

<div class="sect2">

### Metrics Collection: Servo

<div class="admonitionblock warning">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Warning</div>

</td>

<td class="content">If your code is compiled on Java 8, please use Spectator instead of Servo as Spectator is destined to replace Servo entirely in the long term.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

In Servo parlance, a monitor is a named, typed, and tagged configuration and a metric represents the value of a given monitor at a point in time. Servo monitors are logically equivalent to Spectator meters. Servo monitors are created and controlled by a `MonitorRegistry`. In spite of the above warning, Servo does have a [wider array](https://github.com/Netflix/servo/wiki/Getting-Started) of monitor options than Spectator has meters.

</div>

<div class="paragraph">

Spring Cloud integration configures an injectable `com.netflix.servo.MonitorRegistry` instance for you. Once you have created the appropriate `Monitor` type in Servo, the process of recording data is wholly similar to Spectator.

</div>

<div class="sect3">

#### Creating Servo Monitors

<div class="paragraph">

If you are using the Servo `MonitorRegistry` instance provided by Spring Cloud (specifically, an instance of `DefaultMonitorRegistry`), Servo provides convenience classes for retrieving [counters](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamiccounter) and [timers](https://github.com/Netflix/spectator/wiki/Servo-Comparison#dynamictimer). These convenience classes ensure that only one `Monitor` is registered for each unique combination of name and tags.

</div>

<div class="paragraph">

To manually create a Monitor type in Servo, especially for the more exotic monitor types for which convenience methods are not provided, instantiate the appropriate type by providing a `MonitorConfig` instance:

</div>

<div class="listingblock">

<div class="content">

    MonitorConfig config = MonitorConfig.builder("timerName").withTag("tagKey1", "tagValue1").build();

    // somewhere we should cache this Monitor by MonitorConfig
    Timer timer = new BasicTimer(config);
    monitorRegistry.register(timer);

</div>

</div>

</div>

</div>

<div class="sect2">

### Metrics Backend: Atlas

<div class="paragraph">

Atlas was developed by Netflix to manage dimensional time series data for near real-time operational insight. Atlas features in-memory data storage, allowing it to gather and report very large numbers of metrics, very quickly.

</div>

<div class="paragraph">

Atlas captures operational intelligence. Whereas business intelligence is data gathered for analyzing trends over time, operational intelligence provides a picture of what is currently happening within a system.

</div>

<div class="paragraph">

Spring Cloud provides a `spring-cloud-starter-atlas` that has all the dependencies you need. Then just annotate your Spring Boot application with `@EnableAtlas` and provide a location for your running Atlas server with the `netflix.atlas.uri` property.

</div>

<div class="sect3">

#### Global tags

<div class="paragraph">

Spring Cloud enables you to add tags to every metric sent to the Atlas backend. Global tags can be used to separate metrics by application name, environment, region, etc.

</div>

<div class="paragraph">

Each bean implementing `AtlasTagProvider` will contribute to the global tag list:

</div>

<div class="listingblock">

<div class="content">

    @Bean
    AtlasTagProvider atlasCommonTags(
        @Value("${spring.application.name}") String appName) {
      return () -> Collections.singletonMap("app", appName);
    }

</div>

</div>

</div>

<div class="sect3">

#### Using Atlas

<div class="paragraph">

To bootstrap a in-memory standalone Atlas instance:

</div>

<div class="listingblock">

<div class="content">

    $ curl -LO https://github.com/Netflix/atlas/releases/download/v1.4.2/atlas-1.4.2-standalone.jar
    $ java -jar atlas-1.4.2-standalone.jar

</div>

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">An Atlas standalone node running on an r3.2xlarge (61GB RAM) can handle roughly 2 million metrics per minute for a given 6 hour window.</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

Once running and you have collected a handful of metrics, verify that your setup is correct by listing tags on the Atlas server:

</div>

<div class="listingblock">

<div class="content">

    $ curl http://ATLAS/api/v1/tags

</div>

</div>

<div class="admonitionblock tip">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Tip</div>

</td>

<td class="content">After executing several requests against your service, you can gather some very basic information on the request latency of every request by pasting the following url in your browser: `[http://ATLAS/api/v1/graph?q=name,rest,:eq,:avg](http://atlas/api/v1/graph?q=name,rest,:eq,:avg)`</td>

</tr>

</tbody>

</table>

</div>

<div class="paragraph">

The Atlas wiki contains a [compilation of sample queries](https://github.com/Netflix/atlas/wiki/Single-Line) for various scenarios.

</div>

<div class="paragraph">

Make sure to check out the [alerting philosophy](https://github.com/Netflix/atlas/wiki/Alerting-Philosophy) and docs on using [double exponential smoothing](https://github.com/Netflix/atlas/wiki/DES) to generate dynamic alert thresholds.

</div>

</div>

</div>

</div>

</div>

# Spring Cloud Bus

<div class="openblock partintro">

<div class="content">

<div class="paragraph">

Spring Cloud Bus links nodes of a distributed system with a lightweight message broker. This can then be used to broadcast state changes (e.g. configuration changes) or other management instructions. A key idea is that the Bus is like a distributed Actuator for a Spring Boot application that is scaled out, but it can also be used as a communication channel between apps. The only implementation currently is with an AMQP broker as the transport, but the same basic feature set (and some more depending on the transport) is on the roadmap for other transports.

</div>

<div class="paragraph">

[https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc](https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc)

</div>

</div>

</div>

<div class="sect1">

## Quick Start

<div class="sectionbody">

<div class="paragraph">

Spring Cloud Bus works by adding Spring Boot autconfiguration if it detects itself on the classpath. All you need to do to enable the bus is to add `spring-cloud-starter-bus-amqp` to your dependency management and Spring Cloud takes care of the rest. Make sure RabbitMQ is available and configured to provide a `ConnectionFactory`: running on localhost you shouldn’t have to do anything, but if you are running remotely use Spring Cloud Connectors, or Spring Boot conventions to define the broker credentials, e.g.

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

<pre>spring:
  rabbitmq:
    host: mybroker.com
    port: 5672
    username: user
    password: secret</pre>

</div>

</div>

<div class="paragraph">

The bus currently supports sending messages to all nodes listening or all nodes for a particular service (as defined by Eureka). More selector criteria will be added in the future (ie. only service X nodes in data center Y, etc…​). The http endpoints are under the `/bus/*` actuator namespace. There are currently two implemented. The first, `/bus/env`, sends key/values pairs to update each nodes Spring Environment. The second, `/bus/refresh`, will reload each application’s configuration, just as if they had all been pinged on their `/refresh` endpoint.

</div>

</div>

</div>

<div class="sect1">

## Addressing an Instance

<div class="sectionbody">

<div class="paragraph">

The HTTP endpoints accept a "destination" parameter, e.g. "/bus/refresh?destination=customers:9000", where the destination is an `ApplicationContext` ID. If the ID is owned by an instance on the Bus then it will process the message and all other instances will ignore it. Spring Boot sets the ID for you in the `ContextIdApplicationContextInitializer` to a combination of the `spring.application.name`, active profiles and `server.port` by default.

</div>

</div>

</div>

<div class="sect1">

## Addressing all instances of a service

<div class="sectionbody">

<div class="paragraph">

The "destination" parameter is used in a Spring `PathMatcher` (with the path separator as a colon `:`) to determine if an instance will process the message. Using the example from above, "/bus/refresh?destination=customers:**" will target all instances of the "customers" service regardless of the profiles and ports set as the `ApplicationContext` ID.

</div>

</div>

</div>

<div class="sect1">

## Application Context ID must be unique

<div class="sectionbody">

<div class="paragraph">

The bus tries to eliminate processing an event twice, once from the original `ApplicationEvent` and once from the queue. To do this, it checks the sending application context id againts the current application context id. If multiple instances of a service have the same application context id, events will not be processed. Running on a local machine, each service will be on a different port and that will be part of the application context id. Cloud Foundry supplies an index to differentiate. To ensure that the application context id is the unique, set `spring.application.index` to something unique for each instance of a service. For example, in lattice, set `spring.application.index=${INSTANCE_INDEX}` in application.properties (or bootstrap.properties if using configserver).

</div>

</div>

</div>

<div class="sect1">

## Customizing the Message Broker

<div class="sectionbody">

<div class="paragraph">

Spring Cloud Bus uses [Spring Cloud Stream](https://cloud.spring.io/spring-cloud-stream) to broadcast the messages so to get messages to flow you only need to include the binder implementation of your choice in the classpath. There are convenient starters specifically for the bus with AMQP, Kafka and Redis (`spring-cloud-starter-bus-[amqp,kafka,redis]`). Generally speaking Spring Cloud Stream relies on Spring Boot autoconfiguration conventions for configuring middleware, so for instance the AMQP broker address can be changed with `spring.rabbitmq.*` configuration properties. Spring Cloud Bus has a handful of native configuration properties in `spring.cloud.bus.*` (e.g. `spring.cloud.bus.destination` is the name of the topic to use the the externall middleware). Normally the defaults will suffice.

</div>

<div class="paragraph">

To lean more about how to customize the message broker settings consult the Spring Cloud Stream documentation.

</div>

</div>

</div>

<div class="sect1">

## Tracing Bus Events

<div class="sectionbody">

<div class="paragraph">

Bus events (subclasses of `RemoteApplicationEvent`) can be traced by setting `spring.cloud.bus.trace.enabled=true`. If you do this then the Spring Boot `TraceRepository` (if it is present) will show each event sent and all the acks from each service instance. Example (from the `/trace` endpoint):

</div>

<div class="listingblock">

<div class="content">

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

</div>

</div>

<div class="paragraph">

This trace shows that a `RefreshRemoteApplicationEvent` was sent from `customers:9000`, broadcast to all services, and it was received (acked) by `customers:9000` and `stores:8081`.

</div>

<div class="paragraph">

To handle the ack signals yourself you could add an `@EventListener` for the `AckRemoteAppplicationEvent` and `SentApplicationEvent` types to your app (and enable tracing). Or you could tap into the `TraceRepository` and mine the data from there.

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">Any Bus application can trace acks, but sometimes it will be useful to do this in a central service that can do more complex queries on the data. Or forward it to a specialized tracing service.</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

# Spring Boot Cloud CLI

<div class="openblock partintro">

<div class="content">

<div class="paragraph">

Spring Boot CLI provides [Spring Boot](http://projects.spring.io/spring-boot) command line features for [Spring Cloud](https://github.com/spring-cloud). You can write Groovy scripts to run Spring Cloud component applications (e.g. `@EnableEurekaServer`). You can also easily do things like encryption and decryption to support Spring Cloud Config clients with secret configuration values.

</div>

<div class="paragraph">

[https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc](https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc)

</div>

</div>

</div>

<div class="sect1">

## Installation

<div class="sectionbody">

<div class="paragraph">

To install, make sure you have [Spring Boot CLI](https://github.com/spring-projects/spring-boot) (1.2.0 or better):

</div>

<div class="literalblock">

<div class="content">

<pre>$ spring version
Spring CLI v1.2.3.RELEASE</pre>

</div>

</div>

<div class="paragraph">

E.g. for GVM users

</div>

<div class="listingblock">

<div class="content">

    $ gvm install springboot 1.3.0.M5
    $ gvm use springboot 1.3.0.M5

</div>

</div>

<div class="paragraph">

and install the Spring Cloud plugin:

</div>

<div class="listingblock">

<div class="content">

    $ mvn install
    $ spring install org.springframework.cloud:spring-cloud-cli:1.1.0.BUILD-SNAPSHOT

</div>

</div>

<div class="admonitionblock important">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Important</div>

</td>

<td class="content">**Prerequisites:** to use the encryption and decryption features you need the full-strength JCE installed in your JVM (it’s not there by default). You can download the "Java Cryptography Extension (JCE) Unlimited Strength Jurisdiction Policy Files" from Oracle, and follow instructions for installation (essentially replace the 2 policy files in the JRE lib/security directory with the ones that you downloaded).</td>

</tr>

</tbody>

</table>

</div>

</div>

</div>

<div class="sect1">

## Writing Groovy Scripts and Running Applications

<div class="sectionbody">

<div class="paragraph">

Spring Cloud CLI has support for most of the Spring Cloud declarative features, such as the `@Enable*` class of annotations. For example, here is a fully functional Eureka server

</div>

<div class="listingblock">

<div class="title">app.groovy</div>

<div class="content">

    @EnableEurekaServer
    class Eureka {}

</div>

</div>

<div class="paragraph">

which you can run from the command line like this

</div>

<div class="listingblock">

<div class="content">

<pre>$ spring run app.groovy</pre>

</div>

</div>

<div class="paragraph">

To include additional dependencies, often it suffices just to add the appropriate feature-enabling annotation, e.g. `@EnableConfigServer`, `@EnableOAuth2Sso` or `@EnableEurekaClient`. To manually include a dependency you can use a `@Grab` with the special "Spring Boot" short style artifact co-ordinates, i.e. with just the artifact ID (no need for group or version information), e.g. to set up a client app to listen on AMQP for management events from the Spring CLoud Bus:

</div>

<div class="listingblock">

<div class="title">app.groovy</div>

<div class="content">

    @Grab('spring-cloud-starter-bus-amqp')
    @RestController
    class Service {
      @RequestMapping('/')
      def home() { [message: 'Hello'] }
    }

</div>

</div>

</div>

</div>

<div class="sect1">

## Encryption and Decryption

<div class="sectionbody">

<div class="paragraph">

The Spring Cloud CLI comes with an "encrypt" and a "decrypt" command. Both accept arguments in the same form with a key specified as a mandatory "--key", e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>$ spring encrypt mysecret --key foo
682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
$ spring decrypt --key foo 682bc583f4641835fa2db009355293665d2647dade3375c0ee201de2a49f7bda
mysecret</pre>

</div>

</div>

<div class="paragraph">

To use a key in a file (e.g. an RSA public key for encyption) prepend the key value with "@" and provide the file path, e.g.

</div>

<div class="listingblock">

<div class="content">

<pre>$ spring encrypt mysecret --key @${HOME}/.ssh/id_rsa.pub
AQAjPgt3eFZQXwt8tsHAVv/QHiY5sI2dRcR+...</pre>

</div>

</div>

</div>

</div>

# Spring Cloud Security

<div class="openblock partintro">

<div class="content">

<div class="paragraph">

Spring Cloud Security offers a set of primitives for building secure applications and services with minimum fuss. A declarative model which can be heavily configured externally (or centrally) lends itself to the implementation of large systems of co-operating, remote components, usually with a central indentity management service. It is also extremely easy to use in a service platform like Cloud Foundry. Building on Spring Boot and Spring Security OAuth2 we can quickly create systems that implement common patterns like single sign on, token relay and token exchange.

</div>

<div class="paragraph">

[https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc](https://raw.githubusercontent.com/spring-cloud/spring-cloud-build/master/docs/src/main/asciidoc/contributing-docs.adoc)

</div>

</div>

</div>

<div class="sect1">

## Quickstart

<div class="sectionbody">

<div class="sect2">

### OAuth2 Single Sign On

<div class="paragraph">

Here’s a Spring Cloud "Hello World" app with HTTP Basic authentication and a single user account:

</div>

<div class="listingblock">

<div class="title">app.groovy</div>

<div class="content">

    @Grab('spring-boot-starter-security')
    @Controller
    class Application {

      @RequestMapping('/')
      String home() {
        'Hello World'
      }

    }

</div>

</div>

<div class="paragraph">

You can run it with `spring run app.groovy` and watch the logs for the password (username is "user"). So far this is just the default for a Spring Boot app.

</div>

<div class="paragraph">

Here’s a Spring Cloud app with OAuth2 SSO:

</div>

<div class="listingblock">

<div class="title">app.groovy</div>

<div class="content">

    @Controller
    @EnableOAuth2Sso
    class Application {

      @RequestMapping('/')
      String home() {
        'Hello World'
      }

    }

</div>

</div>

<div class="paragraph">

Spot the difference? This app will actually behave exactly the same as the previous one, because it doesn’t know it’s OAuth2 credentals yet.

</div>

<div class="paragraph">

You can register an app in github quite easily, so try that if you want a production app on your own domain. If you are happy to test on localhost:8080, then set up these properties in your application configuration:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

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

</div>

</div>

<div class="paragraph">

run the app above and it will redirect to github for authorization. If you are already signed into github you won’t even notice that it has authenticated. These credentials will only work if your app is running on port 8080.

</div>

<div class="paragraph">

To limit the scope that the client asks for when it obtains an access token you can set `spring.oauth2.client.scope` (comma separated or an array in YAML). By default the scope is empty and it is up to to Authorization Server to decide what the defaults should be, usually depending on the settings in the client registration that it holds.

</div>

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">The examples above are all Groovy scripts. If you want to write the same code in Java (or Groovy) you need to add Spring Security OAuth2 to the classpath (e.g. see the [sample here](https://github.com/spring-cloud-samples/sso)).</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### OAuth2 Protected Resource

<div class="paragraph">

You want to protect an API resource with an OAuth2 token? Here’s a simple example (paired with the client above):

</div>

<div class="listingblock">

<div class="title">app.groovy</div>

<div class="content">

    @Grab('spring-cloud-starter-security')
    @RestController
    @EnableResourceServer
    class Application {

      @RequestMapping('/')
      def home() {
        [message: 'Hello World']
      }

    }

</div>

</div>

<div class="paragraph">

and

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

    spring:
      oauth2:
        resource:
          userInfoUri: https://api.github.com/user
          preferTokenInfo: false

</div>

</div>

</div>

</div>

</div>

<div class="sect1">

## More Detail

<div class="sectionbody">

<div class="sect2">

### Single Sign On

<div class="admonitionblock note">

<table>

<tbody>

<tr>

<td class="icon">

<div class="title">Note</div>

</td>

<td class="content">All of the OAuth2 SSO and resource server features moved to Spring Boot in version 1.3\. You can find documentation in the [Spring Boot user guide](http://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/).</td>

</tr>

</tbody>

</table>

</div>

</div>

<div class="sect2">

### Token Relay

<div class="paragraph">

A Token Relay is where an OAuth2 consumer acts as a Client and forwards the incoming token to outgoing resource requests. The consumer can be a pure Client (like an SSO application) or a Resource Server.

</div>

<div class="sect3">

#### Client Token Relay

<div class="paragraph">

If your app has a [Spring Cloud Zuul](http://cloud.spring.io/spring-cloud.html#netflix-zuul-reverse-proxy) embedded reverse proxy (using `@EnableZuulProxy`) then you can ask it to forward OAuth2 access tokens downstream to the services it is proxying. Thus the SSO app above can be enhanced simply like this:

</div>

<div class="listingblock">

<div class="title">app.groovy</div>

<div class="content">

    @Controller
    @EnableOAuth2Sso
    @EnableZuulProxy
    class Application {

    }

</div>

</div>

<div class="paragraph">

and it will (in addition to loggin the user in and grabbing a token) pass the authentication token downstream to the `/proxy/*` services. If those services are implemented with `@EnableOAuth2Resource` then they will get a valid token in the correct header.

</div>

<div class="paragraph">

How does it work? The `@EnableOAuth2Sso` annotation pulls in `spring-cloud-starter-security` (which you could do manually in a traditional app), and that in turn triggers some autoconfiguration for a `ZuulFilter`, which itself is activated because Zuul is on the classpath (via `@EnableZuulProxy`). The {github}/tree/master/src/main/java/org/springframework/cloud/security/oauth2/proxy/OAuth2TokenRelayFilter.java[filter] just extracts an access token from the currently authenticated user, and puts it in a request header for the downstream requests.

</div>

</div>

<div class="sect3">

#### Resource Server Token Relay

<div class="paragraph">

If your app has `@EnableOAuth2Resource` and also is a Client (i.e. it has a `spring.oauth2.client.clientId`, even if it doesn’t use it), then the `OAuth2RestOperations` that is provided for `@Autowired` users by Spring Cloud (it is declared as `@Primary`) will also forward tokens. If you don’t want to forward tokens (and that is a valid choice, since you might want to act as yourself, rather than the client that sent you the token), then you only need to create your own `OAuth2RestOperations` instead of autowiring the default one. Here’s a basic example showing the use of the autowired rest template ("foo.com" is a Resource Server accepting the same tokens as the surrounding app):

</div>

<div class="listingblock">

<div class="title">MyController.java</div>

<div class="content">

    @Autowired
    private OAuth2RestOperations restTemplate;

    @RequestMapping("/relay")
    public String relay() {
        ResponseEntity<String> response =
          restTemplate.getForEntity("https://foo.com/bar", String.class);
        return "Success! (" + response.getBody() + ")";
    }

</div>

</div>

</div>

</div>

</div>

</div>

<div class="sect1">

## Configuring Authentication Downstream of a Zuul Proxy

<div class="sectionbody">

<div class="paragraph">

You can control the authorization behaviour downstream of an `@EnableZuulProxy` through the `proxy.auth.*` settings. Example:

</div>

<div class="listingblock">

<div class="title">application.yml</div>

<div class="content">

    proxy:
      auth:
        routes:
          customers: oauth2
          stores: passthru
          recommendations: none

</div>

</div>

<div class="paragraph">

In this example the "customers" service gets an OAuth2 token relay, the "stores" service gets a passthrough (the authorization header is just passed downstream), and the "recommendations" service has its authorization header removed. The default behaviour is to do a token relay if there is a token available, and passthru otherwise.

</div>

<div class="paragraph">

See {github}/tree/master/src/main/java/org/springframework/cloud/security/oauth2/proxy/ProxyAuthenticationProperties[ ProxyAuthenticationProperties] for full details.

</div>

</div>

</div>

</div>

<div id="footer">

<div id="footer-text">Last updated 2016-01-26 10:56:04 UTC</div>

</div>

<script type="text/javascript">/* <![CDATA[ */(function(d,s,a,i,j,r,l,m,t){try{l=d.getElementsByTagName('a');t=d.createElement('textarea');for(i=0;l.length-i;i++){try{a=l[i].href;s=a.indexOf('/cdn-cgi/l/email-protection');m=a.length;if(a&&s>-1&&m>28){j=28+s;s='';if(j<m){r='0x'+a.substr(j,2)|0;for(j+=2;j<m&&a.charAt(j)!='X';j+=2)s+='%'+('0'+('0x'+a.substr(j,2)^r).toString(16)).slice(-2);j++;s=decodeURIComponent(s)+a.substr(j,m-j)}t.innerHTML=s.replace(/</g,'&lt;').replace(/>/g,'&gt;');l[i].href='mailto:'+t.value}}catch(e){}}}catch(e){}})(document);/* ]]> */</script>