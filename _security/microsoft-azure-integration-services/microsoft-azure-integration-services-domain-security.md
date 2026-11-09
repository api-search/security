---
api_specs:
- filename: microsoft-azure-integration-services-azure-logic-apps-openapi.yml
  format: yaml
  label: Azure Logic Apps
  slug: azure-logic-apps
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-integration-services/openapi/microsoft-azure-integration-services-azure-logic-apps-openapi.yml
- filename: microsoft-azure-integration-services-azure-service-bus-openapi.yml
  format: yaml
  label: Azure Service Bus
  slug: azure-service-bus
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-integration-services/openapi/microsoft-azure-integration-services-azure-service-bus-openapi.yml
- filename: microsoft-azure-integration-services-azure-event-grid-openapi.yml
  format: yaml
  label: Azure Event Grid
  slug: azure-event-grid
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-integration-services/openapi/microsoft-azure-integration-services-azure-event-grid-openapi.yml
- filename: microsoft-azure-integration-services-azure-event-hubs-openapi.yml
  format: yaml
  label: Azure Event Hubs
  slug: azure-event-hubs
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-integration-services/openapi/microsoft-azure-integration-services-azure-event-hubs-openapi.yml
- filename: microsoft-azure-integration-services-operations-api-openapi.yml
  format: yaml
  label: Microsoft Azure Integration Services Operations API
  slug: microsoft-azure-integration-services-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-integration-services/openapi/microsoft-azure-integration-services-operations-api-openapi.yml
- filename: microsoft-azure-integration-services-azure-api-management-openapi.yml
  format: yaml
  label: Azure API Management
  slug: microsoft-azure-integration-services-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-integration-services/openapi/microsoft-azure-integration-services-azure-api-management-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
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
name: Microsoft Azure Integration Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Integration Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Azure Integration Services
provider_slug: microsoft-azure-integration-services
slug: microsoft-azure-integration-services-domain-security
source_filename: microsoft-azure-integration-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-integration-services/security/microsoft-azure-integration-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Enterprise
- Event-Driven
- Integration
- Messaging
---
