---
api_specs:
- filename: authlete-openapi-original.yml
  format: yaml
  label: Authlete API
  slug: authlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authlete/refs/heads/main/openapi/authlete-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: authlete.com
  spf: true
hosts:
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: authlete.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: us.authlete.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: jp.authlete.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authlete Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authlete, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Authlete
provider_slug: authlete
slug: authlete-domain-security
source_filename: authlete-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authlete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: false\n- host: us.authlete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: false\n- host: jp.authlete.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: authlete.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authlete/refs/heads/main/security/authlete-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- OAuth 2.0
- OpenID Connect
- Authentication
- Authorization
- Identity
- API Security
- FAPI
- Verifiable Credentials
- CIBA
---
