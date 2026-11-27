---
api_specs:
- filename: azure-service-bus-namespaces-api-openapi.yml
  format: yaml
  label: Azure Service Bus Namespaces API
  slug: azure-service-bus-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-namespaces-api-openapi.yml
- filename: azure-service-bus-queues-api-openapi.yml
  format: yaml
  label: Azure Service Bus Queues API
  slug: azure-service-bus-queues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-queues-api-openapi.yml
- filename: azure-service-bus-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Service Bus Subscriptions API
  slug: azure-service-bus-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-subscriptions-api-openapi.yml
- filename: azure-service-bus-topics-api-openapi.yml
  format: yaml
  label: Azure Service Bus Topics API
  slug: azure-service-bus-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-topics-api-openapi.yml
- filename: azure-service-bus-armdisasterrecoveries-api-openapi.yml
  format: yaml
  label: Azure Service Bus Arm Disaster Recoveries API
  slug: azure-service-bus-armdisasterrecoveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-armdisasterrecoveries-api-openapi.yml
- filename: azure-service-bus-disasterrecoveryconfigs-api-openapi.yml
  format: yaml
  label: Azure Service Bus Disaster Recovery Configs API
  slug: azure-service-bus-disasterrecoveryconfigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-disasterrecoveryconfigs-api-openapi.yml
- filename: azure-service-bus-migrationconfigs-api-openapi.yml
  format: yaml
  label: Azure Service Bus Migration Configs API
  slug: azure-service-bus-migrationconfigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-migrationconfigs-api-openapi.yml
- filename: azure-service-bus-namespaces-authorizationrule-api-openapi.yml
  format: yaml
  label: Azure Service Bus Namespaces AuthorizationRule API
  slug: azure-service-bus-namespaces-authorizationrule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-namespaces-authorizationrule-api-openapi.yml
- filename: azure-service-bus-networksecurityperimeterconfigurations-api-openapi.yml
  format: yaml
  label: Azure Service Bus Network Security Perimeter Configurations API
  slug: azure-service-bus-networksecurityperimeterconfigurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-networksecurityperimeterconfigurations-api-openapi.yml
- filename: azure-service-bus-operations-api-openapi.yml
  format: yaml
  label: Azure Service Bus Operations API
  slug: azure-service-bus-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-operations-api-openapi.yml
- filename: azure-service-bus-rules-api-openapi.yml
  format: yaml
  label: Azure Service Bus Rules API
  slug: azure-service-bus-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-rules-api-openapi.yml
- filename: azure-service-bus-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Service Bus Private Endpoint Connections API
  slug: azure-service-bus-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-service-bus/openapi/azure-service-bus-private-endpoint-connections-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure Service Bus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Service Bus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Service Bus
provider_slug: azure-service-bus
slug: azure-service-bus-domain-security
source_filename: azure-service-bus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-service-bus/security/azure-service-bus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Microsoft Azure
- Cloud
- Enterprise
- Message Broker
- Messaging
- Pub/Sub
- Queues
- Real-Time
---
