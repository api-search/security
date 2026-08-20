---
api_specs:
- filename: spring-boot-application-api-openapi.yml
  format: yaml
  label: Spring Boot Application API
  slug: spring-boot-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-application-api-openapi.yml
- filename: spring-boot-caches-api-openapi.yml
  format: yaml
  label: Spring Boot Caches API
  slug: spring-boot-caches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-caches-api-openapi.yml
- filename: spring-boot-configuration-api-openapi.yml
  format: yaml
  label: Spring Boot Configuration API
  slug: spring-boot-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-configuration-api-openapi.yml
- filename: spring-boot-environment-api-openapi.yml
  format: yaml
  label: Spring Boot Environment API
  slug: spring-boot-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-environment-api-openapi.yml
- filename: spring-boot-health-api-openapi.yml
  format: yaml
  label: Spring Boot Health API
  slug: spring-boot-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-health-api-openapi.yml
- filename: spring-boot-info-api-openapi.yml
  format: yaml
  label: Spring Boot Info API
  slug: spring-boot-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-info-api-openapi.yml
- filename: spring-boot-jvm-api-openapi.yml
  format: yaml
  label: Spring Boot JVM API
  slug: spring-boot-jvm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-jvm-api-openapi.yml
- filename: spring-boot-lifecycle-api-openapi.yml
  format: yaml
  label: Spring Boot Lifecycle API
  slug: spring-boot-lifecycle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-lifecycle-api-openapi.yml
- filename: spring-boot-loggers-api-openapi.yml
  format: yaml
  label: Spring Boot Loggers API
  slug: spring-boot-loggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-loggers-api-openapi.yml
- filename: spring-boot-metrics-api-openapi.yml
  format: yaml
  label: Spring Boot Metrics API
  slug: spring-boot-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/openapi/spring-boot-metrics-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:spring-administration.pdl@broadcom.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
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
name: Spring Boot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Boot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Boot
provider_slug: spring-boot
slug: spring-boot-domain-security
source_filename: spring-boot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:spring-administration.pdl@broadcom.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-boot/refs/heads/main/security/spring-boot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Auto-Configuration
- Embedded Server
- Framework
- Java
- Microservices
- REST API
- Spring
- Web Development
---
