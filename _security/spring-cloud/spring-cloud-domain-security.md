---
api_specs:
- filename: spring-cloud-gateway-actuator-openapi.yml
  format: yaml
  label: Spring Cloud Gateway
  slug: spring-cloud-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-cloud/refs/heads/main/openapi/spring-cloud-gateway-actuator-openapi.yml
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
kind: domain-security
layout: security
method: probed
name: Spring Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Cloud
provider_slug: spring-cloud
slug: spring-cloud-domain-security
source_filename: spring-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-cloud/refs/heads/main/security/spring-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Circuit Breaker
- Cloud Native
- Distributed Systems
- Java
- Microservices
- Service Discovery
- Spring Framework
---
