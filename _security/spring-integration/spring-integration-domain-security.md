---
api_specs:
- filename: spring-integration-adapters-api-openapi.yml
  format: yaml
  label: Spring Integration Adapters API
  slug: spring-integration-adapters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-adapters-api-openapi.yml
- filename: spring-integration-channels-api-openapi.yml
  format: yaml
  label: Spring Integration Channels API
  slug: spring-integration-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-channels-api-openapi.yml
- filename: spring-integration-control-api-openapi.yml
  format: yaml
  label: Spring Integration Control API
  slug: spring-integration-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-control-api-openapi.yml
- filename: spring-integration-gateway-api-openapi.yml
  format: yaml
  label: Spring Integration Gateway API
  slug: spring-integration-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-gateway-api-openapi.yml
- filename: spring-integration-graph-api-openapi.yml
  format: yaml
  label: Spring Integration Graph API
  slug: spring-integration-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-graph-api-openapi.yml
- filename: spring-integration-handlers-api-openapi.yml
  format: yaml
  label: Spring Integration Handlers API
  slug: spring-integration-handlers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-handlers-api-openapi.yml
- filename: spring-integration-history-api-openapi.yml
  format: yaml
  label: Spring Integration History API
  slug: spring-integration-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-history-api-openapi.yml
- filename: spring-integration-inbound-adapter-api-openapi.yml
  format: yaml
  label: Spring Integration Inbound Adapter API
  slug: spring-integration-inbound-adapter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/openapi/spring-integration-inbound-adapter-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spring.io
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: spring.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: docs.spring.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spring Integration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Integration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Integration
provider_slug: spring-integration
slug: spring-integration-domain-security
source_filename: spring-integration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-integration/refs/heads/main/security/spring-integration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AMQP
- Enterprise Integration
- Event-Driven
- Integration Patterns
- Java
- Messaging
- Spring
---
