---
api_specs:
- filename: spring-boot-3-environment-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Environment API
  slug: spring-boot-3-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-environment-api-openapi.yml
- filename: spring-boot-3-health-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Health API
  slug: spring-boot-3-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-health-api-openapi.yml
- filename: spring-boot-3-info-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Info API
  slug: spring-boot-3-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-info-api-openapi.yml
- filename: spring-boot-3-loggers-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Loggers API
  slug: spring-boot-3-loggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-loggers-api-openapi.yml
- filename: spring-boot-3-metrics-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Metrics API
  slug: spring-boot-3-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-metrics-api-openapi.yml
- filename: spring-boot-3-scheduling-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Scheduling API
  slug: spring-boot-3-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-scheduling-api-openapi.yml
- filename: spring-boot-3-threads-api-openapi.yml
  format: yaml
  label: Spring Boot 3 Threads API
  slug: spring-boot-3-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/openapi/spring-boot-3-threads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:spring-administration.pdl@broadcom.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spring.io
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: docs.spring.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spring Boot 3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Boot 3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Boot 3
provider_slug: spring-boot-3
slug: spring-boot-3-domain-security
source_filename: spring-boot-3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:spring-administration.pdl@broadcom.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-boot-3/refs/heads/main/security/spring-boot-3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Enterprise
- Framework
- Java
- Microservices
- REST API
- Spring Boot
---
