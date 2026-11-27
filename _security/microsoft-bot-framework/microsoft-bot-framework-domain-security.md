---
api_specs:
- filename: microsoft-bot-framework-bot-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot API
  slug: microsoft-bot-framework-bot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-bot-api-openapi.yml
- filename: microsoft-bot-framework-botconnection-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Connection API
  slug: microsoft-bot-framework-botconnection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-botconnection-api-openapi.yml
- filename: microsoft-bot-framework-bothostsettings-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Bot Host Settings API
  slug: microsoft-bot-framework-bothostsettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-bothostsettings-api-openapi.yml
- filename: microsoft-bot-framework-channel-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Channel API
  slug: microsoft-bot-framework-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-channel-api-openapi.yml
- filename: microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework List Qn A Maker Endpoint Keys API
  slug: microsoft-bot-framework-listqnamakerendpointkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-listqnamakerendpointkeys-api-openapi.yml
- filename: microsoft-bot-framework-listserviceproviders-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework List Service Providers API
  slug: microsoft-bot-framework-listserviceproviders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-listserviceproviders-api-openapi.yml
- filename: microsoft-bot-framework-operationresults-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Operation Results API
  slug: microsoft-bot-framework-operationresults-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-operationresults-api-openapi.yml
- filename: microsoft-bot-framework-operations-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Operations API
  slug: microsoft-bot-framework-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-operations-api-openapi.yml
- filename: microsoft-bot-framework-privatelinkresources-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Private Link Resources API
  slug: microsoft-bot-framework-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-privatelinkresources-api-openapi.yml
- filename: microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Microsoft Bot Framework Private Endpoint Connections API
  slug: microsoft-bot-framework-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bot-framework/openapi/microsoft-bot-framework-private-endpoint-connections-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: botframework.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: dev.botframework.com
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
name: Microsoft Bot Framework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Bot Framework, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Bot Framework
provider_slug: microsoft-bot-framework
slug: microsoft-bot-framework-domain-security
source_filename: microsoft-bot-framework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: dev.botframework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: botframework.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-bot-framework/security/microsoft-bot-framework-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bots
- Conversational AI
- Messaging
- Bot Framework
- Direct Line
---
