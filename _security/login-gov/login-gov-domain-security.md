---
api_specs:
- filename: login-gov-oidc-openapi.yml
  format: yaml
  label: Login.gov OpenID Connect API
  slug: login-gov-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-oidc-openapi.yml
- filename: login-gov-saml-openapi.yml
  format: yaml
  label: Login.gov SAML 2.0 API
  slug: login-gov-saml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/openapi/login-gov-saml-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@login.gov"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: login.gov
  spf: true
hosts:
- cert_expires: Oct  4 10:20:38 2026 GMT
  host: www.login.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 13:21:19 2026 GMT
  host: developers.login.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: secure.login.gov
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Login Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Login.gov, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Login.gov
provider_slug: login-gov
slug: login-gov-domain-security
source_filename: login-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.login.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.login.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 13:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.login.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: login.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@login.gov\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/login-gov/refs/heads/main/security/login-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Federal
- GSA
- Identity
- Authentication
- SSO
- OIDC
- SAML
- IAL2
- AAL2
---
