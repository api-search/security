---
api_specs:
- filename: spring-security-authorization-api-openapi.yml
  format: yaml
  label: Spring Security Authorization API
  slug: spring-security-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-authorization-api-openapi.yml
- filename: spring-security-client-management-api-openapi.yml
  format: yaml
  label: Spring Security Client Management API
  slug: spring-security-client-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-client-management-api-openapi.yml
- filename: spring-security-device-api-openapi.yml
  format: yaml
  label: Spring Security Device API
  slug: spring-security-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-device-api-openapi.yml
- filename: spring-security-discovery-api-openapi.yml
  format: yaml
  label: Spring Security Discovery API
  slug: spring-security-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-discovery-api-openapi.yml
- filename: spring-security-keys-api-openapi.yml
  format: yaml
  label: Spring Security Keys API
  slug: spring-security-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-keys-api-openapi.yml
- filename: spring-security-openid-connect-api-openapi.yml
  format: yaml
  label: Spring Security OpenID Connect API
  slug: spring-security-openid-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-openid-connect-api-openapi.yml
- filename: spring-security-session-api-openapi.yml
  format: yaml
  label: Spring Security Session API
  slug: spring-security-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-session-api-openapi.yml
- filename: spring-security-token-api-openapi.yml
  format: yaml
  label: Spring Security Token API
  slug: spring-security-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/openapi/spring-security-token-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:spring-administration.pdl@broadcom.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
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
name: Spring Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spring Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Spring Security
provider_slug: spring-security
slug: spring-security-domain-security
source_filename: spring-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.spring.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: spring.io\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:spring-administration.pdl@broadcom.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spring-security/refs/heads/main/security/spring-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Authorization
- Java
- JWT
- OAuth2
- OpenID Connect
- SAML
- Security
- Spring Framework
---
