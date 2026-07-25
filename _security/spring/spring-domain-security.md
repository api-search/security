---
api_specs:
- filename: spring-beans-api-openapi.yml
  format: yaml
  label: Spring Framework Beans API
  slug: spring-beans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-beans-api-openapi.yml
- filename: spring-environment-api-openapi.yml
  format: yaml
  label: Spring Framework Environment API
  slug: spring-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-environment-api-openapi.yml
- filename: spring-health-api-openapi.yml
  format: yaml
  label: Spring Framework Health API
  slug: spring-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-health-api-openapi.yml
- filename: spring-info-api-openapi.yml
  format: yaml
  label: Spring Framework Info API
  slug: spring-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-info-api-openapi.yml
- filename: spring-loggers-api-openapi.yml
  format: yaml
  label: Spring Framework Loggers API
  slug: spring-loggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-loggers-api-openapi.yml
- filename: spring-mappings-api-openapi.yml
  format: yaml
  label: Spring Framework Mappings API
  slug: spring-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-mappings-api-openapi.yml
- filename: spring-metadata-api-openapi.yml
  format: yaml
  label: Spring Framework Metadata API
  slug: spring-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-metadata-api-openapi.yml
- filename: spring-metrics-api-openapi.yml
  format: yaml
  label: Spring Framework Metrics API
  slug: spring-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-metrics-api-openapi.yml
- filename: spring-project-generation-api-openapi.yml
  format: yaml
  label: Spring Framework Project Generation API
  slug: spring-project-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-project-generation-api-openapi.yml
- filename: spring-threads-api-openapi.yml
  format: yaml
  label: Spring Framework Threads API
  slug: spring-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/openapi/spring-threads-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
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
  host: start.spring.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Framework, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Framework
provider_slug: spring
slug: spring-domain-security
source_filename: spring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: start.spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring/refs/heads/main/security/spring-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Cloud Native
- Enterprise
- Framework
- Java
- Microservices
- Open Source
- REST
- Spring Boot
---
