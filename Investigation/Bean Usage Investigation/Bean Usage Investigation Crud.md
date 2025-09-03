#investigation #beans

{
    "contexts": {
        "application": {
            "beans": {
                "applicationSubmissionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ApplicationSubmissionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ApplicationSubmissionService.class]",
                    "dependencies": [
                        "applicationSubmissionRepository"
                    ]
                },
                "spring.jpa-org.springframework.boot.autoconfigure.orm.jpa.JpaProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.orm.jpa.JpaProperties",
                    "resource": null,
                    "dependencies": []
                },
                "sentrySpanAdvisor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.aop.support.DefaultPointcutAdvisor",
                    "resource": "class path resource [io/sentry/spring/tracing/SentryAdviceConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.tracing.SentryAdviceConfiguration",
                        "sentrySpanPointcut",
                        "sentrySpanAdvice"
                    ]
                },
                "policyTransactionCopyRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyTransactionCopyRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyTransactionCopyRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#440521c4",
                        "(inner bean)#589da32a",
                        "(inner bean)#4d7648a5",
                        "jpaMappingContext"
                    ]
                },
                "management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "spring.servlet.multipart-org.springframework.boot.autoconfigure.web.servlet.MultipartProperties"
                    ]
                },
                "noteService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.NoteService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/NoteService.class]",
                    "dependencies": [
                        "noteRepository"
                    ]
                },
                "campaignEmployeeDetailsService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CampaignEmployeeDetailsService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CampaignEmployeeDetailsService.class]",
                    "dependencies": [
                        "campaignEmployeeDetailsRepository"
                    ]
                },
                "jdbcTemplate": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.jdbc.core.JdbcTemplate",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jdbc/JdbcTemplateConfiguration.class]",
                    "dependencies": [
                        "dataSourceScriptDatabaseInitializer",
                        "org.springframework.boot.autoconfigure.jdbc.JdbcTemplateConfiguration",
                        "dataSource",
                        "spring.jdbc-org.springframework.boot.autoconfigure.jdbc.JdbcProperties"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c",
                        "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties"
                    ]
                },
                "mondayService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.MondayService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/MondayService.class]",
                    "dependencies": [
                        "properties",
                        "userService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.cache.CachesEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.cache.CachesEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "cnaUnderwritingAttestationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CnaUnderwritingAttestationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CnaUnderwritingAttestationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#54aac0c1",
                        "(inner bean)#716d8f22",
                        "(inner bean)#378c66fb",
                        "jpaMappingContext"
                    ]
                },
                "dashboardController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.DashboardController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/DashboardController.class]",
                    "dependencies": [
                        "validationHelper",
                        "policyService",
                        "applicationSubmissionService",
                        "businessService",
                        "quoteService",
                        "claimService"
                    ]
                },
                "businessClassificationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.BusinessClassificationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.BusinessClassificationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#76ea6f89",
                        "(inner bean)#71e1c7fc",
                        "(inner bean)#30b84f33",
                        "jpaMappingContext"
                    ]
                },
                "customCoverageElementRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CustomCoverageElementRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CustomCoverageElementRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#15b0118",
                        "(inner bean)#37d96651",
                        "(inner bean)#6848faeb",
                        "jpaMappingContext"
                    ]
                },
                "beanNameViewResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.view.BeanNameViewResolver",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration"
                    ]
                },
                "policyDocumentRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyDocumentRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyDocumentRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4388206e",
                        "(inner bean)#136cb5b5",
                        "(inner bean)#74dc61a0",
                        "jpaMappingContext"
                    ]
                },
                "employeeContactInformationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.EmployeeContactInformationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.EmployeeContactInformationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3715c959",
                        "(inner bean)#298734a9",
                        "(inner bean)#41285940",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.endpoint.web.servlet.WebMvcEndpointManagementContextConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.servlet.WebMvcEndpointManagementContextConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "projectingArgumentResolverBeanPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.web.config.ProjectingArgumentResolverRegistrar$ProjectingArgumentResolverBeanPostProcessor",
                    "resource": "class path resource [org/springframework/data/web/config/ProjectingArgumentResolverRegistrar.class]",
                    "dependencies": []
                },
                "boldPenguinService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.BoldPenguinService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/BoldPenguinService.class]",
                    "dependencies": [
                        "properties",
                        "businessService",
                        "addressService",
                        "businessLocationService",
                        "licenseService",
                        "businessClassificationService",
                        "closeService"
                    ]
                },
                "partnerPreferencesRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerPreferencesRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerPreferencesRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#160a5e87",
                        "(inner bean)#61c9e646",
                        "(inner bean)#5d9d7f05",
                        "jpaMappingContext"
                    ]
                },
                "org.springdoc.core.SwaggerUiConfigParameters": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SwaggerUiConfigParameters",
                    "resource": null,
                    "dependencies": [
                        "org.springdoc.core.SwaggerUiConfigProperties"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.OAuth2ResourceServerAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.OAuth2ResourceServerAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "coiToolService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.CoiToolService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/CoiToolService.class]",
                    "dependencies": [
                        "properties",
                        "certificateOfInsuranceService",
                        "coiToolServiceUtil",
                        "coiPolicyLinkService"
                    ]
                },
                "server-org.springframework.boot.autoconfigure.web.ServerProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.ServerProperties",
                    "resource": null,
                    "dependencies": []
                },
                "messageConverters": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.http.HttpMessageConverters",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/http/HttpMessageConvertersAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration"
                    ]
                },
                "websocketServletWebServerCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.websocket.servlet.TomcatWebSocketServletWebServerCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/websocket/servlet/WebSocketServletAutoConfiguration$TomcatWebSocketConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration$TomcatWebSocketConfiguration"
                    ]
                },
                "slackLeadService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.SlackLeadService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/SlackLeadService.class]",
                    "dependencies": [
                        "slackLeadRepository",
                        "activityRepository",
                        "businessRepository",
                        "employeeContactInformationService",
                        "properties"
                    ]
                },
                "helpScoutTicketRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.HelpScoutTicketRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.HelpScoutTicketRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#2eb4d9ee",
                        "(inner bean)#6a15d338",
                        "(inner bean)#55c6e0d0",
                        "jpaMappingContext"
                    ]
                },
                "configurationPropertiesReportEndpointWebExtension": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.context.properties.ConfigurationPropertiesReportEndpointWebExtension",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/context/properties/ConfigurationPropertiesReportEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointAutoConfiguration",
                        "configurationPropertiesReportEndpoint"
                    ]
                },
                "campaignStatusRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CampaignStatusRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CampaignStatusRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#17cb2dfd",
                        "(inner bean)#1cebff9f",
                        "(inner bean)#3d01c301",
                        "jpaMappingContext"
                    ]
                },
                "policyTypeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyTypeService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyTypeService.class]",
                    "dependencies": [
                        "policyTypeRepository",
                        "policyService"
                    ]
                },
                "userRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.UserRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.UserRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#38e1d2c4",
                        "(inner bean)#3951efe0",
                        "(inner bean)#15b078f",
                        "jpaMappingContext"
                    ]
                },
                "carrierRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CarrierRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CarrierRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3d746c8f",
                        "(inner bean)#1841d013",
                        "(inner bean)#3cc7ed87",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.security.servlet.SecurityRequestMatchersManagementContextConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.security.servlet.SecurityRequestMatchersManagementContextConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "agentAssistant": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentAssistant",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentAssistant.class]",
                    "dependencies": [
                        "accountManagerPayoutMetricService",
                        "businessService",
                        "closeService",
                        "policyService",
                        "renewalBatchService",
                        "carrierAutoRenewalService"
                    ]
                },
                "businessService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.BusinessService$$EnhancerBySpringCGLIB$$5b1d8dfd",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/BusinessService.class]",
                    "dependencies": [
                        "properties",
                        "businessRepository"
                    ]
                },
                "excludedCoverageElementService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ExcludedCoverageElementService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ExcludedCoverageElementService.class]",
                    "dependencies": [
                        "excludedCoverageElementRepository"
                    ]
                },
                "partnerWebpageRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerWebpageRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerWebpageRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#7d1e54a6",
                        "(inner bean)#55f3c568",
                        "(inner bean)#6e0e8b7b",
                        "jpaMappingContext"
                    ]
                },
                "cohortService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CohortService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CohortService.class]",
                    "dependencies": [
                        "cohortRepository",
                        "policyRepository",
                        "businessRepository"
                    ]
                },
                "metricsHttpClientUriTagFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.config.MeterFilter$9",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/client/HttpClientMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.client.HttpClientMetricsAutoConfiguration",
                        "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties"
                    ]
                },
                "management.health.diskspace-org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthIndicatorProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthIndicatorProperties",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.gson.GsonAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.gson.GsonAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "management.endpoint.env-org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointProperties",
                    "resource": null,
                    "dependencies": []
                },
                "formPageService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.FormPageService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/FormPageService.class]",
                    "dependencies": [
                        "properties",
                        "applicationSubmissionService",
                        "addressService",
                        "generalClassificationInformationService",
                        "businessService",
                        "ncciClassService",
                        "businessLocationService",
                        "userService",
                        "businessClassificationService",
                        "closeService"
                    ]
                },
                "ecommerceClassificationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.EcommerceClassificationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/EcommerceClassificationService.class]",
                    "dependencies": [
                        "ecommerceClassificationRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.orm.jpa.JpaBaseConfiguration$JpaWebConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.orm.jpa.JpaBaseConfiguration$JpaWebConfiguration",
                    "resource": null,
                    "dependencies": [
                        "spring.jpa-org.springframework.boot.autoconfigure.orm.jpa.JpaProperties"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.JdbcTemplateAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.JdbcTemplateAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.availability.ApplicationAvailabilityAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.availability.ApplicationAvailabilityAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "metricsEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.MetricsEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/MetricsEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.MetricsEndpointAutoConfiguration",
                        "simpleMeterRegistry"
                    ]
                },
                "org.springframework.boot.autoconfigure.aop.AopAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.aop.AopAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "sentryExceptionResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.SentryExceptionResolver",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration",
                        "sentryHub",
                        "transactionNameProvider",
                        "sentry-io.sentry.spring.boot.SentryProperties"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.info.InfoContributorAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.info.InfoContributorAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "customFormFieldService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CustomFormFieldService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CustomFormFieldService.class]",
                    "dependencies": [
                        "customFormFieldRepository"
                    ]
                },
                "paymentRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PaymentRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PaymentRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4f185b5d",
                        "(inner bean)#5a9843bf",
                        "(inner bean)#40dcfef3",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.jpa.hibernate-org.springframework.boot.autoconfigure.orm.jpa.HibernateProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.orm.jpa.HibernateProperties",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.Oauth2ResourceServerConfiguration$JwtConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.Oauth2ResourceServerConfiguration$JwtConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "s3UploadService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.S3UploadService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/S3UploadService.class]",
                    "dependencies": [
                        "properties",
                        "s3UploadRepository",
                        "policyDocumentRepository",
                        "policyRepository"
                    ]
                },
                "carrierQuoteRequestService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CarrierQuoteRequestService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CarrierQuoteRequestService.class]",
                    "dependencies": [
                        "carrierQuoteRequestRepository"
                    ]
                },
                "coiPolicyLinkRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CoiPolicyLinkRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CoiPolicyLinkRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#77e912f8",
                        "(inner bean)#23877a53",
                        "(inner bean)#4ffb223c",
                        "jpaMappingContext"
                    ]
                },
                "localeCharsetMappingsCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration$LocaleCharsetMappingsCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/HttpEncodingAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration"
                    ]
                },
                "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "carrierService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CarrierService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CarrierService.class]",
                    "dependencies": [
                        "carrierRepository"
                    ]
                },
                "agentAvailabilityService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.AgentAvailabilityService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/AgentAvailabilityService.class]",
                    "dependencies": [
                        "properties",
                        "agentStatusService",
                        "agentStatusHistoryService",
                        "campaignStatusHistoryService"
                    ]
                },
                "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$EnableTransactionManagementConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$EnableTransactionManagementConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "customCoverageElementService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CustomCoverageElementService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CustomCoverageElementService.class]",
                    "dependencies": [
                        "customCoverageElementRepository",
                        "ownerOfficer",
                        "coverageElementService"
                    ]
                },
                "routerFunctionMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.function.support.RouterFunctionMapping",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcConversionService",
                        "mvcResourceUrlProvider"
                    ]
                },
                "org.springframework.security.config.annotation.web.configuration.HttpSecurityConfiguration.httpSecurity": {
                    "aliases": [],
                    "scope": "prototype",
                    "type": "org.springframework.security.config.annotation.web.builders.HttpSecurity",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/HttpSecurityConfiguration.class]",
                    "dependencies": [
                        "org.springframework.security.config.annotation.web.configuration.HttpSecurityConfiguration"
                    ]
                },
                "emailHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.EmailHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.EmailHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3627e94a",
                        "(inner bean)#7dcbb6e5",
                        "(inner bean)#5222c67",
                        "jpaMappingContext"
                    ]
                },
                "coverageService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.CoverageService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/CoverageService.class]",
                    "dependencies": [
                        "ownerOfficer"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration$ErrorPageSecurityFilterConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration$ErrorPageSecurityFilterConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.task.scheduling-org.springframework.boot.autoconfigure.task.TaskSchedulingProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.task.TaskSchedulingProperties",
                    "resource": null,
                    "dependencies": []
                },
                "asyncConfig": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.configuration.AsyncConfig$$EnhancerBySpringCGLIB$$40680952",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/configuration/AsyncConfig.class]",
                    "dependencies": []
                },
                "metricsController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.metricsControllers.MetricsController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/metricsControllers/MetricsController.class]",
                    "dependencies": [
                        "validationHelper",
                        "policyService",
                        "employeeContactInformationService",
                        "metricsService",
                        "licenseService",
                        "businessClassificationService",
                        "adminAppUserUtil",
                        "accountManagerPayoutMetricService",
                        "partnerPaymentStructureService",
                        "partnerDashboardApiHistoryService",
                        "partnerPaymentsUtil"
                    ]
                },
                "healthEndpointWebExtension": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.health.HealthEndpointWebExtension",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointWebExtensionConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration",
                        "healthContributorRegistry",
                        "healthEndpointGroups",
                        "management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties"
                    ]
                },
                "partnerTechnologyFeeRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerTechnologyFeeRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerTechnologyFeeRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5b792e4a",
                        "(inner bean)#8fa7f10",
                        "(inner bean)#338e0952",
                        "jpaMappingContext"
                    ]
                },
                "conversionServicePostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.crypto.RsaKeyConversionServicePostProcessor",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/WebSecurityConfiguration.class]",
                    "dependencies": []
                },
                "lifecycleProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.context.support.DefaultLifecycleProcessor",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/context/LifecycleAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.context.LifecycleAutoConfiguration",
                        "spring.lifecycle-org.springframework.boot.autoconfigure.context.LifecycleProperties"
                    ]
                },
                "simpleMessageListenerContainer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.messaging.listener.SimpleMessageListenerContainer",
                    "resource": "class path resource [org/springframework/cloud/aws/messaging/config/annotation/SqsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.cloud.aws.messaging.config.annotation.SqsConfiguration",
                        "amazonSQS",
                        "queueMessageHandler"
                    ]
                },
                "licenseThemeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LicenseThemeService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LicenseThemeService.class]",
                    "dependencies": [
                        "licenseThemeRepository"
                    ]
                },
                "org.springframework.cloud.aws.autoconfigure.context.ContextResourceLoaderAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.context.ContextResourceLoaderAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.data.jpa.repository.support.JpaEvaluationContextExtension": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.jpa.repository.support.JpaEvaluationContextExtension",
                    "resource": null,
                    "dependencies": []
                },
                "sentryRequestResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.SentryRequestResolver",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration",
                        "sentryHub"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.web.client.HttpClientMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.web.client.HttpClientMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "io.sentry.spring.boot.SentryAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.context.ConfigurationPropertiesAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.context.ConfigurationPropertiesAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.security.config.annotation.web.configuration.HttpSecurityConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.web.configuration.HttpSecurityConfiguration",
                    "resource": null,
                    "dependencies": [
                        "org.springframework.security.config.annotation.authentication.configuration.AuthenticationConfiguration",
                        "objectPostProcessor"
                    ]
                },
                "coterieControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.CoterieControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/CoterieControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "objectMapper",
                        "webhookHistoryService",
                        "reconcileCoterieDataService"
                    ]
                },
                "sentrySpringFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.FilterRegistrationBean",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration",
                        "sentryHub",
                        "sentryRequestResolver",
                        "transactionNameProvider"
                    ]
                },
                "sentryTracingFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.FilterRegistrationBean",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration",
                        "sentryHub",
                        "transactionNameProvider"
                    ]
                },
                "lateInvoiceTrackerService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.LateInvoiceTrackerService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/LateInvoiceTrackerService.class]",
                    "dependencies": [
                        "lateInvoicePolicyLinkService",
                        "lateInvoiceService",
                        "ascendService",
                        "policyService",
                        "closeService",
                        "employeeContactInformationService",
                        "s3UploadService",
                        "noticeOfCancellationService",
                        "properties"
                    ]
                },
                "agentScoreWeightService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentScoreWeightService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentScoreWeightService.class]",
                    "dependencies": [
                        "agentScoreWeightRepository"
                    ]
                },
                "leadMatchHistoryEntryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LeadMatchHistoryEntryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LeadMatchHistoryEntryService.class]",
                    "dependencies": [
                        "leadMatchHistoryEntryRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.info.ProjectInfoAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.info.ProjectInfoAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "spring.info-org.springframework.boot.autoconfigure.info.ProjectInfoProperties"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.web.client.RestTemplateMetricsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.web.client.RestTemplateMetricsConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "carrierAppetiteSuggestionOverrideService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CarrierAppetiteSuggestionOverrideService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CarrierAppetiteSuggestionOverrideService.class]",
                    "dependencies": [
                        "carrierAppetiteSuggestionOverrideRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryConfiguration$EmbeddedTomcat": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryConfiguration$EmbeddedTomcat",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.management.HeapDumpWebEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.management.HeapDumpWebEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "delegatingApplicationListener": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.context.DelegatingApplicationListener",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/WebSecurityConfiguration.class]",
                    "dependencies": []
                },
                "httpServletRequestSentryUserProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.HttpServletRequestSentryUserProvider",
                    "resource": "class path resource [io/sentry/spring/SentryWebConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.SentryWebConfiguration",
                        "sentry-io.sentry.spring.boot.SentryProperties"
                    ]
                },
                "responseBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.GenericResponseService",
                    "resource": "class path resource [org/springdoc/webmvc/core/SpringDocWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration",
                        "operationBuilder",
                        "genericReturnTypeParser",
                        "org.springdoc.core.SpringDocConfigProperties",
                        "propertyResolverUtils"
                    ]
                },
                "org.springframework.data.web.config.SpringDataJacksonConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.web.config.SpringDataJacksonConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "taskRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.TaskRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.TaskRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4a2bf283",
                        "(inner bean)#687bf48e",
                        "(inner bean)#22d57aa3",
                        "jpaMappingContext"
                    ]
                },
                "shareInfoRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ShareInfoRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ShareInfoRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#233f9fc",
                        "(inner bean)#7de621f",
                        "(inner bean)#16cb3161",
                        "jpaMappingContext"
                    ]
                },
                "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties",
                    "resource": null,
                    "dependencies": []
                },
                "affinityPartnerCommissionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AffinityPartnerCommissionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AffinityPartnerCommissionService.class]",
                    "dependencies": [
                        "affinityPartnerCommissionRepository"
                    ]
                },
                "trimmedDocService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TrimmedDocService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TrimmedDocService.class]",
                    "dependencies": []
                },
                "accountManagerPayoutMetricRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AccountManagerPayoutMetricRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AccountManagerPayoutMetricRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6707fc3e",
                        "(inner bean)#7d365620",
                        "(inner bean)#7b330cbd",
                        "jpaMappingContext"
                    ]
                },
                "requestBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.core.RequestService",
                    "resource": "class path resource [org/springdoc/webmvc/core/SpringDocWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration",
                        "parameterBuilder",
                        "requestBodyBuilder",
                        "operationBuilder",
                        "localSpringDocParameterNameDiscoverer"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "metricsRepositoryMethodInvocationListener": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.data.MetricsRepositoryMethodInvocationListener",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/data/RepositoryMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.data.RepositoryMetricsAutoConfiguration",
                        "repositoryTagsProvider"
                    ]
                },
                "activityService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ActivityService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ActivityService.class]",
                    "dependencies": [
                        "activityRepository",
                        "properties"
                    ]
                },
                "stripeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.StripeService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/StripeService.class]",
                    "dependencies": [
                        "properties",
                        "virtualCardService"
                    ]
                },
                "naicsClassificationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.NaicsClassificationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.NaicsClassificationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#317f3713",
                        "(inner bean)#10418c7",
                        "(inner bean)#6cebeb7d",
                        "jpaMappingContext"
                    ]
                },
                "businessLocationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.BusinessLocationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.BusinessLocationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6a2e7d2d",
                        "(inner bean)#6ca20c96",
                        "(inner bean)#4790479a",
                        "jpaMappingContext"
                    ]
                },
                "pathMappedEndpoints": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.PathMappedEndpoints",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration",
                        "servletEndpointDiscoverer",
                        "webEndpointDiscoverer",
                        "controllerEndpointDiscoverer"
                    ]
                },
                "jvmThreadMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.jvm.JvmThreadMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/JvmMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration"
                    ]
                },
                "campaignStatusService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CampaignStatusService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CampaignStatusService.class]",
                    "dependencies": [
                        "campaignStatusRepository"
                    ]
                },
                "adminAppService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.AdminAppService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/AdminAppService.class]",
                    "dependencies": [
                        "properties",
                        "renewalBatchService",
                        "renewalsService",
                        "closeService",
                        "employeeContactInformationService",
                        "adminAppUserUtil",
                        "policyService",
                        "policyTransactionService",
                        "coverdashUserUtil",
                        "helpscoutService",
                        "carrierService",
                        "applicationSubmissionService"
                    ]
                },
                "fileDescriptorMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.system.FileDescriptorMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/SystemMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.SystemMetricsAutoConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.aop.AopAutoConfiguration$AspectJAutoProxyingConfiguration$CglibAutoProxyConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.aop.AopAutoConfiguration$AspectJAutoProxyingConfiguration$CglibAutoProxyConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalFormController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.renewalsControllers.RenewalFormController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/renewalsControllers/RenewalFormController.class]",
                    "dependencies": [
                        "validationHelper",
                        "properties",
                        "userService",
                        "businessService",
                        "addressService",
                        "generalClassificationInformationService",
                        "businessLocationService",
                        "businessClassificationService",
                        "ncciClassService",
                        "renewalFormService",
                        "renewalFormFieldService",
                        "renewalChecklistItemService",
                        "formService",
                        "renewalBatchService",
                        "employeeContactInformationService",
                        "closeService",
                        "renewalsService"
                    ]
                },
                "opsAssignmentWeightRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.OpsAssignmentWeightRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.OpsAssignmentWeightRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#68ebc1ed",
                        "(inner bean)#f9b0bfb",
                        "(inner bean)#41404e50",
                        "jpaMappingContext"
                    ]
                },
                "conditionsReportEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.condition.ConditionsReportEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/condition/ConditionsReportEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.condition.ConditionsReportEndpointAutoConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "applicationAvailability": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.availability.ApplicationAvailabilityBean",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/availability/ApplicationAvailabilityAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.availability.ApplicationAvailabilityAutoConfiguration"
                    ]
                },
                "org.springdoc.webmvc.ui.SwaggerConfig": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.ui.SwaggerConfig",
                    "resource": null,
                    "dependencies": []
                },
                "mvcResourceUrlProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.resource.ResourceUrlProvider",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "technologyFeeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TechnologyFeeService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TechnologyFeeService.class]",
                    "dependencies": [
                        "properties",
                        "quoteService"
                    ]
                },
                "leadScoreWeightRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LeadScoreWeightRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LeadScoreWeightRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#42bab829",
                        "(inner bean)#44d0f9bc",
                        "(inner bean)#49329ce9",
                        "jpaMappingContext"
                    ]
                },
                "sentryHub": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.HubAdapter",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration",
                        "sentryOptionsConfiguration",
                        "sentry-io.sentry.spring.boot.SentryProperties"
                    ]
                },
                "servletEndpointRegistrar": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.ServletEndpointRegistrar",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/ServletEndpointManagementContextConfiguration$WebMvcServletEndpointManagementContextConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration$WebMvcServletEndpointManagementContextConfiguration",
                        "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties",
                        "servletEndpointDiscoverer",
                        "dispatcherServletRegistration"
                    ]
                },
                "renewalFormTemplateService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalFormTemplateService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalFormTemplateService.class]",
                    "dependencies": [
                        "renewalFormTemplateRepository"
                    ]
                },
                "agentLeadRuleService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentLeadRuleService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentLeadRuleService.class]",
                    "dependencies": [
                        "agentLeadRuleRepository"
                    ]
                },
                "transactionManagerService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.TransactionManagerService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/TransactionManagerService.class]",
                    "dependencies": [
                        "policyTransactionService",
                        "carrierCommission",
                        "paymentPlanService",
                        "paymentService"
                    ]
                },
                "leadScoreWeightService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LeadScoreWeightService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LeadScoreWeightService.class]",
                    "dependencies": [
                        "leadScoreWeightRepository"
                    ]
                },
                "org.springdoc.core.SpringDocConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.cloud.aws.autoconfigure.messaging.MessagingAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.messaging.MessagingAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "springSecuritySentryUserProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.SpringSecuritySentryUserProvider",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration$SentrySecurityConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration$SentrySecurityConfiguration",
                        "sentry-io.sentry.spring.boot.SentryProperties"
                    ]
                },
                "partnerWebpageService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerWebpageService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerWebpageService.class]",
                    "dependencies": [
                        "partnerWebpageRepository"
                    ]
                },
                "queueMessageHandler": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.messaging.listener.QueueMessageHandler",
                    "resource": "class path resource [org/springframework/cloud/aws/messaging/config/annotation/SqsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.cloud.aws.messaging.config.annotation.SqsConfiguration"
                    ]
                },
                "manualPlacementService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.ManualPlacementService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/ManualPlacementService.class]",
                    "dependencies": [
                        "quoteService",
                        "properties",
                        "stripeService",
                        "virtualCardService",
                        "validationHelper",
                        "closeService",
                        "businessService",
                        "businessLocationService",
                        "addressService",
                        "userService",
                        "generalClassificationInformationService",
                        "policyService",
                        "customCoverageElementService",
                        "tooltipService",
                        "adminAppUserUtil",
                        "policyTransactionService",
                        "certificateOfInsuranceService",
                        "coiToolService",
                        "claimService",
                        "customFormFieldService",
                        "subscriptionService",
                        "braintreeService",
                        "leadService",
                        "leadScoringEngineService",
                        "agentOutOfOfficeService",
                        "renewalBatchService",
                        "lateInvoiceService",
                        "lateInvoicePolicyLinkService",
                        "coverdashUserUtil",
                        "saleService"
                    ]
                },
                "io.sentry.spring.tracing.SentrySpanPointcutConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.tracing.SentrySpanPointcutConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalsController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.renewalsControllers.RenewalsController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/renewalsControllers/RenewalsController.class]",
                    "dependencies": [
                        "validationHelper",
                        "properties",
                        "carrierService",
                        "renewalBatchService",
                        "renewalPolicyService",
                        "renewalLifeCycleService",
                        "adminAppUserUtil",
                        "renewalChecklistItemService",
                        "renewalFormService",
                        "renewalFormTemplateService",
                        "baseRenewalFormFieldService",
                        "adminAppService",
                        "employeeContactInformationService",
                        "emailHistoryService",
                        "renewalsService",
                        "closeService",
                        "businessService",
                        "ascendService",
                        "licenseService",
                        "userService",
                        "policyService",
                        "addressService",
                        "businessLocationService",
                        "businessClassificationService",
                        "renewalSLAEvaluationService"
                    ]
                },
                "contextTagsEventProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.ContextTagsEventProcessor",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$ContextTagsEventProcessorConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$ContextTagsEventProcessorConfiguration",
                        "sentry-io.sentry.spring.boot.SentryProperties"
                    ]
                },
                "businessRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.BusinessRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.BusinessRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5223eb62",
                        "(inner bean)#1b65076",
                        "(inner bean)#730b8793",
                        "jpaMappingContext"
                    ]
                },
                "operationsService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.OperationsService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/OperationsService.class]",
                    "dependencies": [
                        "braintreeService",
                        "subscriptionService",
                        "stripeService",
                        "virtualCardService",
                        "properties",
                        "emailHistoryService",
                        "helpscoutService",
                        "employeeContactInformationService",
                        "coverdashUserUtil",
                        "policyService",
                        "closeService",
                        "loopsService",
                        "userService",
                        "renewalLifeCycleService",
                        "renewalBatchService",
                        "renewalsService",
                        "policyTransactionService",
                        "transactionManagerService",
                        "lateInvoiceService",
                        "lateInvoiceTrackerService"
                    ]
                },
                "webSecurityConfig": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.oauthSetup.WebSecurityConfig$$EnhancerBySpringCGLIB$$2735330a",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/oauthSetup/WebSecurityConfig.class]",
                    "dependencies": []
                },
                "amazonS3": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.amazonaws.services.s3.AmazonS3Client",
                    "resource": null,
                    "dependencies": [
                        "credentialsProvider",
                        "org.springframework.cloud.aws.core.region.RegionProvider.BEAN_NAME"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.Oauth2ResourceServerConfiguration$OpaqueTokenConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.Oauth2ResourceServerConfiguration$OpaqueTokenConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "hiscoxUnderwritingQuestionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.HiscoxUnderwritingQuestionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.HiscoxUnderwritingQuestionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#503c6c4d",
                        "(inner bean)#467e6dc2",
                        "(inner bean)#69d5078d",
                        "jpaMappingContext"
                    ]
                },
                "employeeController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.EmployeeController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/EmployeeController.class]",
                    "dependencies": [
                        "validationHelper",
                        "employeeContactInformationService"
                    ]
                },
                "renewalChecklistItemRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalChecklistItemRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalChecklistItemRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1d6d1a18",
                        "(inner bean)#2b6cd876",
                        "(inner bean)#519910b2",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.data.web.config.SpringDataWebConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.web.config.SpringDataWebConfiguration",
                    "resource": null,
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "generalControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.GeneralControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/GeneralControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "userService",
                        "applicationSubmissionService",
                        "quoteService",
                        "businessService",
                        "policyService",
                        "closeService",
                        "slackLeadService",
                        "lateInvoiceService",
                        "coverdashUserUtil",
                        "employeeContactInformationService"
                    ]
                },
                "agentStatusService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentStatusService$$EnhancerBySpringCGLIB$$e618e3d6",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentStatusService.class]",
                    "dependencies": [
                        "agentStatusRepository"
                    ]
                },
                "errorPageRegistrarBeanPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.server.ErrorPageRegistrarBeanPostProcessor",
                    "resource": null,
                    "dependencies": []
                },
                "mvcConversionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.format.support.DefaultFormattingConversionService",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "ncciClassService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.NcciClassService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/NcciClassService.class]",
                    "dependencies": [
                        "ncciClassRepository"
                    ]
                },
                "initializeAuthenticationProviderBeanManagerConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.authentication.configuration.InitializeAuthenticationProviderBeanManagerConfigurer",
                    "resource": "class path resource [org/springframework/security/config/annotation/authentication/configuration/AuthenticationConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "controllerEndpointDiscoverer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.annotation.ControllerEndpointDiscoverer",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration"
                    ]
                },
                "jvmMemoryMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.jvm.JvmMemoryMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/JvmMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration"
                    ]
                },
                "ringbaCampaignWeightService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RingbaCampaignWeightService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RingbaCampaignWeightService.class]",
                    "dependencies": [
                        "ringbaCampaignWeightRepository"
                    ]
                },
                "io.sentry.spring.SentryWebConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.SentryWebConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "quotingPageController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.QuotingPageController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/QuotingPageController.class]",
                    "dependencies": [
                        "validationHelper",
                        "applicationSubmissionBatchService",
                        "policyTypeService",
                        "properties",
                        "businessService",
                        "businessClassificationService",
                        "carrierAppetiteSuggestionOverrideService",
                        "applicationSubmissionService",
                        "licenseService",
                        "quotingPageService",
                        "quoteService",
                        "hybridApplicationInProgressService",
                        "coverageElementService",
                        "adminAppUserUtil",
                        "employeeContactInformationService"
                    ]
                },
                "helpscoutControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.HelpscoutControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/HelpscoutControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "helpscoutService",
                        "policyService",
                        "policyTransactionService",
                        "businessService",
                        "opsAssignmentWeightService",
                        "helpScoutTicketService",
                        "helpScoutTicketHistoryService",
                        "employeeContactInformationService"
                    ]
                },
                "mvcPathMatcher": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.util.AntPathMatcher",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "management.metrics.export.simple-org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleProperties",
                    "resource": null,
                    "dependencies": []
                },
                "routerFunctionProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.core.RouterFunctionWebMvcProvider",
                    "resource": "class path resource [org/springdoc/webmvc/core/SpringDocWebMvcConfiguration$SpringDocWebMvcRouterConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration$SpringDocWebMvcRouterConfiguration"
                    ]
                },
                "agentOutOfOfficeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentOutOfOfficeService$$EnhancerBySpringCGLIB$$83025269",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentOutOfOfficeService.class]",
                    "dependencies": [
                        "agentOutOfOfficeRepository"
                    ]
                },
                "io.sentry.spring.tracing.SentryTransactionPointcutConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.tracing.SentryTransactionPointcutConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "pingHealthContributor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.health.PingHealthIndicator",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthContributorAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthContributorAutoConfiguration"
                    ]
                },
                "sentrySpanAdvice": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.tracing.SentrySpanAdvice",
                    "resource": "class path resource [io/sentry/spring/tracing/SentryAdviceConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.tracing.SentryAdviceConfiguration",
                        "sentryHub"
                    ]
                },
                "leadRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LeadRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LeadRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#2016896e",
                        "(inner bean)#427a0746",
                        "(inner bean)#515a3e3a",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.http.GsonHttpMessageConvertersConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.http.GsonHttpMessageConvertersConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalChecklistItemService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalChecklistItemService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalChecklistItemService.class]",
                    "dependencies": [
                        "renewalChecklistItemRepository"
                    ]
                },
                "namedParameterJdbcTemplate": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.jdbc.core.namedparam.NamedParameterJdbcTemplate",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jdbc/NamedParameterJdbcTemplateConfiguration.class]",
                    "dependencies": [
                        "dataSourceScriptDatabaseInitializer",
                        "org.springframework.boot.autoconfigure.jdbc.NamedParameterJdbcTemplateConfiguration",
                        "jdbcTemplate"
                    ]
                },
                "org.springframework.cloud.aws.autoconfigure.messaging.MessagingAutoConfiguration$SnsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.messaging.MessagingAutoConfiguration$SnsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.web-org.springframework.boot.autoconfigure.web.WebProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.WebProperties",
                    "resource": null,
                    "dependencies": []
                },
                "soldBusinessService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.SoldBusinessService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/SoldBusinessService.class]",
                    "dependencies": [
                        "soldBusinessRepository",
                        "tivlyService",
                        "boldPenguinService"
                    ]
                },
                "ascendControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.AscendControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/AscendControllerPublic.class]",
                    "dependencies": [
                        "validationHelper",
                        "ascendService",
                        "policyService",
                        "renewalBatchService",
                        "renewalLifeCycleService",
                        "renewalsService",
                        "quoteService",
                        "webhookHistoryService",
                        "lateInvoiceTrackerService",
                        "lateInvoiceService",
                        "closeService",
                        "properties"
                    ]
                },
                "simpleConfig": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimplePropertiesConfigAdapter",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/export/simple/SimpleMetricsExportAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleMetricsExportAutoConfiguration",
                        "management.metrics.export.simple-org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleProperties"
                    ]
                },
                "renewalCarrierSLAService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalCarrierSLAService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalCarrierSLAService.class]",
                    "dependencies": [
                        "renewalCarrierSLARepository"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceAspectsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceAspectsConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "businessClassificationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.BusinessClassificationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/BusinessClassificationService.class]",
                    "dependencies": [
                        "businessClassificationRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.JdbcTemplateConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.JdbcTemplateConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "agencyStatRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgencyStatRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgencyStatRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5107f87e",
                        "(inner bean)#74bf382f",
                        "(inner bean)#5a8daa11",
                        "jpaMappingContext"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceAspectsConfiguration$SentrySpanPointcutAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceAspectsConfiguration$SentrySpanPointcutAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "requestBodyBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.RequestBodyService",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "parameterBuilder"
                    ]
                },
                "endpointCachingOperationInvokerAdvisor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.invoker.cache.CachingOperationInvokerAdvisor",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/EndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.EndpointAutoConfiguration",
                        "environment"
                    ]
                },
                "defaultServletHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.HandlerMapping",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "renewalsService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.renewals.RenewalsService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/renewals/RenewalsService.class]",
                    "dependencies": [
                        "carrierAutoRenewalService",
                        "renewalLifeCycleService",
                        "businessService",
                        "renewalBatchService",
                        "renewalBillingBatchService",
                        "renewalChecklistItemService",
                        "renewalFormService",
                        "renewalFormFieldService",
                        "baseRenewalFormFieldService",
                        "customFormFieldService",
                        "renewalPolicyService",
                        "policyService",
                        "tooltipService",
                        "customCoverageElementService",
                        "closeService",
                        "policyTransactionService",
                        "coiToolService",
                        "ascendService",
                        "emailHistoryService",
                        "employeeContactInformationService",
                        "helpscoutService",
                        "savvyCalService",
                        "adminAppUserUtil",
                        "carrierCommission",
                        "saleService",
                        "slackNotificationUtil",
                        "renewalSLAEvaluationService",
                        "powerPointService"
                    ]
                },
                "renewalBillingBatchService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalBillingBatchService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalBillingBatchService.class]",
                    "dependencies": [
                        "renewalBillingBatchRepository"
                    ]
                },
                "swaggerWebMvcConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.ui.SwaggerWebMvcConfigurer",
                    "resource": "class path resource [org/springdoc/webmvc/ui/SwaggerConfig.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.ui.SwaggerConfig",
                        "org.springdoc.core.SwaggerUiConfigParameters",
                        "indexPageTransformer"
                    ]
                },
                "globalExceptionHandler": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.web.GlobalExceptionHandler",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/web/GlobalExceptionHandler.class]",
                    "dependencies": []
                },
                "persistenceExceptionTranslationPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.dao.annotation.PersistenceExceptionTranslationPostProcessor",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/dao/PersistenceExceptionTranslationAutoConfiguration.class]",
                    "dependencies": [
                        "environment"
                    ]
                },
                "management.health.db-org.springframework.boot.actuate.autoconfigure.jdbc.DataSourceHealthIndicatorProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.jdbc.DataSourceHealthIndicatorProperties",
                    "resource": null,
                    "dependencies": []
                },
                "spring.data.web-org.springframework.boot.autoconfigure.data.web.SpringDataWebProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.data.web.SpringDataWebProperties",
                    "resource": null,
                    "dependencies": []
                },
                "renewalsControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.renewalsControllers.RenewalsControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/renewalsControllers/RenewalsControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "renewalsService",
                        "renewalSLAEvaluationService",
                        "renewalBatchService"
                    ]
                },
                "jwtDecoder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.oauth2.jwt.NimbusJwtDecoder",
                    "resource": "class path resource [com/coverdash/crud_service/oauthSetup/WebSecurityConfig.class]",
                    "dependencies": [
                        "webSecurityConfig"
                    ]
                },
                "preserveErrorControllerTargetClassPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$PreserveErrorControllerTargetClassPostProcessor",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration.class]",
                    "dependencies": []
                },
                "agentStatusRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentStatusRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentStatusRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#7efc8091",
                        "(inner bean)#472505ef",
                        "(inner bean)#124f03b9",
                        "jpaMappingContext"
                    ]
                },
                "tooltipService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TooltipService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TooltipService.class]",
                    "dependencies": [
                        "jdbcTemplate"
                    ]
                },
                "renewalFormFieldService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalFormFieldService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalFormFieldService.class]",
                    "dependencies": [
                        "renewalFormFieldRepository"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.trace.http.HttpTraceEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.trace.http.HttpTraceEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "policyTransactionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyTransactionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyTransactionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#519cb1bd",
                        "(inner bean)#48fd7749",
                        "(inner bean)#2454ee88",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.data.RepositoryMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.data.RepositoryMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties"
                    ]
                },
                "policyDocumentRelevantInformationMappingService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyDocumentRelevantInformationMappingService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyDocumentRelevantInformationMappingService.class]",
                    "dependencies": [
                        "policyDocumentRelevantInformationMappingRepository"
                    ]
                },
                "propertySourcesPlaceholderConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.context.support.PropertySourcesPlaceholderConfigurer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/context/PropertyPlaceholderAutoConfiguration.class]",
                    "dependencies": []
                },
                "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                    "resource": null,
                    "dependencies": [
                        "webConfig",
                        "swaggerWebMvcConfigurer",
                        "openEntityManagerInViewInterceptorConfigurer",
                        "metricsWebMvcConfigurer",
                        "org.springframework.data.web.config.SpringDataWebConfiguration",
                        "org.springframework.security.config.annotation.web.configuration.WebMvcSecurityConfiguration",
                        "org.springframework.cloud.aws.messaging.config.annotation.SnsWebConfiguration"
                    ]
                },
                "spring.security-org.springframework.boot.autoconfigure.security.SecurityProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.SecurityProperties",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.transaction.jta.JtaAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.jta.JtaAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "helpScoutTicketHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.HelpScoutTicketHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.HelpScoutTicketHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#76991b36",
                        "(inner bean)#2ca6b438",
                        "(inner bean)#5f4163c8",
                        "jpaMappingContext"
                    ]
                },
                "agentPayoutMetricService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentPayoutMetricService$$EnhancerBySpringCGLIB$$4e72feca",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentPayoutMetricService.class]",
                    "dependencies": [
                        "agentPayoutMetricRepository"
                    ]
                },
                "objectMapper": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.fasterxml.jackson.databind.ObjectMapper",
                    "resource": "com.coverdash.crud_service.CrudServiceApplication",
                    "dependencies": [
                        "crudServiceApplication"
                    ]
                },
                "accountExecutiveStatService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AccountExecutiveStatService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AccountExecutiveStatService.class]",
                    "dependencies": [
                        "accountExecutiveStatRepository"
                    ]
                },
                "techFeeEligibilityRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.TechFeeEligibilityRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.TechFeeEligibilityRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#58e35006",
                        "(inner bean)#69f5a73c",
                        "(inner bean)#26a9a09a",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.cloud.aws.autoconfigure.context.ContextCredentialsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.context.ContextCredentialsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration$TomcatWebServerFactoryCustomizerConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration$TomcatWebServerFactoryCustomizerConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration$SpringMvcConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration$SpringMvcConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "scheduledBeanLazyInitializationExcludeFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.task.ScheduledBeanLazyInitializationExcludeFilter",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/task/TaskSchedulingAutoConfiguration.class]",
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceJmxConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceJmxConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "warmTransferRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.WarmTransferRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.WarmTransferRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#f98d9b1",
                        "(inner bean)#37568ac9",
                        "(inner bean)#744200de",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.servlet.SecurityFilterAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.servlet.SecurityFilterAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "springSecurityFilterChain": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.web.FilterChainProxy",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/WebSecurityConfiguration.class]",
                    "dependencies": [
                        "org.springframework.security.config.annotation.web.configuration.WebSecurityConfiguration"
                    ]
                },
                "sic4MappingRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.Sic4MappingRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.Sic4MappingRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#25463407",
                        "(inner bean)#5ab85072",
                        "(inner bean)#5f990556",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.SystemMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.SystemMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "partnerPaymentsUtil": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.components.PartnerPaymentsUtil",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/components/PartnerPaymentsUtil.class]",
                    "dependencies": [
                        "policyService",
                        "policyTransactionService",
                        "partnerPaymentStructureService",
                        "applicationSubmissionService",
                        "businessService"
                    ]
                },
                "credentialsProvider": {
                    "aliases": [
                        "org.springframework.cloud.aws.core.credentials.CredentialsProviderFactoryBean.BEAN_NAME"
                    ],
                    "scope": "singleton",
                    "type": "com.amazonaws.auth.AWSCredentialsProvider",
                    "resource": null,
                    "dependencies": [
                        "(inner bean)#56ec6960",
                        "(inner bean)#73b74615"
                    ]
                },
                "applicationController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.ApplicationController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/ApplicationController.class]",
                    "dependencies": [
                        "validationHelper",
                        "carrierService",
                        "carrierQuoteRequestService",
                        "applicationSubmissionService",
                        "businessClassificationService",
                        "businessService",
                        "addressService",
                        "closeService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.startup.StartupTimeMetricsListenerAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.startup.StartupTimeMetricsListenerAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "servletMappingDescriptionProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.web.mappings.servlet.ServletsMappingDescriptionProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/web/mappings/MappingsEndpointAutoConfiguration$ServletWebConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration"
                    ]
                },
                "docIngestionAISubmissionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.DocIngestionAISubmissionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.DocIngestionAISubmissionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#60ed5158",
                        "(inner bean)#51223aca",
                        "(inner bean)#4f413b4c",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "instantPayControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.InstantPayControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/InstantPayControllerPublic.class]",
                    "dependencies": [
                        "stripeService",
                        "virtualCardService",
                        "properties"
                    ]
                },
                "addressRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AddressRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AddressRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#cf92193",
                        "(inner bean)#2b1205a7",
                        "(inner bean)#44261d79",
                        "jpaMappingContext"
                    ]
                },
                "lateInvoicePolicyLinkRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LateInvoicePolicyLinkRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LateInvoicePolicyLinkRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5ea34883",
                        "(inner bean)#1c43b31d",
                        "(inner bean)#1ca749cb",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "standardJacksonObjectMapperBuilderCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration$StandardJackson2ObjectMapperBuilderCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jackson/JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$Jackson2ObjectMapperBuilderCustomizerConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c",
                        "spring.jackson-org.springframework.boot.autoconfigure.jackson.JacksonProperties"
                    ]
                },
                "org.springframework.cloud.aws.messaging.config.annotation.SqsClientConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.messaging.config.annotation.SqsClientConfiguration",
                    "resource": null,
                    "dependencies": [
                        "credentialsProvider",
                        "org.springframework.cloud.aws.core.region.RegionProvider.BEAN_NAME"
                    ]
                },
                "taskSchedulerBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.task.TaskSchedulerBuilder",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/task/TaskSchedulingAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.task.TaskSchedulingAutoConfiguration",
                        "spring.task.scheduling-org.springframework.boot.autoconfigure.task.TaskSchedulingProperties"
                    ]
                },
                "publicController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.PublicController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/PublicController.class]",
                    "dependencies": [
                        "leadService",
                        "businessService",
                        "properties",
                        "startupIndustryService",
                        "businessClassificationService",
                        "userService",
                        "tooltipService",
                        "licenseService",
                        "saleService",
                        "partnerWebpageService",
                        "loopsService",
                        "closeService",
                        "slackNotificationUtil"
                    ]
                },
                "org.springframework.boot.autoconfigure.task.TaskExecutionAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.task.TaskExecutionAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.security.config.annotation.web.configuration.WebSecurityConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.web.configuration.WebSecurityConfiguration",
                    "resource": null,
                    "dependencies": [
                        "objectPostProcessor",
                        "configure",
                        "webSecurity"
                    ]
                },
                "policyDocumentService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyDocumentService$$EnhancerBySpringCGLIB$$c66f0936",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyDocumentService.class]",
                    "dependencies": [
                        "policyDocumentRepository",
                        "s3UploadService",
                        "policyService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.web.tomcat.TomcatMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.web.tomcat.TomcatMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.mvc-org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties",
                    "resource": null,
                    "dependencies": []
                },
                "configurationPropertiesReportEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.context.properties.ConfigurationPropertiesReportEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/context/properties/ConfigurationPropertiesReportEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointAutoConfiguration",
                        "management.endpoint.configprops-org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointProperties"
                    ]
                },
                "sentryOptionsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$$Lambda$512/0x00000008005c1c40",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration",
                        "contextTagsEventProcessor",
                        "inAppPackagesResolver"
                    ]
                },
                "carrierCommission": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.api.CarrierCommission",
                    "resource": "com.coverdash.crud_service.CrudServiceApplication",
                    "dependencies": [
                        "crudServiceApplication"
                    ]
                },
                "virtualCardService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.VirtualCardService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/VirtualCardService.class]",
                    "dependencies": [
                        "virtualCardRepository"
                    ]
                },
                "operationBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.OperationService",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "parameterBuilder",
                        "requestBodyBuilder",
                        "securityParser",
                        "propertyResolverUtils"
                    ]
                },
                "trustedChoiceControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.TrustedChoiceControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/TrustedChoiceControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "ncciClassService",
                        "businessService",
                        "userService",
                        "addressService",
                        "businessLocationService",
                        "generalClassificationInformationService",
                        "licenseService",
                        "businessClassificationService",
                        "closeService",
                        "zipCodeLookupService",
                        "coverdashUserUtil",
                        "warmTransferService"
                    ]
                },
                "slackLeadRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.SlackLeadRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.SlackLeadRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#2e29a193",
                        "(inner bean)#81847c4",
                        "(inner bean)#26a4b864",
                        "jpaMappingContext"
                    ]
                },
                "webMvcMetricsFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.FilterRegistrationBean",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/servlet/WebMvcMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration",
                        "simpleMeterRegistry",
                        "webMvcTagsProvider"
                    ]
                },
                "accountingController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.AccountingController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/AccountingController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "policyService",
                        "policyTransactionService",
                        "s3UploadService",
                        "accountingService"
                    ]
                },
                "pageableResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.web.PageableHandlerMethodArgumentResolver",
                    "resource": "class path resource [org/springframework/data/web/config/SpringDataWebConfiguration.class]",
                    "dependencies": [
                        "org.springframework.data.web.config.SpringDataWebConfiguration"
                    ]
                },
                "handlerFunctionAdapter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.function.support.HandlerFunctionAdapter",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "localeResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.i18n.AcceptHeaderLocaleResolver",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "schemaPropertyDeprecatingConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.SchemaPropertyDeprecatingConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration$SameManagementContextConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration$SameManagementContextConfiguration",
                    "resource": null,
                    "dependencies": [
                        "environment"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.NamedParameterJdbcTemplateConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.NamedParameterJdbcTemplateConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "applicationSubmissionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ApplicationSubmissionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ApplicationSubmissionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#d11c8fa",
                        "(inner bean)#4df0be5e",
                        "(inner bean)#45fc4c95",
                        "jpaMappingContext"
                    ]
                },
                "spring.transaction-org.springframework.boot.autoconfigure.transaction.TransactionProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.TransactionProperties",
                    "resource": null,
                    "dependencies": []
                },
                "sentryLogbackInitializer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryLogbackInitializer",
                    "resource": "class path resource [io/sentry/spring/boot/SentryLogbackAppenderAutoConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryLogbackAppenderAutoConfiguration",
                        "sentry-io.sentry.spring.boot.SentryProperties"
                    ]
                },
                "jvmHeapPressureMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.jvm.JvmHeapPressureMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/JvmMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "server-org.springframework.boot.autoconfigure.web.ServerProperties"
                    ]
                },
                "jpaVendorAdapter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.orm.jpa.vendor.HibernateJpaVendorAdapter",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/orm/jpa/HibernateJpaConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaConfiguration"
                    ]
                },
                "campaignStatusHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CampaignStatusHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CampaignStatusHistoryService.class]",
                    "dependencies": [
                        "campaignStatusHistoryRepository"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.info.InfoEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.info.InfoEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "loopsService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LoopsService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LoopsService.class]",
                    "dependencies": [
                        "properties",
                        "loopsHistoryService",
                        "licenseService",
                        "employeeContactInformationService"
                    ]
                },
                "jacksonGeoModule": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.geo.GeoModule",
                    "resource": "class path resource [org/springframework/data/web/config/SpringDataJacksonConfiguration.class]",
                    "dependencies": [
                        "org.springframework.data.web.config.SpringDataJacksonConfiguration"
                    ]
                },
                "recommendedPolicyService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RecommendedPolicyService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RecommendedPolicyService.class]",
                    "dependencies": [
                        "recommendedPolicyRepository"
                    ]
                },
                "mvcContentNegotiationManager": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.accept.ContentNegotiationManager",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "configure": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.web.DefaultSecurityFilterChain",
                    "resource": "class path resource [com/coverdash/crud_service/oauthSetup/WebSecurityConfig.class]",
                    "dependencies": [
                        "webSecurityConfig",
                        "org.springframework.security.config.annotation.web.configuration.HttpSecurityConfiguration.httpSecurity",
                        "corsFilter"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.CompositeMeterRegistryAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.CompositeMeterRegistryAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "ncciClassRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.NcciClassRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.NcciClassRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#db70c9b",
                        "(inner bean)#a0bbbed",
                        "(inner bean)#3989e022",
                        "jpaMappingContext"
                    ]
                },
                "io.sentry.spring.tracing.SentryAdviceConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.tracing.SentryAdviceConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$HikariDataSourceMetricsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$HikariDataSourceMetricsConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.task.TaskSchedulingAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.task.TaskSchedulingAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "braintreeController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.BraintreeController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/BraintreeController.class]",
                    "dependencies": [
                        "operationsService",
                        "braintreeGateway",
                        "webhookHistoryService"
                    ]
                },
                "httpRequestHandlerAdapter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.mvc.HttpRequestHandlerAdapter",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "org.springdoc.core.SwaggerUiConfigProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SwaggerUiConfigProperties",
                    "resource": null,
                    "dependencies": []
                },
                "spring.servlet.multipart-org.springframework.boot.autoconfigure.web.servlet.MultipartProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.MultipartProperties",
                    "resource": null,
                    "dependencies": []
                },
                "saleController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.SaleController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/SaleController.class]",
                    "dependencies": [
                        "validationHelper",
                        "quoteService",
                        "saleAnnouncementService",
                        "saleService",
                        "policyService",
                        "licenseService",
                        "userService",
                        "carrierService",
                        "adminAppUserUtil",
                        "employeeContactInformationService",
                        "closeService",
                        "businessService",
                        "asyncDocumentIngestionService"
                    ]
                },
                "tivlyService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TivlyService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TivlyService.class]",
                    "dependencies": [
                        "properties",
                        "applicationSubmissionService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleMetricsExportAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleMetricsExportAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalLifeCycleSLARepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalLifeCycleSLARepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalLifeCycleSLARepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#27bace1f",
                        "(inner bean)#7fd68450",
                        "(inner bean)#60285daa",
                        "jpaMappingContext"
                    ]
                },
                "propertyResolverUtils": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.PropertyResolverUtils",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "org.springframework.beans.factory.support.DefaultListableBeanFactory@c0b41d6",
                        "messageSource",
                        "org.springdoc.core.SpringDocConfigProperties"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceJmxConfiguration$Hikari": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceJmxConfiguration$Hikari",
                    "resource": null,
                    "dependencies": [
                        "dataSource"
                    ]
                },
                "ownerOfficer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.api.OwnerOfficer",
                    "resource": "com.coverdash.crud_service.CrudServiceApplication",
                    "dependencies": [
                        "crudServiceApplication"
                    ]
                },
                "agencyStatService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgencyStatService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgencyStatService.class]",
                    "dependencies": [
                        "agencyStatRepository"
                    ]
                },
                "cachesEndpointWebExtension": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.cache.CachesEndpointWebExtension",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/cache/CachesEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.cache.CachesEndpointAutoConfiguration",
                        "cachesEndpoint"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.lifecycle-org.springframework.boot.autoconfigure.context.LifecycleProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.context.LifecycleProperties",
                    "resource": null,
                    "dependencies": []
                },
                "techFeeEligibilityService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TechFeeEligibilityService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TechFeeEligibilityService.class]",
                    "dependencies": [
                        "techFeeEligibilityRepository"
                    ]
                },
                "s3UploadController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.S3UploadController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/S3UploadController.class]",
                    "dependencies": [
                        "validationHelper",
                        "s3UploadService",
                        "policyDocumentService",
                        "properties"
                    ]
                },
                "healthContributorRegistry": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.AutoConfiguredHealthContributorRegistry",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c",
                        "healthEndpointGroups",
                        "diskSpaceHealthIndicator",
                        "pingHealthContributor",
                        "dbHealthContributor"
                    ]
                },
                "paymentService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PaymentService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PaymentService.class]",
                    "dependencies": [
                        "paymentRepository"
                    ]
                },
                "webhookHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.WebhookHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.WebhookHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#20099dbd",
                        "(inner bean)#2f0c2b93",
                        "(inner bean)#32272d0b",
                        "jpaMappingContext"
                    ]
                },
                "savvyCalControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.SavvyCalControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/SavvyCalControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "renewalBatchService",
                        "userService",
                        "businessService",
                        "employeeContactInformationService",
                        "closeService",
                        "renewalsService"
                    ]
                },
                "responseSupportConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.ResponseSupportConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "userController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.UserController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/UserController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "businessInviteService",
                        "userService",
                        "businessService",
                        "applicationSubmissionService",
                        "addressService",
                        "generalClassificationInformationService",
                        "businessLocationService",
                        "activityService",
                        "closeService",
                        "emailHistoryService",
                        "noteService",
                        "adminAppService",
                        "partnerUserUtil",
                        "coverdashUserUtil"
                    ]
                },
                "propertiesMeterFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.PropertiesMeterFilter",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/MetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration",
                        "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties"
                    ]
                },
                "licenseThemeRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LicenseThemeRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LicenseThemeRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#14cb3b20",
                        "(inner bean)#d9b664f",
                        "(inner bean)#23c8dd5a",
                        "jpaMappingContext"
                    ]
                },
                "quoteComponentControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.QuoteComponentControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/QuoteComponentControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "s3UploadService",
                        "applicationSubmissionService",
                        "hybridApplicationInProgressService",
                        "policyTypeService",
                        "businessService",
                        "closeService",
                        "slackLeadService",
                        "customCoverageElementService",
                        "quoteService",
                        "quotingPageService"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.client.RestTemplateAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.client.RestTemplateAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "hybridApplicationInProgressService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.HybridApplicationInProgressService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/HybridApplicationInProgressService.class]",
                    "dependencies": [
                        "hybridApplicationInProgressRepository"
                    ]
                },
                "noticeOfCancellationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.NoticeOfCancellationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/NoticeOfCancellationService.class]",
                    "dependencies": [
                        "noticeOfCancellationRepository"
                    ]
                },
                "ringbaService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RingbaService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RingbaService.class]",
                    "dependencies": [
                        "properties",
                        "employeeContactInformationService",
                        "ringbaCampaignWeightService"
                    ]
                },
                "partnerTechnologyFeeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerTechnologyFeeService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerTechnologyFeeService.class]",
                    "dependencies": [
                        "partnerTechnologyFeeRepository"
                    ]
                },
                "diskSpaceMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.system.DiskSpaceMetricsBinder",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/SystemMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.SystemMetricsAutoConfiguration",
                        "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties"
                    ]
                },
                "slackControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.SlackControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/SlackControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "intercomMonitoringScheduleService"
                    ]
                },
                "policyNoteService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyNoteService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyNoteService.class]",
                    "dependencies": [
                        "policyNoteRepository"
                    ]
                },
                "adminAppUserUtil": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.components.AdminAppUserUtil",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/components/AdminAppUserUtil.class]",
                    "dependencies": [
                        "employeeContactInformationService",
                        "auth0HttpClient",
                        "auth0AdminTokenManager"
                    ]
                },
                "agentStatusHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentStatusHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentStatusHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#494b20a4",
                        "(inner bean)#3a2b797",
                        "(inner bean)#3f8d1391",
                        "jpaMappingContext"
                    ]
                },
                "customFormFieldRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CustomFormFieldRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CustomFormFieldRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6ed5c449",
                        "(inner bean)#61bd6c16",
                        "(inner bean)#337b9526",
                        "jpaMappingContext"
                    ]
                },
                "accountManagerStatService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AccountManagerStatService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AccountManagerStatService.class]",
                    "dependencies": [
                        "accountManagerStatRepository"
                    ]
                },
                "emBeanDefinitionRegistrarPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.jpa.repository.support.EntityManagerBeanDefinitionRegistrarPostProcessor",
                    "resource": null,
                    "dependencies": []
                },
                "cohortRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CohortRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CohortRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5475de4",
                        "(inner bean)#2ae34d2a",
                        "(inner bean)#774ca718",
                        "jpaMappingContext"
                    ]
                },
                "privilegeEvaluator": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.web.access.RequestMatcherDelegatingWebInvocationPrivilegeEvaluator",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/WebSecurityConfiguration.class]",
                    "dependencies": [
                        "springSecurityFilterChain",
                        "org.springframework.security.config.annotation.web.configuration.WebSecurityConfiguration"
                    ]
                },
                "partnerPaymentController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.PartnerPaymentController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/PartnerPaymentController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "partnerPaymentStructureService",
                        "partnerPaymentService",
                        "licenseService"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration$PooledDataSourceConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration$PooledDataSourceConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "openApiResource": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.api.OpenApiWebMvcResource",
                    "resource": "class path resource [org/springdoc/webmvc/core/SpringDocWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration",
                        "requestBuilder",
                        "responseBuilder",
                        "operationBuilder",
                        "org.springdoc.core.SpringDocConfigProperties",
                        "springDocProviders"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.availability.AvailabilityHealthContributorAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.availability.AvailabilityHealthContributorAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration$MvcAdditionalHealthEndpointPathsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration$MvcAdditionalHealthEndpointPathsConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "docIngestionEvaluationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.DocIngestionEvaluationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/DocIngestionEvaluationService.class]",
                    "dependencies": [
                        "promptService",
                        "claudeService",
                        "policyService",
                        "customCoverageElementService"
                    ]
                },
                "chubbUnderwritingQuestionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ChubbUnderwritingQuestionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ChubbUnderwritingQuestionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5e1d2327",
                        "(inner bean)#7f9a762b",
                        "(inner bean)#559dd1ed",
                        "jpaMappingContext"
                    ]
                },
                "dispatcherServlet": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.DispatcherServlet",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/DispatcherServletAutoConfiguration$DispatcherServletConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletConfiguration",
                        "spring.mvc-org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceRestTemplateConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceRestTemplateConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.cloud.aws.autoconfigure.messaging.MessagingAutoConfiguration$SqsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.messaging.MessagingAutoConfiguration$SqsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "leadService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LeadService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LeadService.class]",
                    "dependencies": [
                        "leadRepository"
                    ]
                },
                "springWebProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.core.SpringWebMvcProvider",
                    "resource": "class path resource [org/springdoc/webmvc/core/SpringDocWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.OAuth2ResourceServerOpaqueTokenConfiguration$OpaqueTokenIntrospectionClientConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.oauth2.resource.servlet.OAuth2ResourceServerOpaqueTokenConfiguration$OpaqueTokenIntrospectionClientConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "parameterBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.GenericParameterService",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "propertyResolverUtils",
                        "springDocObjectMapperProvider"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.jdbc.DataSourceHealthContributorAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.jdbc.DataSourceHealthContributorAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "processorMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.system.ProcessorMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/SystemMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.SystemMetricsAutoConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.integration.IntegrationMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.integration.IntegrationMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "partnerExportController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.PartnerExportController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/PartnerExportController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "activityService",
                        "licenseService",
                        "policyService",
                        "closeService",
                        "policyTransactionService",
                        "carrierCommission"
                    ]
                },
                "transactionManager": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.orm.jpa.JpaTransactionManager",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/orm/jpa/HibernateJpaConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaConfiguration"
                    ]
                },
                "lateInvoicePolicyLinkService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LateInvoicePolicyLinkService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LateInvoicePolicyLinkService.class]",
                    "dependencies": [
                        "lateInvoicePolicyLinkRepository"
                    ]
                },
                "errorPageCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$ErrorPageCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration",
                        "dispatcherServletRegistration"
                    ]
                },
                "metricsWebMvcConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration$MetricsWebMvcConfigurer",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/servlet/WebMvcMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration",
                        "simpleMeterRegistry",
                        "webMvcTagsProvider"
                    ]
                },
                "certificateHolderTemplateRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CertificateHolderTemplateRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CertificateHolderTemplateRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4d71d5ab",
                        "(inner bean)#40188fe6",
                        "(inner bean)#2758e4cb",
                        "jpaMappingContext"
                    ]
                },
                "sentrySpanRestTemplateCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentrySpanRestTemplateCustomizer",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryPerformanceRestTemplateConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceRestTemplateConfiguration",
                        "sentryHub"
                    ]
                },
                "standardGsonBuilderCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.gson.GsonAutoConfiguration$StandardGsonBuilderCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/gson/GsonAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.gson.GsonAutoConfiguration",
                        "spring.gson-org.springframework.boot.autoconfigure.gson.GsonProperties"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$DefaultErrorViewResolverConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$DefaultErrorViewResolverConfiguration",
                    "resource": null,
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c",
                        "spring.web-org.springframework.boot.autoconfigure.web.WebProperties"
                    ]
                },
                "closeController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.CloseController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/CloseController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "policyService",
                        "businessService",
                        "closeService",
                        "userService",
                        "leadService",
                        "leadScoringEngineService",
                        "agentOutOfOfficeService",
                        "renewalBatchService",
                        "renewalPolicyService",
                        "renewalsService",
                        "slackLeadService",
                        "renewalChecklistItemService",
                        "webhookHistoryService",
                        "lateInvoiceService",
                        "lateInvoiceTrackerService",
                        "adminAppService",
                        "loopsService",
                        "objectMapper"
                    ]
                },
                "PDFService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PDFService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PDFService.class]",
                    "dependencies": []
                },
                "partnerAPIRequestRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerAPIRequestRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerAPIRequestRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#76fa6d23",
                        "(inner bean)#3152985e",
                        "(inner bean)#6a544178",
                        "jpaMappingContext"
                    ]
                },
                "slackController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.SlackController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/SlackController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "policyService",
                        "closeService",
                        "mondayService",
                        "slackLeadService",
                        "employeeContactInformationService"
                    ]
                },
                "claimAttachmentRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ClaimAttachmentRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ClaimAttachmentRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#52d2053",
                        "(inner bean)#2d5caaf1",
                        "(inner bean)#24170847",
                        "jpaMappingContext"
                    ]
                },
                "viewNameTranslator": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.view.DefaultRequestToViewNameTranslator",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "polymorphicModelConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.PolymorphicModelConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "subscriptionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.SubscriptionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.SubscriptionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4c77eb54",
                        "(inner bean)#2d683b2d",
                        "(inner bean)#67488c90",
                        "jpaMappingContext"
                    ]
                },
                "dispatcherServletRegistration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletRegistrationBean",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/DispatcherServletAutoConfiguration$DispatcherServletRegistrationConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletRegistrationConfiguration",
                        "dispatcherServlet",
                        "spring.mvc-org.springframework.boot.autoconfigure.web.servlet.WebMvcProperties"
                    ]
                },
                "businessInviteService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.BusinessInviteService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/BusinessInviteService.class]",
                    "dependencies": [
                        "properties",
                        "businessInviteRepository"
                    ]
                },
                "generalClassificationInformationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.GeneralClassificationInformationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/GeneralClassificationInformationService.class]",
                    "dependencies": [
                        "generalClassificationInformationRepository"
                    ]
                },
                "carrierAutoRenewalRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CarrierAutoRenewalRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CarrierAutoRenewalRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#2cf97fb4",
                        "(inner bean)#14e9eace",
                        "(inner bean)#79dd676f",
                        "jpaMappingContext"
                    ]
                },
                "loopsControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.LoopsControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/LoopsControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "policyService",
                        "businessService",
                        "loopsService",
                        "loopsHistoryService",
                        "applicationSubmissionService",
                        "coverdashUserUtil"
                    ]
                },
                "healthEndpointGroupsBeanPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration$HealthEndpointGroupsBeanPostProcessor",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointConfiguration.class]",
                    "dependencies": []
                },
                "validationHelper": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.validation.ValidationHelper",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/validation/ValidationHelper.class]",
                    "dependencies": []
                },
                "tomcatServletWebServerFactory": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.embedded.tomcat.TomcatServletWebServerFactory",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/ServletWebServerFactoryConfiguration$EmbeddedTomcat.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryConfiguration$EmbeddedTomcat"
                    ]
                },
                "helpScoutTicketService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.HelpScoutTicketService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/HelpScoutTicketService.class]",
                    "dependencies": [
                        "helpScoutTicketRepository"
                    ]
                },
                "certificateHolderTemplateService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CertificateHolderTemplateService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CertificateHolderTemplateService.class]",
                    "dependencies": [
                        "certificateHolderTemplateRepository"
                    ]
                },
                "auth0HttpClient": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.components.Auth0HttpClient",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/components/Auth0HttpClient.class]",
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.data.web.SpringDataWebAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.data.web.SpringDataWebAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "spring.data.web-org.springframework.boot.autoconfigure.data.web.SpringDataWebProperties"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceAspectsConfiguration$SentryTransactionPointcutAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryPerformanceAspectsConfiguration$SentryTransactionPointcutAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "jsonMixinModule": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.jackson.JsonMixinModule",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jackson/JacksonAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "braintreeGateway": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.braintreegateway.BraintreeGateway",
                    "resource": "com.coverdash.crud_service.CrudServiceApplication",
                    "dependencies": [
                        "crudServiceApplication",
                        "properties"
                    ]
                },
                "genericReturnTypeParser": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration$1",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration"
                    ]
                },
                "initializeUserDetailsBeanManagerConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.authentication.configuration.InitializeUserDetailsBeanManagerConfigurer",
                    "resource": "class path resource [org/springframework/security/config/annotation/authentication/configuration/AuthenticationConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "webConfig": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.oauthSetup.WebConfig$$EnhancerBySpringCGLIB$$a3db27aa",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/oauthSetup/WebConfig.class]",
                    "dependencies": [
                        "loggerInterceptor",
                        "adminAppUserValidationInterceptor",
                        "fieldValidationInterceptor"
                    ]
                },
                "carrierAutoRenewalService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CarrierAutoRenewalService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CarrierAutoRenewalService.class]",
                    "dependencies": [
                        "carrierAutoRenewalRepository"
                    ]
                },
                "helpscoutController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.HelpscoutController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/HelpscoutController.class]",
                    "dependencies": [
                        "validationHelper",
                        "properties",
                        "helpscoutService",
                        "adminAppUserUtil",
                        "opsAssignmentWeightService",
                        "employeeContactInformationService",
                        "coiToolServiceUtil",
                        "lateInvoiceService",
                        "s3UploadService",
                        "noticeOfCancellationService",
                        "loopsService",
                        "virtualCardService",
                        "policyDocumentService",
                        "policyService",
                        "userService",
                        "closeService",
                        "businessService"
                    ]
                },
                "servletExposeExcludePropertyEndpointFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.expose.IncludeExcludeEndpointFilter",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/ServletEndpointManagementContextConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration",
                        "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties"
                    ]
                },
                "renewalBillingBatchRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalBillingBatchRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalBillingBatchRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6b19f4b8",
                        "(inner bean)#54bb1786",
                        "(inner bean)#755cc0c9",
                        "jpaMappingContext"
                    ]
                },
                "coverdashUserUtil": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.components.CoverdashUserUtil",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/components/CoverdashUserUtil.class]",
                    "dependencies": [
                        "properties",
                        "auth0HttpClient",
                        "userService",
                        "auth0CoverdashTokenManager",
                        "businessService",
                        "applicationSubmissionService",
                        "activityService",
                        "policyService",
                        "addressService",
                        "businessLocationService",
                        "generalClassificationInformationService"
                    ]
                },
                "leadActivityEntryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LeadActivityEntryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LeadActivityEntryService.class]",
                    "dependencies": [
                        "leadActivityEntryRepository"
                    ]
                },
                "licenseService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LicenseService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LicenseService.class]",
                    "dependencies": [
                        "licenseRepository"
                    ]
                },
                "coverageElementService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CoverageElementService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CoverageElementService.class]",
                    "dependencies": [
                        "coverageElementRepository"
                    ]
                },
                "helpScoutTicketHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.HelpScoutTicketHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/HelpScoutTicketHistoryService.class]",
                    "dependencies": [
                        "helpScoutTicketHistoryRepository"
                    ]
                },
                "transactionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TransactionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TransactionService.class]",
                    "dependencies": [
                        "transactionRepository"
                    ]
                },
                "healthEndpointGroups": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.AutoConfiguredHealthEndpointGroups",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c",
                        "management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties"
                    ]
                },
                "webConversionServiceProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.providers.WebConversionServiceProvider",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration$WebConversionServiceConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration$WebConversionServiceConfiguration"
                    ]
                },
                "recommendedPolicyRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RecommendedPolicyRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RecommendedPolicyRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#62f6f159",
                        "(inner bean)#250f839",
                        "(inner bean)#665cfc03",
                        "jpaMappingContext"
                    ]
                },
                "hikariDataSourceMeterBinder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$HikariDataSourceMetricsConfiguration$HikariDataSourceMeterBinder",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/jdbc/DataSourcePoolMetricsAutoConfiguration$HikariDataSourceMetricsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$HikariDataSourceMetricsConfiguration"
                    ]
                },
                "webEndpointPathMapper": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.MappingWebEndpointPathMapper",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration"
                    ]
                },
                "agencyStatsControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.AgencyStatsControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/AgencyStatsControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "adminAppService",
                        "policyService",
                        "policyTransactionService",
                        "agencyStatService",
                        "metricsService",
                        "employeeContactInformationService",
                        "carrierService"
                    ]
                },
                "org.springframework.cloud.aws.messaging.config.annotation.SnsWebConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.messaging.config.annotation.SnsWebConfiguration",
                    "resource": null,
                    "dependencies": [
                        "amazonSNS"
                    ]
                },
                "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaConfiguration",
                    "resource": null,
                    "dependencies": [
                        "dataSource",
                        "spring.jpa-org.springframework.boot.autoconfigure.orm.jpa.JpaProperties",
                        "org.springframework.beans.factory.support.DefaultListableBeanFactory@c0b41d6",
                        "spring.jpa.hibernate-org.springframework.boot.autoconfigure.orm.jpa.HibernateProperties"
                    ]
                },
                "org.springframework.boot.autoconfigure.aop.AopAutoConfiguration$AspectJAutoProxyingConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.aop.AopAutoConfiguration$AspectJAutoProxyingConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$EnableTransactionManagementConfiguration$CglibAutoProxyConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$EnableTransactionManagementConfiguration$CglibAutoProxyConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "openEntityManagerInViewInterceptor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.orm.jpa.support.OpenEntityManagerInViewInterceptor",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/orm/jpa/JpaBaseConfiguration$JpaWebConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.orm.jpa.JpaBaseConfiguration$JpaWebConfiguration"
                    ]
                },
                "reconcileCoterieDataService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.ReconcileCoterieDataService$$EnhancerBySpringCGLIB$$70f3823d",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/ReconcileCoterieDataService.class]",
                    "dependencies": [
                        "webhookHistoryService",
                        "helpscoutService",
                        "policyService"
                    ]
                },
                "coiToolServiceUtil": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.components.CoiToolServiceUtil",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/components/CoiToolServiceUtil.class]",
                    "dependencies": [
                        "properties",
                        "businessLocationService",
                        "customCoverageElementService",
                        "certificateOfInsuranceService",
                        "policyTypeService",
                        "helpscoutService",
                        "coiPolicyLinkService"
                    ]
                },
                "partnerDashboardApiHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerDashboardApiHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerDashboardApiHistoryService.class]",
                    "dependencies": [
                        "partnerDashboardApiHistoryRepository"
                    ]
                },
                "userService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.UserService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/UserService.class]",
                    "dependencies": [
                        "userRepository"
                    ]
                },
                "tomcatServletWebServerFactoryCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.TomcatServletWebServerFactoryCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/ServletWebServerFactoryAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryAutoConfiguration",
                        "server-org.springframework.boot.autoconfigure.web.ServerProperties"
                    ]
                },
                "quoteComponentController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.QuoteComponentController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/QuoteComponentController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "closeService",
                        "startupIndustryService",
                        "slackLeadService",
                        "mondayService",
                        "activityService",
                        "applicationSubmissionService",
                        "businessService",
                        "addressService",
                        "generalClassificationInformationService",
                        "businessLocationService",
                        "userService",
                        "businessClassificationService",
                        "ncciClassService",
                        "quoteService",
                        "licenseService",
                        "tooltipService",
                        "leadService",
                        "leadScoringEngineService",
                        "agentOutOfOfficeService"
                    ]
                },
                "adminAppExportService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.AdminAppExportService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/AdminAppExportService.class]",
                    "dependencies": [
                        "properties",
                        "adminAppService",
                        "partnerPaymentStructureService",
                        "partnerPaymentsUtil"
                    ]
                },
                "renewalLifeCycleSLAService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalLifeCycleSLAService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalLifeCycleSLAService.class]",
                    "dependencies": [
                        "renewalLifeCycleSLARepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.sql.init.SqlInitializationAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.sql.init.SqlInitializationAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "dataSourceScriptDatabaseInitializer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.sql.init.SqlDataSourceScriptDatabaseInitializer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/sql/init/DataSourceInitializationConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.sql.init.DataSourceInitializationConfiguration",
                        "dataSource",
                        "spring.sql.init-org.springframework.boot.autoconfigure.sql.init.SqlInitializationProperties"
                    ]
                },
                "certificateOfInsuranceService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CertificateOfInsuranceService$$EnhancerBySpringCGLIB$$22d86179",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CertificateOfInsuranceService.class]",
                    "dependencies": [
                        "certificateOfInsuranceRepository"
                    ]
                },
                "carrierCommissionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CarrierCommissionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CarrierCommissionService.class]",
                    "dependencies": []
                },
                "meterRegistryPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.MeterRegistryPostProcessor",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/MetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "partnerController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.PartnerController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/PartnerController.class]",
                    "dependencies": [
                        "validationHelper",
                        "partnerService",
                        "licenseService",
                        "licenseThemeService"
                    ]
                },
                "endpointMediaTypes": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.EndpointMediaTypes",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "reductoService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ReductoService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ReductoService.class]",
                    "dependencies": [
                        "promptService",
                        "properties",
                        "carrierService",
                        "objectMapper",
                        "docIngestionAISubmissionService",
                        "docIngestionAISubmissionSuggestionService"
                    ]
                },
                "repositoryTagsProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.data.DefaultRepositoryTagsProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/data/RepositoryMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.data.RepositoryMetricsAutoConfiguration"
                    ]
                },
                "spring.security.oauth2.resourceserver-org.springframework.boot.autoconfigure.security.oauth2.resource.OAuth2ResourceServerProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.oauth2.resource.OAuth2ResourceServerProperties",
                    "resource": null,
                    "dependencies": []
                },
                "dbHealthContributor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.jdbc.DataSourceHealthIndicator",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/jdbc/DataSourceHealthContributorAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.jdbc.DataSourceHealthContributorAutoConfiguration",
                        "dataSource",
                        "management.health.db-org.springframework.boot.actuate.autoconfigure.jdbc.DataSourceHealthIndicatorProperties"
                    ]
                },
                "dataSourcePoolMetadataMeterBinder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$DataSourcePoolMetadataMetricsConfiguration$DataSourcePoolMetadataMeterBinder",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/jdbc/DataSourcePoolMetricsAutoConfiguration$DataSourcePoolMetadataMetricsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$DataSourcePoolMetadataMetricsConfiguration",
                        "dataSource"
                    ]
                },
                "adminAppUserValidationInterceptor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.oauthSetup.AdminAppUserValidationInterceptor",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/oauthSetup/AdminAppUserValidationInterceptor.class]",
                    "dependencies": [
                        "validationHelper",
                        "adminAppUserUtil"
                    ]
                },
                "leadActivityEntryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LeadActivityEntryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LeadActivityEntryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6754608e",
                        "(inner bean)#3deec5a0",
                        "(inner bean)#5a28827e",
                        "jpaMappingContext"
                    ]
                },
                "webServerFactoryCustomizerBeanPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.server.WebServerFactoryCustomizerBeanPostProcessor",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "controllerEndpointHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.servlet.ControllerEndpointHandlerMapping",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/servlet/WebMvcEndpointManagementContextConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.servlet.WebMvcEndpointManagementContextConfiguration",
                        "controllerEndpointDiscoverer",
                        "management.endpoints.web.cors-org.springframework.boot.actuate.autoconfigure.endpoint.web.CorsEndpointProperties",
                        "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.management.ThreadDumpEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.management.ThreadDumpEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "startupIndustryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.StartupIndustryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/StartupIndustryService.class]",
                    "dependencies": [
                        "startupIndustryRepository"
                    ]
                },
                "saleRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.SaleRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.SaleRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#735666c4",
                        "(inner bean)#4eddb903",
                        "(inner bean)#648cfdc8",
                        "jpaMappingContext"
                    ]
                },
                "soldBusinessRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.SoldBusinessRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.SoldBusinessRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6a32569b",
                        "(inner bean)#d2527b5",
                        "(inner bean)#4c841ccb",
                        "jpaMappingContext"
                    ]
                },
                "sentryUserFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.FilterRegistrationBean",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration",
                        "sentryHub",
                        "sentry-io.sentry.spring.boot.SentryProperties",
                        "springSecuritySentryUserProvider",
                        "httpServletRequestSentryUserProvider"
                    ]
                },
                "io.sentry.spring.boot.SentryLogbackAppenderAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryLogbackAppenderAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "environmentEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.env.EnvironmentEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/env/EnvironmentEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointAutoConfiguration",
                        "environment",
                        "management.endpoint.env-org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointProperties"
                    ]
                },
                "conventionErrorViewResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.DefaultErrorViewResolver",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration$DefaultErrorViewResolverConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$DefaultErrorViewResolverConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.LogbackMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.LogbackMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalFormService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalFormService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalFormService.class]",
                    "dependencies": [
                        "renewalFormRepository"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.logging.LoggersEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.logging.LoggersEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "formService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.FormService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/FormService.class]",
                    "dependencies": [
                        "businessService",
                        "customFormFieldService",
                        "userService",
                        "addressService",
                        "businessLocationService",
                        "renewalFormService",
                        "renewalFormFieldService"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration$WebSecurityEnablerConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration$WebSecurityEnablerConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "hiscoxUnderwritingQuestionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.HiscoxUnderwritingQuestionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/HiscoxUnderwritingQuestionService.class]",
                    "dependencies": [
                        "hiscoxUnderwritingQuestionRepository"
                    ]
                },
                "claimService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ClaimService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ClaimService.class]",
                    "dependencies": [
                        "claimRepository"
                    ]
                },
                "jacksonObjectMapperBuilder": {
                    "aliases": [],
                    "scope": "prototype",
                    "type": "org.springframework.http.converter.json.Jackson2ObjectMapperBuilder",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jackson/JacksonAutoConfiguration$JacksonObjectMapperBuilderConfiguration.class]",
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.dao.PersistenceExceptionTranslationAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.dao.PersistenceExceptionTranslationAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "saleService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.SaleService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/SaleService.class]",
                    "dependencies": [
                        "saleRepository"
                    ]
                },
                "crudServiceApplication": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.CrudServiceApplication$$EnhancerBySpringCGLIB$$1dcb6995",
                    "resource": null,
                    "dependencies": [
                        "jdbcTemplate"
                    ]
                },
                "cachedBodyFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.filters.CachedBodyFilter",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/filters/CachedBodyFilter.class]",
                    "dependencies": []
                },
                "corsFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.filter.CorsFilter",
                    "resource": "class path resource [com/coverdash/crud_service/oauthSetup/WebSecurityConfig.class]",
                    "dependencies": [
                        "webSecurityConfig"
                    ]
                },
                "multipartResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.multipart.support.StandardServletMultipartResolver",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/MultipartAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration"
                    ]
                },
                "renewalLifeCycleService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalLifeCycleService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalLifeCycleService.class]",
                    "dependencies": [
                        "renewalLifeCycleRepository"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration$WebEndpointServletConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration$WebEndpointServletConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "requestMappingHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcContentNegotiationManager",
                        "mvcConversionService",
                        "mvcResourceUrlProvider"
                    ]
                },
                "webExposeExcludePropertyEndpointFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.expose.IncludeExcludeEndpointFilter",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration"
                    ]
                },
                "paymentPlanRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PaymentPlanRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PaymentPlanRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5bd9bb05",
                        "(inner bean)#6d881fec",
                        "(inner bean)#629f2844",
                        "jpaMappingContext"
                    ]
                },
                "requestMappingHandlerAdapter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerAdapter",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcContentNegotiationManager",
                        "mvcConversionService",
                        "mvcValidator"
                    ]
                },
                "tomcatMetricsBinder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.web.tomcat.TomcatMetricsBinder",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/tomcat/TomcatMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.tomcat.TomcatMetricsAutoConfiguration",
                        "simpleMeterRegistry"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$DataSourcePoolMetadataMetricsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.jdbc.DataSourcePoolMetricsAutoConfiguration$DataSourcePoolMetadataMetricsConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "leadScoringEngineService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LeadScoringEngineService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LeadScoringEngineService.class]",
                    "dependencies": [
                        "properties",
                        "leadService",
                        "agentLeadRuleService",
                        "agentScoreService",
                        "applicationSubmissionService",
                        "leadActivityEntryService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration$WebMvcServletEndpointManagementContextConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration$WebMvcServletEndpointManagementContextConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "docIngestionAISubmissionSuggestionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.DocIngestionAISubmissionSuggestionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.DocIngestionAISubmissionSuggestionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1d21033e",
                        "(inner bean)#899d0e",
                        "(inner bean)#78546c38",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.context.LifecycleAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.context.LifecycleAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.logging.LogFileWebEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.logging.LogFileWebEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.info-org.springframework.boot.autoconfigure.info.ProjectInfoProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.info.ProjectInfoProperties",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceTransactionManagerAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceTransactionManagerAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "formPageController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.FormPageController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/FormPageController.class]",
                    "dependencies": [
                        "applicationSubmissionService",
                        "businessLocationService",
                        "generalClassificationInformationService",
                        "addressService",
                        "ncciClassService",
                        "businessService",
                        "coverageService",
                        "hybridApplicationInProgressService",
                        "formPageService",
                        "closeService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.MetricsEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.MetricsEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "infoEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.info.InfoEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/info/InfoEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.info.InfoEndpointAutoConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceTransactionManagerAutoConfiguration$JdbcTransactionManagerConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceTransactionManagerAutoConfiguration$JdbcTransactionManagerConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "chubbUnderwritingQuestionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ChubbUnderwritingQuestionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ChubbUnderwritingQuestionService.class]",
                    "dependencies": [
                        "chubbUnderwritingQuestionRepository"
                    ]
                },
                "metricsRepositoryMethodInvocationListenerBeanPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.data.MetricsRepositoryMethodInvocationListenerBeanPostProcessor",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/data/RepositoryMetricsAutoConfiguration.class]",
                    "dependencies": []
                },
                "applicationSubmissionBatchService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ApplicationSubmissionBatchService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ApplicationSubmissionBatchService.class]",
                    "dependencies": [
                        "applicationSubmissionBatchRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.security.servlet.SecurityAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.servlet.SecurityAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "cnaUnderwritingAttestationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CnaUnderwritingAttestationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CnaUnderwritingAttestationService.class]",
                    "dependencies": [
                        "cnaUnderwritingAttestationRepository"
                    ]
                },
                "classLoaderMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.jvm.ClassLoaderMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/JvmMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration"
                    ]
                },
                "org.springframework.security.config.annotation.web.configuration.WebMvcSecurityConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.web.configuration.WebMvcSecurityConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.internalCachingMetadataReaderFactory": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.core.type.classreading.CachingMetadataReaderFactory",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$ParameterNamesModuleConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$ParameterNamesModuleConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "sortResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.web.SortHandlerMethodArgumentResolver",
                    "resource": "class path resource [org/springframework/data/web/config/SpringDataWebConfiguration.class]",
                    "dependencies": [
                        "org.springframework.data.web.config.SpringDataWebConfiguration"
                    ]
                },
                "hybridApplicationInProgressRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.HybridApplicationInProgressRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.HybridApplicationInProgressRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#2a5ae8d4",
                        "(inner bean)#454f2ac7",
                        "(inner bean)#5e50461f",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.sql.init.DataSourceInitializationConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.sql.init.DataSourceInitializationConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.audit.AuditEventsEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.audit.AuditEventsEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "errorAttributes": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.error.DefaultErrorAttributes",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration"
                    ]
                },
                "slackNotificationUtil": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.util.SlackNotificationUtil",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/util/SlackNotificationUtil.class]",
                    "dependencies": [
                        "properties"
                    ]
                },
                "agentOutOfOfficeRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentOutOfOfficeRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentOutOfOfficeRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#7d538a7a",
                        "(inner bean)#17640714",
                        "(inner bean)#2a3cdf2b",
                        "jpaMappingContext"
                    ]
                },
                "agentLeadRuleRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentLeadRuleRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentLeadRuleRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1b89b1ac",
                        "(inner bean)#3cf48234",
                        "(inner bean)#2c9a4791",
                        "jpaMappingContext"
                    ]
                },
                "beanNameHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.handler.BeanNameUrlHandlerMapping",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcConversionService",
                        "mvcResourceUrlProvider"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springdoc.core.SpringDocConfiguration$SpringDocSpringDataWebPropertiesProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration$SpringDocSpringDataWebPropertiesProvider",
                    "resource": null,
                    "dependencies": []
                },
                "zipCodeLookupService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ZipCodeLookupService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ZipCodeLookupService.class]",
                    "dependencies": [
                        "zipCodeLookupRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.DataSourceConfiguration$Hikari": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceConfiguration$Hikari",
                    "resource": null,
                    "dependencies": []
                },
                "springDataWebPropertiesProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.providers.SpringDataWebPropertiesProvider",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration$SpringDocSpringDataWebPropertiesProvider.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration$SpringDocSpringDataWebPropertiesProvider"
                    ]
                },
                "cnaUnderwritingQuestionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CnaUnderwritingQuestionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CnaUnderwritingQuestionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#13d4bf8",
                        "(inner bean)#2e4ebad5",
                        "(inner bean)#577981ca",
                        "jpaMappingContext"
                    ]
                },
                "customerTouchPointService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.touchpoints.CustomerTouchPointService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/touchpoints/CustomerTouchPointService.class]",
                    "dependencies": [
                        "policyService",
                        "closeService",
                        "businessService",
                        "loopsService"
                    ]
                },
                "renewalSLAEvaluationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.renewals.RenewalSLAEvaluationService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/renewals/RenewalSLAEvaluationService.class]",
                    "dependencies": [
                        "renewalLifeCycleSLAService",
                        "renewalCarrierSLAService",
                        "renewalLifeCycleService",
                        "renewalBatchService",
                        "closeService",
                        "properties"
                    ]
                },
                "accountExecutiveStatRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AccountExecutiveStatRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AccountExecutiveStatRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5585f547",
                        "(inner bean)#515432cb",
                        "(inner bean)#41bd7cb1",
                        "jpaMappingContext"
                    ]
                },
                "partnerPaymentStructureService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerPaymentStructureService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerPaymentStructureService.class]",
                    "dependencies": [
                        "partnerPaymentStructureRepository"
                    ]
                },
                "auth0PartnerTokenManager": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.tokenManagers.Auth0PartnerTokenManager",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/tokenManagers/Auth0PartnerTokenManager.class]",
                    "dependencies": [
                        "auth0HttpClient"
                    ]
                },
                "lateInvoiceTrackerController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.LateInvoiceTrackerController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/LateInvoiceTrackerController.class]",
                    "dependencies": [
                        "validationHelper",
                        "policyService",
                        "lateInvoiceService",
                        "lateInvoicePolicyLinkService",
                        "lateInvoiceTrackerService",
                        "adminAppUserUtil"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.security.servlet.SecurityRequestMatchersManagementContextConfiguration$MvcRequestMatcherConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.security.servlet.SecurityRequestMatchersManagementContextConfiguration$MvcRequestMatcherConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "agentScoreRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentScoreRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentScoreRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1000dbea",
                        "(inner bean)#59e182",
                        "(inner bean)#52aac6ff",
                        "jpaMappingContext"
                    ]
                },
                "ecommerceClassificationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.EcommerceClassificationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.EcommerceClassificationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#44b3c545",
                        "(inner bean)#15c5d50e",
                        "(inner bean)#1108694",
                        "jpaMappingContext"
                    ]
                },
                "partnerPaymentService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerPaymentService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerPaymentService.class]",
                    "dependencies": [
                        "partnerPaymentRepository"
                    ]
                },
                "swaggerWelcome": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.ui.SwaggerWelcomeWebMvc",
                    "resource": "class path resource [org/springdoc/webmvc/ui/SwaggerConfig.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.ui.SwaggerConfig",
                        "org.springdoc.core.SwaggerUiConfigProperties",
                        "org.springdoc.core.SpringDocConfigProperties",
                        "org.springdoc.core.SwaggerUiConfigParameters",
                        "springWebProvider"
                    ]
                },
                "flashMapManager": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.support.SessionFlashMapManager",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "requestMatcherProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.security.servlet.AntPathRequestMatcherProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/security/servlet/SecurityRequestMatchersManagementContextConfiguration$MvcRequestMatcherConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.security.servlet.SecurityRequestMatchersManagementContextConfiguration$MvcRequestMatcherConfiguration",
                        "dispatcherServletRegistration"
                    ]
                },
                "licenseRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LicenseRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LicenseRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3a8be13b",
                        "(inner bean)#18c135fa",
                        "(inner bean)#5db07ad9",
                        "jpaMappingContext"
                    ]
                },
                "noteRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.NoteRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.NoteRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1c5c560a",
                        "(inner bean)#3f962128",
                        "(inner bean)#641f5513",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.netty.NettyAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.netty.NettyAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "spring.netty-org.springframework.boot.autoconfigure.netty.NettyProperties"
                    ]
                },
                "healthHttpCodeStatusMapper": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.health.SimpleHttpCodeStatusMapper",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration",
                        "management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties"
                    ]
                },
                "policyTypeRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyTypeRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyTypeRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#18ae9e1b",
                        "(inner bean)#2bc1cc4",
                        "(inner bean)#19b3800e",
                        "jpaMappingContext"
                    ]
                },
                "transactionNameProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.tracing.SpringMvcTransactionNameProvider",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration"
                    ]
                },
                "uptimeMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.system.UptimeMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/SystemMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.SystemMetricsAutoConfiguration"
                    ]
                },
                "controllerExposeExcludePropertyEndpointFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.expose.IncludeExcludeEndpointFilter",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration"
                    ]
                },
                "scheduledTasksEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.scheduling.ScheduledTasksEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/scheduling/ScheduledTasksEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.scheduling.ScheduledTasksEndpointAutoConfiguration"
                    ]
                },
                "indexPageTransformer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.ui.SwaggerIndexPageTransformer",
                    "resource": "class path resource [org/springdoc/webmvc/ui/SwaggerConfig.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.ui.SwaggerConfig",
                        "org.springdoc.core.SwaggerUiConfigProperties",
                        "org.springdoc.core.SwaggerUiOAuthProperties",
                        "org.springdoc.core.SwaggerUiConfigParameters",
                        "swaggerWelcome",
                        "springDocObjectMapperProvider"
                    ]
                },
                "org.springframework.data.web.config.ProjectingArgumentResolverRegistrar": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.web.config.ProjectingArgumentResolverRegistrar",
                    "resource": null,
                    "dependencies": []
                },
                "partnerPaymentRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerPaymentRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerPaymentRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3833da6f",
                        "(inner bean)#4e3ee82f",
                        "(inner bean)#5b6e2a7e",
                        "jpaMappingContext"
                    ]
                },
                "sentrySpanPointcut": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.aop.support.ComposablePointcut",
                    "resource": "class path resource [io/sentry/spring/tracing/SentrySpanPointcutConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.tracing.SentrySpanPointcutConfiguration"
                    ]
                },
                "heapDumpWebEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.management.HeapDumpWebEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/management/HeapDumpWebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.management.HeapDumpWebEndpointAutoConfiguration"
                    ]
                },
                "managementServletContext": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextAutoConfiguration$$Lambda$1376/0x0000000800e18c40",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/web/servlet/ServletManagementContextAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextAutoConfiguration",
                        "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties"
                    ]
                },
                "spring.gson-org.springframework.boot.autoconfigure.gson.GsonProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.gson.GsonProperties",
                    "resource": null,
                    "dependencies": []
                },
                "environmentEndpointWebExtension": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.env.EnvironmentEndpointWebExtension",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/env/EnvironmentEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointAutoConfiguration",
                        "environmentEndpoint"
                    ]
                },
                "certificateOfInsuranceRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CertificateOfInsuranceRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CertificateOfInsuranceRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#460d7e4a",
                        "(inner bean)#21baa851",
                        "(inner bean)#48a28383",
                        "jpaMappingContext"
                    ]
                },
                "mvcValidator": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.validation.beanvalidation.OptionalValidatorFactoryBean",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "awsCredentialsProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.context.properties.AwsCredentialsProperties",
                    "resource": "class path resource [org/springframework/cloud/aws/autoconfigure/context/ContextCredentialsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.cloud.aws.autoconfigure.context.ContextCredentialsAutoConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration$SameManagementContextConfiguration$EnableSameManagementContextConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration$SameManagementContextConfiguration$EnableSameManagementContextConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "accountingService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.AccountingService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/AccountingService.class]",
                    "dependencies": [
                        "accountingUploadService",
                        "policyTransactionService",
                        "policyService",
                        "transactionManagerService",
                        "s3UploadService"
                    ]
                },
                "sentryTransactionPointcut": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.aop.support.ComposablePointcut",
                    "resource": "class path resource [io/sentry/spring/tracing/SentryTransactionPointcutConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.tracing.SentryTransactionPointcutConfiguration"
                    ]
                },
                "intercomMonitoringScheduleService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.IntercomMonitoringScheduleService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/IntercomMonitoringScheduleService.class]",
                    "dependencies": [
                        "intercomMonitoringScheduleRepository"
                    ]
                },
                "zipCodeLookupRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ZipCodeLookupRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ZipCodeLookupRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4d0bbae5",
                        "(inner bean)#1944391c",
                        "(inner bean)#16a81431",
                        "jpaMappingContext"
                    ]
                },
                "dumpEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.management.ThreadDumpEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/management/ThreadDumpEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.management.ThreadDumpEndpointAutoConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.ServletEndpointManagementContextConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "onboardingController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.OnboardingController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/OnboardingController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "adminAppUserUtil",
                        "ringbaService",
                        "agentLeadRuleService",
                        "agentOutOfOfficeService",
                        "agentStatusService",
                        "agentPayoutMetricService",
                        "employeeContactInformationService",
                        "accountManagerPayoutMetricService",
                        "ascendService",
                        "emailHistoryService",
                        "licenseService"
                    ]
                },
                "cohortController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.CohortController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/CohortController.class]",
                    "dependencies": [
                        "validationHelper",
                        "policyService",
                        "businessService",
                        "cohortService"
                    ]
                },
                "policyDocumentRelevantInformationMappingRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyDocumentRelevantInformationMappingRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyDocumentRelevantInformationMappingRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5fc38804",
                        "(inner bean)#c7ae966",
                        "(inner bean)#385c3093",
                        "jpaMappingContext"
                    ]
                },
                "adminAppCustomersController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.AdminAppCustomersController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/AdminAppCustomersController.class]",
                    "dependencies": [
                        "validationHelper",
                        "applicationSubmissionBatchService",
                        "stripeService",
                        "virtualCardService",
                        "braintreeService",
                        "subscriptionService",
                        "adminAppUserUtil",
                        "adminAppCustomersService",
                        "policyService",
                        "employeeContactInformationService",
                        "closeService",
                        "loopsService",
                        "ascendService",
                        "businessService",
                        "tivlyService",
                        "boldPenguinService",
                        "coverdashUserUtil",
                        "policyDocumentService"
                    ]
                },
                "org.springdoc.core.SwaggerUiOAuthProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SwaggerUiOAuthProperties",
                    "resource": null,
                    "dependencies": []
                },
                "hikariPoolDataSourceMetadataProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.metadata.DataSourcePoolMetadataProvidersConfiguration$HikariPoolDataSourceMetadataProviderConfiguration$$Lambda$770/0x00000008006b6c40",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jdbc/metadata/DataSourcePoolMetadataProvidersConfiguration$HikariPoolDataSourceMetadataProviderConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.jdbc.metadata.DataSourcePoolMetadataProvidersConfiguration$HikariPoolDataSourceMetadataProviderConfiguration"
                    ]
                },
                "renewalBatchRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalBatchRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalBatchRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4d5d8bdb",
                        "(inner bean)#6e5b0d3c",
                        "(inner bean)#5b9e7722",
                        "jpaMappingContext"
                    ]
                },
                "agentScoreWeightRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentScoreWeightRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentScoreWeightRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#646759b2",
                        "(inner bean)#1e49f8ca",
                        "(inner bean)#a5810be",
                        "jpaMappingContext"
                    ]
                },
                "excludedCoverageElementRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ExcludedCoverageElementRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ExcludedCoverageElementRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#57567018",
                        "(inner bean)#72558d04",
                        "(inner bean)#2ab42a53",
                        "jpaMappingContext"
                    ]
                },
                "campaignEmployeeDetailsRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CampaignEmployeeDetailsRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CampaignEmployeeDetailsRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#484b250b",
                        "(inner bean)#11de3445",
                        "(inner bean)#2d18085f",
                        "jpaMappingContext"
                    ]
                },
                "s3UploadRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.S3UploadRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.S3UploadRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#222303b9",
                        "(inner bean)#63be584e",
                        "(inner bean)#3eaa23",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.context.PropertyPlaceholderAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.context.PropertyPlaceholderAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.cloud.aws.messaging.config.annotation.SqsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.messaging.config.annotation.SqsConfiguration$$EnhancerBySpringCGLIB$$300ec7a3",
                    "resource": null,
                    "dependencies": [
                        "org.springframework.cloud.aws.core.env.ResourceIdResolver.BEAN_NAME"
                    ]
                },
                "agentStatusHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentStatusHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentStatusHistoryService.class]",
                    "dependencies": [
                        "agentStatusHistoryRepository"
                    ]
                },
                "baseRenewalFormFieldService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.BaseRenewalFormFieldService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/BaseRenewalFormFieldService.class]",
                    "dependencies": [
                        "baseRenewalFormFieldRepository"
                    ]
                },
                "org.springdoc.core.SpringDocConfiguration$WebConversionServiceConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration$WebConversionServiceConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "tivlyControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.TivlyControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/TivlyControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "businessService",
                        "userService",
                        "addressService",
                        "businessLocationService",
                        "licenseService",
                        "businessClassificationService",
                        "closeService",
                        "coverdashUserUtil",
                        "naicsClassificationService",
                        "warmTransferService"
                    ]
                },
                "lateInvoiceRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LateInvoiceRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LateInvoiceRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4c0410a7",
                        "(inner bean)#12e8738",
                        "(inner bean)#5a8424af",
                        "jpaMappingContext"
                    ]
                },
                "diskSpaceHealthIndicator": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.system.DiskSpaceHealthIndicator",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/system/DiskSpaceHealthContributorAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthContributorAutoConfiguration",
                        "management.health.diskspace-org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthIndicatorProperties"
                    ]
                },
                "modelConverterRegistrar": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.ModelConverterRegistrar",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.condition.ConditionsReportEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.condition.ConditionsReportEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "naicsClassificationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.NaicsClassificationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/NaicsClassificationService.class]",
                    "dependencies": [
                        "naicsClassificationRepository"
                    ]
                },
                "handlerExceptionResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.handler.HandlerExceptionResolverComposite",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcContentNegotiationManager"
                    ]
                },
                "saleAnnouncementService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.SaleAnnouncementService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/SaleAnnouncementService.class]",
                    "dependencies": [
                        "closeService",
                        "saleService",
                        "helpscoutService",
                        "loopsService",
                        "slackNotificationUtil",
                        "virtualCardService"
                    ]
                },
                "org.springframework.cloud.aws.messaging.config.annotation.SnsConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.messaging.config.annotation.SnsConfiguration",
                    "resource": null,
                    "dependencies": [
                        "credentialsProvider",
                        "org.springframework.cloud.aws.core.region.RegionProvider.BEAN_NAME"
                    ]
                },
                "basicErrorController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.BasicErrorController",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration",
                        "errorAttributes"
                    ]
                },
                "mappingsEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.web.mappings.MappingsEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/web/mappings/MappingsEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "sortOpenAPIConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.SortOpenAPIConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration$SpringDocSortConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration$SpringDocSortConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "opsAssignmentWeightService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.OpsAssignmentWeightService$$EnhancerBySpringCGLIB$$c8120776",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/OpsAssignmentWeightService.class]",
                    "dependencies": [
                        "opsAssignmentWeightRepository"
                    ]
                },
                "claimRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ClaimRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ClaimRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#28533a9a",
                        "(inner bean)#21247135",
                        "(inner bean)#70573f5f",
                        "jpaMappingContext"
                    ]
                },
                "employeeContactInformationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.EmployeeContactInformationService$$EnhancerBySpringCGLIB$$8c1e524f",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/EmployeeContactInformationService.class]",
                    "dependencies": [
                        "employeeContactInformationRepository"
                    ]
                },
                "AWLControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.AWLControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/AWLControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "businessService",
                        "userService",
                        "addressService",
                        "businessLocationService",
                        "licenseService",
                        "businessClassificationService",
                        "closeService",
                        "coverdashUserUtil",
                        "sic4MappingService",
                        "campaignStatusService",
                        "warmTransferService"
                    ]
                },
                "coverageElementRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CoverageElementRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CoverageElementRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#d0bb60",
                        "(inner bean)#5157d57c",
                        "(inner bean)#b5911b3",
                        "jpaMappingContext"
                    ]
                },
                "spring.datasource-org.springframework.boot.autoconfigure.jdbc.DataSourceProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.DataSourceProperties",
                    "resource": null,
                    "dependencies": []
                },
                "renewalPolicyRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalPolicyRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalPolicyRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4bfe0b18",
                        "(inner bean)#1e4ca02",
                        "(inner bean)#2d3a0c75",
                        "jpaMappingContext"
                    ]
                },
                "braintreeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.BraintreeService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/BraintreeService.class]",
                    "dependencies": [
                        "braintreeGateway",
                        "stripeService",
                        "virtualCardService",
                        "subscriptionService",
                        "policyService",
                        "businessService"
                    ]
                },
                "org.springdoc.core.SpringDocConfiguration$SpringDocSortConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration$SpringDocSortConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalLifeCycleRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalLifeCycleRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalLifeCycleRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4fc454d5",
                        "(inner bean)#463b73e1",
                        "(inner bean)#3f3ed8bc",
                        "jpaMappingContext"
                    ]
                },
                "emailHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.EmailHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/EmailHistoryService.class]",
                    "dependencies": [
                        "emailHistoryRepository"
                    ]
                },
                "mvcViewResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.view.ViewResolverComposite",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcContentNegotiationManager"
                    ]
                },
                "businessLocationService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.BusinessLocationService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/BusinessLocationService.class]",
                    "dependencies": [
                        "businessLocationRepository",
                        "ncciClassService",
                        "generalClassificationInformationService"
                    ]
                },
                "requestDataValueProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.web.servlet.support.csrf.CsrfRequestDataValueProcessor",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/WebMvcSecurityConfiguration.class]",
                    "dependencies": [
                        "org.springframework.security.config.annotation.web.configuration.WebMvcSecurityConfiguration"
                    ]
                },
                "ringbaCampaignWeightRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RingbaCampaignWeightRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RingbaCampaignWeightRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#7461712c",
                        "(inner bean)#3b5ab6fe",
                        "(inner bean)#65498049",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "mvcUriComponentsContributor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.method.support.CompositeUriComponentsContributor",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcConversionService",
                        "requestMappingHandlerAdapter"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration$SentrySecurityConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration$SentrySecurityConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.server.ManagementContextAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "campaignStatusHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CampaignStatusHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CampaignStatusHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#78eb4fee",
                        "(inner bean)#15915959",
                        "(inner bean)#38f964a5",
                        "jpaMappingContext"
                    ]
                },
                "taskExecutorBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.task.TaskExecutorBuilder",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/task/TaskExecutionAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.task.TaskExecutionAutoConfiguration",
                        "spring.task.execution-org.springframework.boot.autoconfigure.task.TaskExecutionProperties"
                    ]
                },
                "securityFilterChainRegistration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.DelegatingFilterProxyRegistrationBean",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/security/servlet/SecurityFilterAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.security.servlet.SecurityFilterAutoConfiguration",
                        "spring.security-org.springframework.boot.autoconfigure.security.SecurityProperties"
                    ]
                },
                "platformTransactionManagerCustomizers": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.transaction.TransactionManagerCustomizers",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/transaction/TransactionAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration"
                    ]
                },
                "accountManagerPayoutMetricService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AccountManagerPayoutMetricService$$EnhancerBySpringCGLIB$$e288f37b",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AccountManagerPayoutMetricService.class]",
                    "dependencies": [
                        "accountManagerPayoutMetricRepository"
                    ]
                },
                "properties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "java.util.Properties",
                    "resource": "com.coverdash.crud_service.CrudServiceApplication",
                    "dependencies": [
                        "crudServiceApplication"
                    ]
                },
                "leadScoreWeightValueRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LeadScoreWeightValueRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LeadScoreWeightValueRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#29c2418",
                        "(inner bean)#1b0f3b5",
                        "(inner bean)#33adb727",
                        "jpaMappingContext"
                    ]
                },
                "helpscoutService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.HelpscoutService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/HelpscoutService.class]",
                    "dependencies": [
                        "properties"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$ContextTagsEventProcessorConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$ContextTagsEventProcessorConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "sic4MappingService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.Sic4MappingService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/Sic4MappingService.class]",
                    "dependencies": [
                        "sic4MappingRepository"
                    ]
                },
                "metricsRestTemplateCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.web.client.MetricsRestTemplateCustomizer",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/client/RestTemplateMetricsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.client.RestTemplateMetricsConfiguration",
                        "simpleMeterRegistry",
                        "restTemplateExchangeTagsProvider",
                        "management.metrics-org.springframework.boot.actuate.autoconfigure.metrics.MetricsProperties"
                    ]
                },
                "characterEncodingFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.filter.OrderedCharacterEncodingFilter",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/HttpEncodingAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.HttpEncodingAutoConfiguration"
                    ]
                },
                "activityRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ActivityRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ActivityRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#e320f5",
                        "(inner bean)#19f926cf",
                        "(inner bean)#182c3b79",
                        "jpaMappingContext"
                    ]
                },
                "docIngestionAISubmissionSuggestionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.DocIngestionAISubmissionSuggestionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/DocIngestionAISubmissionSuggestionService.class]",
                    "dependencies": [
                        "docIngestionAISubmissionSuggestionRepository"
                    ]
                },
                "sortCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.data.web.SpringDataWebAutoConfiguration$$Lambda$1311/0x0000000800d62440",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/data/web/SpringDataWebAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.data.web.SpringDataWebAutoConfiguration"
                    ]
                },
                "webEndpointDiscoverer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.annotation.WebEndpointDiscoverer",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration",
                        "endpointOperationParameterMapper",
                        "endpointMediaTypes"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletRegistrationConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration$DispatcherServletRegistrationConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperBuilderConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperBuilderConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "openAPIBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.OpenAPIService",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "securityParser",
                        "org.springdoc.core.SpringDocConfigProperties",
                        "propertyResolverUtils"
                    ]
                },
                "logbackMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.logging.LogbackMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/LogbackMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.LogbackMetricsAutoConfiguration"
                    ]
                },
                "partnerDashboardApiHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerDashboardApiHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerDashboardApiHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3887479d",
                        "(inner bean)#15ed06d3",
                        "(inner bean)#27b93919",
                        "jpaMappingContext"
                    ]
                },
                "management.info-org.springframework.boot.actuate.autoconfigure.info.InfoContributorProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.info.InfoContributorProperties",
                    "resource": null,
                    "dependencies": []
                },
                "lateInvoiceService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LateInvoiceService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LateInvoiceService.class]",
                    "dependencies": [
                        "lateInvoiceRepository",
                        "lateInvoicePolicyLinkService"
                    ]
                },
                "accountingUploadRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AccountingUploadRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AccountingUploadRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#60fa2204",
                        "(inner bean)#14a7acd8",
                        "(inner bean)#4b378607",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.security.config.annotation.authentication.configuration.AuthenticationConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.authentication.configuration.AuthenticationConfiguration",
                    "resource": null,
                    "dependencies": [
                        "enableGlobalAuthenticationAutowiredConfigurer",
                        "initializeUserDetailsBeanManagerConfigurer",
                        "initializeAuthenticationProviderBeanManagerConfigurer",
                        "objectPostProcessor"
                    ]
                },
                "restTemplateExchangeTagsProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.web.client.DefaultRestTemplateExchangeTagsProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/client/RestTemplateMetricsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.client.RestTemplateMetricsConfiguration"
                    ]
                },
                "org.springdoc.core.SpringDocConfiguration$OpenApiResourceAdvice": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration$OpenApiResourceAdvice",
                    "resource": null,
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration"
                    ]
                },
                "powerPointController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.PowerPointController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/PowerPointController.class]",
                    "dependencies": [
                        "validationHelper",
                        "powerPointService",
                        "businessService",
                        "renewalBatchService"
                    ]
                },
                "intercomMonitoringScheduleRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.IntercomMonitoringScheduleRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.IntercomMonitoringScheduleRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5b2ebfe5",
                        "(inner bean)#42923ae8",
                        "(inner bean)#52907b1e",
                        "jpaMappingContext"
                    ]
                },
                "management.endpoints.web.cors-org.springframework.boot.actuate.autoconfigure.endpoint.web.CorsEndpointProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.CorsEndpointProperties",
                    "resource": null,
                    "dependencies": []
                },
                "errorPageSecurityFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.web.servlet.FilterRegistrationBean",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/security/servlet/SpringBootWebSecurityConfiguration$ErrorPageSecurityFilterConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.security.servlet.SpringBootWebSecurityConfiguration$ErrorPageSecurityFilterConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "stringHttpMessageConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.http.converter.StringHttpMessageConverter",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/http/HttpMessageConvertersAutoConfiguration$StringHttpMessageConverterConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration$StringHttpMessageConverterConfiguration",
                        "environment"
                    ]
                },
                "policyRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#11ff1c7f",
                        "(inner bean)#28b15698",
                        "(inner bean)#113d2a24",
                        "jpaMappingContext"
                    ]
                },
                "ascendService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AscendService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AscendService.class]",
                    "dependencies": [
                        "objectMapper",
                        "properties",
                        "technologyFeeService",
                        "policyService",
                        "quoteService",
                        "businessService",
                        "carrierCommission"
                    ]
                },
                "carrierQuoteRequestRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CarrierQuoteRequestRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CarrierQuoteRequestRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#107bea33",
                        "(inner bean)#58c92c02",
                        "(inner bean)#78bc7456",
                        "jpaMappingContext"
                    ]
                },
                "jsonComponentModule": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.jackson.JsonComponentModule",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jackson/JacksonAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration"
                    ]
                },
                "quoteRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.QuoteRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.QuoteRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#4a126898",
                        "(inner bean)#7bce4a64",
                        "(inner bean)#43fa82c1",
                        "jpaMappingContext"
                    ]
                },
                "entityManagerFactoryBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.orm.jpa.EntityManagerFactoryBuilder",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/orm/jpa/HibernateJpaConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaConfiguration",
                        "jpaVendorAdapter"
                    ]
                },
                "loopsHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LoopsHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LoopsHistoryService.class]",
                    "dependencies": [
                        "loopsHistoryRepository"
                    ]
                },
                "mappingJackson2HttpMessageConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.http.converter.json.MappingJackson2HttpMessageConverter",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/http/JacksonHttpMessageConvertersConfiguration$MappingJackson2HttpMessageConverterConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration$MappingJackson2HttpMessageConverterConfiguration",
                        "objectMapper"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.env.EnvironmentEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "applicationSubmissionBatchRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.ApplicationSubmissionBatchRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.ApplicationSubmissionBatchRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6ae52aa2",
                        "(inner bean)#58c9a808",
                        "(inner bean)#4226618c",
                        "jpaMappingContext"
                    ]
                },
                "renewalFormRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalFormRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalFormRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#548afb9a",
                        "(inner bean)#41971628",
                        "(inner bean)#6c3921",
                        "jpaMappingContext"
                    ]
                },
                "amazonSNS": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.amazonaws.services.sns.AmazonSNSClient",
                    "resource": "class path resource [org/springframework/cloud/aws/messaging/config/annotation/SnsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.cloud.aws.messaging.config.annotation.SnsConfiguration"
                    ]
                },
                "healthStatusAggregator": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.health.SimpleStatusAggregator",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration",
                        "management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties"
                    ]
                },
                "management.server-org.springframework.boot.actuate.autoconfigure.web.server.ManagementServerProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.server.ManagementServerProperties",
                    "resource": null,
                    "dependencies": []
                },
                "enableGlobalAuthenticationAutowiredConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.authentication.configuration.AuthenticationConfiguration$EnableGlobalAuthenticationAutowiredConfigurer",
                    "resource": "class path resource [org/springframework/security/config/annotation/authentication/configuration/AuthenticationConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "mvcUrlPathHelper": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.util.UrlPathHelper",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "servletWebServerFactoryCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/ServletWebServerFactoryAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.ServletWebServerFactoryAutoConfiguration",
                        "server-org.springframework.boot.autoconfigure.web.ServerProperties"
                    ]
                },
                "transactionTemplate": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.transaction.support.TransactionTemplate",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/transaction/TransactionAutoConfiguration$TransactionTemplateConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.transaction.TransactionAutoConfiguration$TransactionTemplateConfiguration",
                        "transactionManager"
                    ]
                },
                "claimAttachmentService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ClaimAttachmentService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ClaimAttachmentService.class]",
                    "dependencies": [
                        "claimAttachmentRepository"
                    ]
                },
                "cnaUnderwritingQuestionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CnaUnderwritingQuestionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CnaUnderwritingQuestionService.class]",
                    "dependencies": [
                        "cnaUnderwritingQuestionRepository"
                    ]
                },
                "warmTransferActivityController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.metricsControllers.WarmTransferActivityController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/metricsControllers/WarmTransferActivityController.class]",
                    "dependencies": [
                        "validationHelper",
                        "metricsService",
                        "campaignStatusService"
                    ]
                },
                "spring.sql.init-org.springframework.boot.autoconfigure.sql.init.SqlInitializationProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.sql.init.SqlInitializationProperties",
                    "resource": null,
                    "dependencies": []
                },
                "policyService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyService$$EnhancerBySpringCGLIB$$8cc815e7",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyService.class]",
                    "dependencies": [
                        "policyRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration$StringHttpMessageConverterConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration$StringHttpMessageConverterConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "leadMatchHistoryEntryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LeadMatchHistoryEntryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LeadMatchHistoryEntryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#49ecdbc8",
                        "(inner bean)#5f4f7f1a",
                        "(inner bean)#22d105f",
                        "jpaMappingContext"
                    ]
                },
                "shareInfoService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ShareInfoService$$EnhancerBySpringCGLIB$$967e6614",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ShareInfoService.class]",
                    "dependencies": [
                        "shareInfoRepository"
                    ]
                },
                "quoteService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.QuoteService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/QuoteService.class]",
                    "dependencies": [
                        "quoteRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.DispatcherServletAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "fieldValidationInterceptor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.interceptors.FieldValidationInterceptor",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/interceptors/FieldValidationInterceptor.class]",
                    "dependencies": [
                        "objectMapper"
                    ]
                },
                "agentPayoutMetricRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AgentPayoutMetricRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AgentPayoutMetricRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#54e1dc9a",
                        "(inner bean)#6868b60c",
                        "(inner bean)#a5491ab",
                        "jpaMappingContext"
                    ]
                },
                "boldPenguinControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.BoldPenguinControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/BoldPenguinControllerPublic.class]",
                    "dependencies": [
                        "userService",
                        "campaignStatusService",
                        "closeService",
                        "boldPenguinService",
                        "coverdashUserUtil",
                        "warmTransferService"
                    ]
                },
                "savvyCalService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.SavvyCalService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/SavvyCalService.class]",
                    "dependencies": [
                        "properties",
                        "policyService",
                        "businessService",
                        "saleService"
                    ]
                },
                "powerPointService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.PowerPointService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/PowerPointService.class]",
                    "dependencies": [
                        "properties",
                        "businessService",
                        "policyService",
                        "customCoverageElementService",
                        "employeeContactInformationService",
                        "coverdashUserUtil",
                        "businessLocationService",
                        "closeService",
                        "s3UploadService",
                        "renewalBatchService"
                    ]
                },
                "simpleMeterRegistry": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.simple.SimpleMeterRegistry",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/export/simple/SimpleMetricsExportAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.export.simple.SimpleMetricsExportAutoConfiguration",
                        "simpleConfig",
                        "micrometerClock"
                    ]
                },
                "authenticationEventPublisher": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.authentication.DefaultAuthenticationEventPublisher",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/security/servlet/SecurityAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.security.servlet.SecurityAutoConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "entityManagerFactory": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.sun.proxy.$Proxy150",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/orm/jpa/HibernateJpaConfiguration.class]",
                    "dependencies": [
                        "dataSourceScriptDatabaseInitializer",
                        "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaConfiguration",
                        "entityManagerFactoryBuilder"
                    ]
                },
                "startupTimeMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.startup.StartupTimeMetricsListener",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/startup/StartupTimeMetricsListenerAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.startup.StartupTimeMetricsListenerAutoConfiguration",
                        "simpleMeterRegistry"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.metadata.DataSourcePoolMetadataProvidersConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.metadata.DataSourcePoolMetadataProvidersConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "policyTransactionCopyService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyTransactionCopyService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyTransactionCopyService.class]",
                    "dependencies": [
                        "policyTransactionCopyRepository"
                    ]
                },
                "multipartConfigElement": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "javax.servlet.MultipartConfigElement",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/MultipartAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.MultipartAutoConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "beansEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.beans.BeansEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/beans/BeansEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.beans.BeansEndpointAutoConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "baseRenewalFormFieldRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.BaseRenewalFormFieldRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.BaseRenewalFormFieldRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1df73457",
                        "(inner bean)#378ffded",
                        "(inner bean)#7bc0e96a",
                        "jpaMappingContext"
                    ]
                },
                "localSpringDocParameterNameDiscoverer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.core.LocalVariableTableParameterNameDiscoverer",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration"
                    ]
                },
                "warmTransferService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.WarmTransferService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/WarmTransferService.class]",
                    "dependencies": [
                        "warmTransferRepository"
                    ]
                },
                "springDocObjectMapperProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.providers.ObjectMapperProvider",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "org.springdoc.core.SpringDocConfigProperties"
                    ]
                },
                "org.springframework.cloud.aws.context.support.io.SimpleStorageProtocolResolverConfigurer#0": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.context.support.io.SimpleStorageProtocolResolverConfigurer",
                    "resource": null,
                    "dependencies": [
                        "(inner bean)#626299bc"
                    ]
                },
                "partnerUserUtil": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.components.PartnerUserUtil",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/components/PartnerUserUtil.class]",
                    "dependencies": [
                        "auth0HttpClient",
                        "auth0PartnerTokenManager"
                    ]
                },
                "adminAppExportController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.AdminAppExportController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/AdminAppExportController.class]",
                    "dependencies": [
                        "properties",
                        "validationHelper",
                        "licenseService",
                        "adminAppUserUtil",
                        "adminAppExportService",
                        "partnerPaymentStructureService"
                    ]
                },
                "partnerAPIRequestService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerAPIRequestService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerAPIRequestService.class]",
                    "dependencies": [
                        "partnerAPIRequestRepository"
                    ]
                },
                "partnerPreferencesService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerPreferencesService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerPreferencesService.class]",
                    "dependencies": [
                        "partnerPreferencesRepository"
                    ]
                },
                "endpointOperationParameterMapper": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.invoke.convert.ConversionServiceParameterValueMapper",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/EndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.EndpointAutoConfiguration"
                    ]
                },
                "claudeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.ClaudeService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/ClaudeService.class]",
                    "dependencies": [
                        "PDFService",
                        "carrierService",
                        "promptService",
                        "docIngestionAISubmissionService",
                        "objectMapper"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.health.HealthContributorAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthContributorAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "renewalBatchService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalBatchService$$EnhancerBySpringCGLIB$$5da0c8d7",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalBatchService.class]",
                    "dependencies": [
                        "renewalBatchRepository"
                    ]
                },
                "policyTransactionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PolicyTransactionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PolicyTransactionService.class]",
                    "dependencies": [
                        "policyTransactionRepository"
                    ]
                },
                "org.springdoc.core.SpringDocConfigProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfigProperties",
                    "resource": null,
                    "dependencies": []
                },
                "servletWebChildContextFactory": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextFactory",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/web/servlet/ServletManagementContextAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.web.servlet.ServletManagementContextAutoConfiguration"
                    ]
                },
                "promptService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PromptService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PromptService.class]",
                    "dependencies": [
                        "coverageElementService",
                        "carrierService"
                    ]
                },
                "documentIngestionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.DocumentIngestionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/DocumentIngestionService.class]",
                    "dependencies": [
                        "carrierService",
                        "promptService",
                        "s3UploadService",
                        "reductoService",
                        "policyDocumentRelevantInformationMappingService",
                        "PDFService",
                        "claudeService",
                        "saleService",
                        "docIngestionAISubmissionService",
                        "docIngestionAISubmissionSuggestionService",
                        "trimmedDocService",
                        "objectMapper"
                    ]
                },
                "additionalModelsConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.AdditionalModelsConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "virtualCardRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.VirtualCardRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.VirtualCardRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5c8a83d",
                        "(inner bean)#709e3f6a",
                        "(inner bean)#6297b104",
                        "jpaMappingContext"
                    ]
                },
                "sentry-io.sentry.spring.boot.SentryProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryProperties",
                    "resource": null,
                    "dependencies": []
                },
                "docIngestionAISubmissionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.DocIngestionAISubmissionService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/DocIngestionAISubmissionService.class]",
                    "dependencies": [
                        "docIngestionAISubmissionRepository"
                    ]
                },
                "addressService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AddressService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AddressService.class]",
                    "dependencies": [
                        "addressRepository"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "webMvcTagsProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.metrics.web.servlet.DefaultWebMvcTagsProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/servlet/WebMvcMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration"
                    ]
                },
                "resourceHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.handler.SimpleUrlHandlerMapping",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcContentNegotiationManager",
                        "mvcConversionService",
                        "mvcResourceUrlProvider"
                    ]
                },
                "simpleControllerHandlerAdapter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.mvc.SimpleControllerHandlerAdapter",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "webhookHistoryService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.WebhookHistoryService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/WebhookHistoryService.class]",
                    "dependencies": [
                        "webhookHistoryRepository",
                        "helpscoutService",
                        "policyService"
                    ]
                },
                "awsS3ResourceLoaderProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.autoconfigure.context.properties.AwsS3ResourceLoaderProperties",
                    "resource": "class path resource [org/springframework/cloud/aws/autoconfigure/context/ContextResourceLoaderAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.cloud.aws.autoconfigure.context.ContextResourceLoaderAutoConfiguration"
                    ]
                },
                "auth0CoverdashTokenManager": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.tokenManagers.Auth0CoverdashTokenManager",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/tokenManagers/Auth0CoverdashTokenManager.class]",
                    "dependencies": [
                        "auth0HttpClient"
                    ]
                },
                "org.springframework.cloud.aws.core.env.ResourceIdResolver.BEAN_NAME": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.cloud.aws.core.env.StackResourceRegistryDetectingResourceIdResolver",
                    "resource": null,
                    "dependencies": []
                },
                "coiPolicyLinkService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CoiPolicyLinkService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CoiPolicyLinkService.class]",
                    "dependencies": [
                        "coiPolicyLinkRepository"
                    ]
                },
                "paymentPlanService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PaymentPlanService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PaymentPlanService.class]",
                    "dependencies": [
                        "paymentPlanRepository"
                    ]
                },
                "taskExecutor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.scheduling.concurrent.ThreadPoolTaskExecutor",
                    "resource": "class path resource [com/coverdash/crud_service/configuration/AsyncConfig.class]",
                    "dependencies": [
                        "asyncConfig"
                    ]
                },
                "management.endpoint.configprops-org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.context.properties.ConfigurationPropertiesReportEndpointProperties",
                    "resource": null,
                    "dependencies": []
                },
                "parameterNamesModule": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.fasterxml.jackson.module.paramnames.ParameterNamesModule",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jackson/JacksonAutoConfiguration$ParameterNamesModuleConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$ParameterNamesModuleConfiguration"
                    ]
                },
                "micrometerClock": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.Clock$1",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/MetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration"
                    ]
                },
                "partnerRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#691722b4",
                        "(inner bean)#63657988",
                        "(inner bean)#6ae8efc6",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.beans.BeansEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.beans.BeansEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "pageableOpenAPIConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.PageableOpenAPIConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration$SpringDocPageableConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration$SpringDocPageableConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "CRMController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.CRMController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/CRMController.class]",
                    "dependencies": [
                        "validationHelper",
                        "properties",
                        "policyService",
                        "activityService",
                        "taskService",
                        "userService",
                        "policyTransactionService",
                        "noteService",
                        "closeService",
                        "agentAssistant",
                        "businessService"
                    ]
                },
                "gsonBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.google.gson.GsonBuilder",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/gson/GsonAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.gson.GsonAutoConfiguration",
                        "standardGsonBuilderCustomizer"
                    ]
                },
                "securityParser": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SecurityService",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "propertyResolverUtils"
                    ]
                },
                "businessInviteRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.BusinessInviteRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.BusinessInviteRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#5d2b5b6c",
                        "(inner bean)#552d2df6",
                        "(inner bean)#52990f00",
                        "jpaMappingContext"
                    ]
                },
                "customerTouchPointControllerPublic": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.publicControllers.CustomerTouchPointControllerPublic",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/publicControllers/CustomerTouchPointControllerPublic.class]",
                    "dependencies": [
                        "properties",
                        "adminAppCustomersService",
                        "customerTouchPointService"
                    ]
                },
                "org.springframework.data.jpa.util.JpaMetamodelCacheCleanup": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.jpa.util.JpaMetamodelCacheCleanup",
                    "resource": null,
                    "dependencies": []
                },
                "noticeOfCancellationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.NoticeOfCancellationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.NoticeOfCancellationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#26e57fce",
                        "(inner bean)#1a74e65",
                        "(inner bean)#7e5f596f",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "server-org.springframework.boot.autoconfigure.web.ServerProperties"
                    ]
                },
                "servletEndpointDiscoverer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.annotation.ServletEndpointDiscoverer",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/WebEndpointAutoConfiguration$WebEndpointServletConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointAutoConfiguration$WebEndpointServletConfiguration",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "metricsHttpServerUriTagFilter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.config.MeterFilter$9",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/web/servlet/WebMvcMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.web.servlet.WebMvcMetricsAutoConfiguration"
                    ]
                },
                "subscriptionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.SubscriptionService$$EnhancerBySpringCGLIB$$d1800b66",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/SubscriptionService.class]",
                    "dependencies": [
                        "subscriptionRepository"
                    ]
                },
                "org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration$TomcatWebSocketConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.websocket.servlet.WebSocketServletAutoConfiguration$TomcatWebSocketConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.http.HttpMessageConvertersAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "webSecurity": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.oauthSetup.WebSecurityConfig$$Lambda$1322/0x0000000800d8e840",
                    "resource": "class path resource [com/coverdash/crud_service/oauthSetup/WebSecurityConfig.class]",
                    "dependencies": [
                        "webSecurityConfig"
                    ]
                },
                "healthEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.health.HealthEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointConfiguration",
                        "healthContributorRegistry",
                        "healthEndpointGroups",
                        "management.endpoint.health-org.springframework.boot.actuate.autoconfigure.health.HealthEndpointProperties"
                    ]
                },
                "viewControllerHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.HandlerMapping",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration",
                        "mvcConversionService",
                        "mvcResourceUrlProvider"
                    ]
                },
                "spring.task.execution-org.springframework.boot.autoconfigure.task.TaskExecutionProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.task.TaskExecutionProperties",
                    "resource": null,
                    "dependencies": []
                },
                "sentryTransactionAdvice": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.tracing.SentryTransactionAdvice",
                    "resource": "class path resource [io/sentry/spring/tracing/SentryAdviceConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.tracing.SentryAdviceConfiguration",
                        "sentryHub"
                    ]
                },
                "manualPlacementController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.ManualPlacementController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/ManualPlacementController.class]",
                    "dependencies": [
                        "cohortService",
                        "documentIngestionService",
                        "properties",
                        "quoteService",
                        "subscriptionService",
                        "virtualCardService",
                        "validationHelper",
                        "agentAssistant",
                        "carrierCommission",
                        "closeService",
                        "businessService",
                        "businessLocationService",
                        "addressService",
                        "userService",
                        "businessClassificationService",
                        "generalClassificationInformationService",
                        "policyService",
                        "carrierService",
                        "customCoverageElementService",
                        "coverageElementService",
                        "activityService",
                        "adminAppUserUtil",
                        "tooltipService",
                        "policyTransactionService",
                        "carrierAutoRenewalService",
                        "claimService",
                        "accountManagerPayoutMetricService",
                        "manualPlacementService",
                        "renewalBatchService",
                        "helpscoutService",
                        "operationsService",
                        "loopsService",
                        "coverdashUserUtil",
                        "docIngestionAISubmissionService",
                        "stripeService",
                        "ncciClassService",
                        "licenseService"
                    ]
                },
                "themeResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.servlet.theme.FixedThemeResolver",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.jdbc.metadata.DataSourcePoolMetadataProvidersConfiguration$HikariPoolDataSourceMetadataProviderConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.metadata.DataSourcePoolMetadataProvidersConfiguration$HikariPoolDataSourceMetadataProviderConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "mvcPatternParser": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.web.util.pattern.PathPatternParser",
                    "resource": "class path resource [org/springframework/web/servlet/config/annotation/DelegatingWebMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.web.servlet.config.annotation.DelegatingWebMvcConfiguration"
                    ]
                },
                "transactionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.TransactionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.TransactionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#43187052",
                        "(inner bean)#74be2d81",
                        "(inner bean)#1ebfb7b6",
                        "jpaMappingContext"
                    ]
                },
                "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "loggerInterceptor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.oauthSetup.LoggerInterceptor",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/oauthSetup/LoggerInterceptor.class]",
                    "dependencies": []
                },
                "org.springframework.boot.sql.init.dependency.DatabaseInitializationDependencyConfigurer$DependsOnDatabaseInitializationPostProcessor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.sql.init.dependency.DatabaseInitializationDependencyConfigurer$DependsOnDatabaseInitializationPostProcessor",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.task.TaskExecutorMetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.task.TaskExecutorMetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": [
                        "taskExecutor",
                        "simpleMeterRegistry"
                    ]
                },
                "adminAppController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.AdminAppController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/AdminAppController.class]",
                    "dependencies": [
                        "quoteService",
                        "properties",
                        "validationHelper",
                        "policyService",
                        "policyTransactionService",
                        "carrierCommission",
                        "coverageElementService",
                        "startupIndustryService",
                        "ncciClassService",
                        "businessClassificationService",
                        "businessLocationService",
                        "addressService",
                        "partnerService",
                        "licenseService",
                        "generalClassificationInformationService",
                        "agentPayoutMetricService",
                        "accountManagerPayoutMetricService",
                        "applicationSubmissionService",
                        "businessService",
                        "partnerAPIRequestService",
                        "closeService",
                        "adminAppUserUtil",
                        "adminAppService",
                        "customFormFieldService",
                        "userService",
                        "customCoverageElementService",
                        "carrierService",
                        "saleAnnouncementService",
                        "partnerPaymentStructureService",
                        "saleService",
                        "employeeContactInformationService",
                        "partnerWebpageService",
                        "policyTypeService",
                        "recommendedPolicyService",
                        "partnerPreferencesService",
                        "partnerTechnologyFeeService",
                        "agentScoreService",
                        "agencyStatService",
                        "agentLeadRuleService",
                        "loopsService",
                        "agentAssistant",
                        "partnerUserUtil",
                        "coverdashUserUtil",
                        "licenseThemeService"
                    ]
                },
                "org.springdoc.core.SpringDocConfiguration$SpringDocPageableConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocConfiguration$SpringDocPageableConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "partnerService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.PartnerService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/PartnerService.class]",
                    "dependencies": [
                        "partnerRepository"
                    ]
                },
                "accountManagerStatRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AccountManagerStatRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AccountManagerStatRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#56a6a684",
                        "(inner bean)#56db546a",
                        "(inner bean)#3faff6a1",
                        "jpaMappingContext"
                    ]
                },
                "affinityPartnerCommissionRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.AffinityPartnerCommissionRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.AffinityPartnerCommissionRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#7c06c9ed",
                        "(inner bean)#61a045c5",
                        "(inner bean)#73985f35",
                        "jpaMappingContext"
                    ]
                },
                "webEndpointServletHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.servlet.WebMvcEndpointHandlerMapping",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/endpoint/web/servlet/WebMvcEndpointManagementContextConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.endpoint.web.servlet.WebMvcEndpointManagementContextConfiguration",
                        "webEndpointDiscoverer",
                        "servletEndpointDiscoverer",
                        "controllerEndpointDiscoverer",
                        "endpointMediaTypes",
                        "management.endpoints.web.cors-org.springframework.boot.actuate.autoconfigure.endpoint.web.CorsEndpointProperties",
                        "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties",
                        "environment"
                    ]
                },
                "accountManagerOperationsController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.AccountManagerOperationsController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/AccountManagerOperationsController.class]",
                    "dependencies": [
                        "employeeContactInformationService",
                        "carrierAutoRenewalService",
                        "properties",
                        "businessService",
                        "policyService",
                        "agentAssistant",
                        "closeService",
                        "renewalBatchService",
                        "accountManagerPayoutMetricService"
                    ]
                },
                "accountingUploadService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AccountingUploadService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AccountingUploadService.class]",
                    "dependencies": [
                        "accountingUploadRepository"
                    ]
                },
                "dispatcherServletMappingDescriptionProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.web.mappings.servlet.DispatcherServletsMappingDescriptionProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/web/mappings/MappingsEndpointAutoConfiguration$ServletWebConfiguration$SpringMvcConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration$SpringMvcConfiguration"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.scheduling.ScheduledTasksEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.scheduling.ScheduledTasksEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.jdbc-org.springframework.boot.autoconfigure.jdbc.JdbcProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jdbc.JdbcProperties",
                    "resource": null,
                    "dependencies": []
                },
                "leadScoreWeightValueService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.LeadScoreWeightValueService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/LeadScoreWeightValueService.class]",
                    "dependencies": [
                        "leadScoreWeightValueRepository"
                    ]
                },
                "documentIngestionController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.DocumentIngestionController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/DocumentIngestionController.class]",
                    "dependencies": [
                        "validationHelper",
                        "documentIngestionService",
                        "saleService",
                        "PDFService",
                        "docIngestionAISubmissionService",
                        "objectMapper",
                        "docIngestionEvaluationService",
                        "s3UploadService",
                        "docIngestionAISubmissionSuggestionService"
                    ]
                },
                "closeService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.CloseService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/CloseService.class]",
                    "dependencies": [
                        "properties",
                        "policyService",
                        "businessService",
                        "saleService",
                        "leadService",
                        "lateInvoicePolicyLinkService",
                        "lateInvoiceService",
                        "slackLeadService",
                        "businessLocationService",
                        "addressService"
                    ]
                },
                "auth0AdminTokenManager": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.tokenManagers.Auth0AdminTokenManager",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/tokenManagers/Auth0AdminTokenManager.class]",
                    "dependencies": [
                        "auth0HttpClient"
                    ]
                },
                "agentScoreService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.AgentScoreService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/AgentScoreService.class]",
                    "dependencies": [
                        "agentScoreRepository"
                    ]
                },
                "startupIndustryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.StartupIndustryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.StartupIndustryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#6e858079",
                        "(inner bean)#264700ed",
                        "(inner bean)#ab7eb31",
                        "jpaMappingContext"
                    ]
                },
                "inAppPackagesResolver": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.InAppIncludesResolver",
                    "resource": "class path resource [io/sentry/spring/boot/SentryAutoConfiguration$HubConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration"
                    ]
                },
                "adminAppCustomersService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.AdminAppCustomersService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/AdminAppCustomersService.class]",
                    "dependencies": [
                        "customCoverageElementService",
                        "policyService",
                        "closeService",
                        "businessService",
                        "employeeContactInformationService",
                        "agentOutOfOfficeService",
                        "coverdashUserUtil"
                    ]
                },
                "renewalCarrierSLARepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalCarrierSLARepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalCarrierSLARepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#102645b8",
                        "(inner bean)#698e4e6c",
                        "(inner bean)#3179fa7c",
                        "jpaMappingContext"
                    ]
                },
                "policyNoteRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PolicyNoteRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PolicyNoteRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#689f9dc8",
                        "(inner bean)#7181f2ac",
                        "(inner bean)#74aa8c30",
                        "jpaMappingContext"
                    ]
                },
                "springDocProviders": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.SpringDocProviders",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "spring.netty-org.springframework.boot.autoconfigure.netty.NettyProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.netty.NettyProperties",
                    "resource": null,
                    "dependencies": []
                },
                "loggersEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.logging.LoggersEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/logging/LoggersEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.logging.LoggersEndpointAutoConfiguration",
                        "springBootLoggingSystem"
                    ]
                },
                "openEntityManagerInViewInterceptorConfigurer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.orm.jpa.JpaBaseConfiguration$JpaWebConfiguration$1",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/orm/jpa/JpaBaseConfiguration$JpaWebConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.orm.jpa.JpaBaseConfiguration$JpaWebConfiguration",
                        "openEntityManagerInViewInterceptor"
                    ]
                },
                "tomcatWebServerFactoryCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.embedded.TomcatWebServerFactoryCustomizer",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/embedded/EmbeddedWebServerFactoryCustomizerAutoConfiguration$TomcatWebServerFactoryCustomizerConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.embedded.EmbeddedWebServerFactoryCustomizerAutoConfiguration$TomcatWebServerFactoryCustomizerConfiguration",
                        "environment",
                        "server-org.springframework.boot.autoconfigure.web.ServerProperties"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.endpoint.EndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.EndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "loopsHistoryRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.LoopsHistoryRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.LoopsHistoryRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#1a763008",
                        "(inner bean)#6c83c86f",
                        "(inner bean)#2f312137",
                        "jpaMappingContext"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "partnerPaymentStructureRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.PartnerPaymentStructureRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.PartnerPaymentStructureRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#16165af2",
                        "(inner bean)#10005a46",
                        "(inner bean)#2ee58ed1",
                        "jpaMappingContext"
                    ]
                },
                "quotingPageService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.QuotingPageService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/QuotingPageService.class]",
                    "dependencies": [
                        "properties",
                        "virtualCardService",
                        "helpscoutService",
                        "stripeService",
                        "braintreeService",
                        "s3UploadService",
                        "technologyFeeService",
                        "applicationSubmissionBatchService",
                        "employeeContactInformationService",
                        "applicationSubmissionService",
                        "carrierQuoteRequestService",
                        "slackLeadService",
                        "policyTypeService",
                        "businessService",
                        "carrierService",
                        "policyService",
                        "quoteService",
                        "closeService",
                        "carrierAppetiteSuggestionOverrideService",
                        "ascendService"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthContributorAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.system.DiskSpaceHealthContributorAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "fileSupportConverter": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.converters.FileSupportConverter",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration",
                        "springDocObjectMapperProvider"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.metrics.MetricsAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "amazonSQS": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.amazonaws.services.sqs.buffered.AmazonSQSBufferedAsyncClient",
                    "resource": "class path resource [org/springframework/cloud/aws/messaging/config/annotation/SqsClientConfiguration.class]",
                    "dependencies": [
                        "org.springframework.cloud.aws.messaging.config.annotation.SqsClientConfiguration"
                    ]
                },
                "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.sentry.spring.boot.SentryAutoConfiguration$HubConfiguration$SentryWebMvcConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "cachesEndpoint": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.cache.CachesEndpoint",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/cache/CachesEndpointAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.cache.CachesEndpointAutoConfiguration"
                    ]
                },
                "taskService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.TaskService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/TaskService.class]",
                    "dependencies": [
                        "taskRepository"
                    ]
                },
                "pageableCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.data.web.SpringDataWebAutoConfiguration$$Lambda$1313/0x0000000800d61c40",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/data/web/SpringDataWebAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.data.web.SpringDataWebAutoConfiguration"
                    ]
                },
                "carrierAppetiteSuggestionOverrideRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.CarrierAppetiteSuggestionOverrideRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.CarrierAppetiteSuggestionOverrideRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#373aa5d6",
                        "(inner bean)#225be644",
                        "(inner bean)#63c9df77",
                        "jpaMappingContext"
                    ]
                },
                "dataSource": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.zaxxer.hikari.HikariDataSource",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/jdbc/DataSourceConfiguration$Hikari.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.jdbc.DataSourceConfiguration$Hikari",
                        "spring.datasource-org.springframework.boot.autoconfigure.jdbc.DataSourceProperties"
                    ]
                },
                "metricsService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.MetricsService",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/MetricsService.class]",
                    "dependencies": [
                        "policyService",
                        "helpScoutTicketHistoryService",
                        "employeeContactInformationService",
                        "applicationSubmissionService",
                        "policyTransactionService",
                        "partnerPaymentsUtil",
                        "businessService",
                        "adminAppUserUtil",
                        "agentPayoutMetricService",
                        "accountManagerPayoutMetricService",
                        "accountManagerStatService",
                        "campaignStatusService",
                        "helpScoutTicketService",
                        "licenseService",
                        "accountExecutiveStatService",
                        "techFeeEligibilityService",
                        "warmTransferService"
                    ]
                },
                "management.endpoints.web-org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.endpoint.web.WebEndpointProperties",
                    "resource": null,
                    "dependencies": []
                },
                "agentAvailabilityController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.AgentAvailabilityController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/AgentAvailabilityController.class]",
                    "dependencies": [
                        "validationHelper",
                        "agentAvailabilityService",
                        "agentStatusService",
                        "agentStatusHistoryService",
                        "campaignStatusService",
                        "adminAppUserUtil",
                        "campaignStatusHistoryService",
                        "employeeContactInformationService"
                    ]
                },
                "jpaMappingContext": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.data.jpa.mapping.JpaMetamodelMappingContext",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration$MappingJackson2HttpMessageConverterConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.http.JacksonHttpMessageConvertersConfiguration$MappingJackson2HttpMessageConverterConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "spring.jackson-org.springframework.boot.autoconfigure.jackson.JacksonProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonProperties",
                    "resource": null,
                    "dependencies": []
                },
                "error": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$StaticView",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/web/servlet/error/ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.web.servlet.error.ErrorMvcAutoConfiguration$WhitelabelErrorViewConfiguration"
                    ]
                },
                "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.autoconfigure.jackson.JacksonAutoConfiguration$JacksonObjectMapperConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "swaggerConfigResource": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.ui.SwaggerConfigResource",
                    "resource": "class path resource [org/springdoc/webmvc/ui/SwaggerConfig.class]",
                    "dependencies": [
                        "org.springdoc.webmvc.ui.SwaggerConfig",
                        "swaggerWelcome"
                    ]
                },
                "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointAutoConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointAutoConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "delegatingMethodParameterCustomizer": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.core.customizers.DataRestDelegatingMethodParameterCustomizer",
                    "resource": "class path resource [org/springdoc/core/SpringDocConfiguration$SpringDocSortConfiguration.class]",
                    "dependencies": [
                        "org.springdoc.core.SpringDocConfiguration$SpringDocSortConfiguration"
                    ]
                },
                "jvmGcMetrics": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "io.micrometer.core.instrument.binder.jvm.JvmGcMetrics",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/metrics/JvmMetricsAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.metrics.JvmMetricsAutoConfiguration"
                    ]
                },
                "healthEndpointWebMvcHandlerMapping": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.endpoint.web.servlet.AdditionalHealthEndpointPathsWebMvcHandlerMapping",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/health/HealthEndpointWebExtensionConfiguration$MvcAdditionalHealthEndpointPathsConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.health.HealthEndpointWebExtensionConfiguration$MvcAdditionalHealthEndpointPathsConfiguration",
                        "webEndpointDiscoverer",
                        "healthEndpointGroups"
                    ]
                },
                "cancellationMetricsDashboardController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.metricsControllers.CancellationMetricsDashboardController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/metricsControllers/CancellationMetricsDashboardController.class]",
                    "dependencies": [
                        "validationHelper",
                        "metricsService",
                        "licenseService",
                        "carrierService",
                        "policyService"
                    ]
                },
                "sentryTransactionAdvisor": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.aop.support.DefaultPointcutAdvisor",
                    "resource": "class path resource [io/sentry/spring/tracing/SentryAdviceConfiguration.class]",
                    "dependencies": [
                        "io.sentry.spring.tracing.SentryAdviceConfiguration",
                        "sentryTransactionPointcut",
                        "sentryTransactionAdvice"
                    ]
                },
                "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration$SpringDocWebMvcActuatorConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration$SpringDocWebMvcActuatorConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "coiToolController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.adminAppControllers.CoiToolController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/adminAppControllers/CoiToolController.class]",
                    "dependencies": [
                        "validationHelper",
                        "coiToolServiceUtil",
                        "certificateOfInsuranceService",
                        "businessService",
                        "policyService",
                        "shareInfoService",
                        "coiToolService",
                        "operationsService",
                        "policyTypeService",
                        "coiPolicyLinkService"
                    ]
                },
                "filterMappingDescriptionProvider": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.web.mappings.servlet.FiltersMappingDescriptionProvider",
                    "resource": "class path resource [org/springframework/boot/actuate/autoconfigure/web/mappings/MappingsEndpointAutoConfiguration$ServletWebConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.actuate.autoconfigure.web.mappings.MappingsEndpointAutoConfiguration$ServletWebConfiguration"
                    ]
                },
                "operationsController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.OperationsController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/OperationsController.class]",
                    "dependencies": [
                        "policyTypeService",
                        "properties",
                        "braintreeService",
                        "virtualCardService",
                        "validationHelper",
                        "transactionManagerService",
                        "closeService",
                        "certificateHolderTemplateService",
                        "policyTransactionService",
                        "businessService",
                        "applicationSubmissionService",
                        "claimService",
                        "quoteService",
                        "policyService",
                        "businessLocationService",
                        "addressService",
                        "userService",
                        "customCoverageElementService",
                        "excludedCoverageElementService",
                        "coverageElementService",
                        "generalClassificationInformationService",
                        "policyNoteService",
                        "operationsService",
                        "jdbcTemplate",
                        "ascendService",
                        "saleService",
                        "adminAppService",
                        "licenseService",
                        "manualPlacementService",
                        "coverdashUserUtil"
                    ]
                },
                "asyncDocumentIngestionService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.services.AsyncDocumentIngestionService$$EnhancerBySpringCGLIB$$9dfc0440",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/services/AsyncDocumentIngestionService.class]",
                    "dependencies": [
                        "documentIngestionService"
                    ]
                },
                "renewalFormFieldRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalFormFieldRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalFormFieldRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3f504d20",
                        "(inner bean)#5c7744f0",
                        "(inner bean)#75ff2d79",
                        "jpaMappingContext"
                    ]
                },
                "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration$SpringDocWebMvcRouterConfiguration": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springdoc.webmvc.core.SpringDocWebMvcConfiguration$SpringDocWebMvcRouterConfiguration",
                    "resource": null,
                    "dependencies": []
                },
                "authenticationManagerBuilder": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.config.annotation.authentication.configuration.AuthenticationConfiguration$DefaultPasswordEncoderAuthenticationManagerBuilder",
                    "resource": "class path resource [org/springframework/security/config/annotation/authentication/configuration/AuthenticationConfiguration.class]",
                    "dependencies": [
                        "org.springframework.security.config.annotation.authentication.configuration.AuthenticationConfiguration",
                        "objectPostProcessor",
                        "org.springframework.boot.web.servlet.context.AnnotationConfigServletWebServerApplicationContext@1c98290c"
                    ]
                },
                "webSecurityExpressionHandler": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.security.web.access.expression.DefaultWebSecurityExpressionHandler",
                    "resource": "class path resource [org/springframework/security/config/annotation/web/configuration/WebSecurityConfiguration.class]",
                    "dependencies": [
                        "springSecurityFilterChain",
                        "org.springframework.security.config.annotation.web.configuration.WebSecurityConfiguration"
                    ]
                },
                "management.endpoint.logfile-org.springframework.boot.actuate.autoconfigure.logging.LogFileWebEndpointProperties": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "org.springframework.boot.actuate.autoconfigure.logging.LogFileWebEndpointProperties",
                    "resource": null,
                    "dependencies": []
                },
                "formController": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.crud_service.controllers.FormController",
                    "resource": "file [/Users/bennymagid/Development/crud_service/target/classes/com/coverdash/crud_service/controllers/FormController.class]",
                    "dependencies": [
                        "properties"
                    ]
                },
                "gson": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.google.gson.Gson",
                    "resource": "class path resource [org/springframework/boot/autoconfigure/gson/GsonAutoConfiguration.class]",
                    "dependencies": [
                        "org.springframework.boot.autoconfigure.gson.GsonAutoConfiguration",
                        "gsonBuilder"
                    ]
                },
                "renewalFormTemplateRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.RenewalFormTemplateRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.RenewalFormTemplateRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#54e1c058",
                        "(inner bean)#11908095",
                        "(inner bean)#6453dcc3",
                        "jpaMappingContext"
                    ]
                },
                "renewalPolicyService": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.services.RenewalPolicyService",
                    "resource": "URL [jar:file:/Users/bennymagid/.m2/repository/com/coverdash/coverdash_common/1.1210/coverdash_common-1.1210.jar!/com/coverdash/coverdash_common/services/RenewalPolicyService.class]",
                    "dependencies": [
                        "renewalPolicyRepository"
                    ]
                },
                "generalClassificationInformationRepository": {
                    "aliases": [],
                    "scope": "singleton",
                    "type": "com.coverdash.coverdash_common.repositories.GeneralClassificationInformationRepository",
                    "resource": "com.coverdash.coverdash_common.repositories.GeneralClassificationInformationRepository defined in @EnableJpaRepositories declared on CrudServiceApplication",
                    "dependencies": [
                        "(inner bean)#3e8771a1",
                        "(inner bean)#1f3241b3",
                        "(inner bean)#342daa77",
                        "jpaMappingContext"
                    ]
                }
            },
            "parentId": null
        }
    }
}
