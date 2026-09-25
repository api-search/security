---
api_specs:
- filename: authelia-authentication-api-openapi.yml
  format: yaml
  label: Authelia Authentication API
  slug: authelia-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-authentication-api-openapi.yml
- filename: authelia-authorization-api-openapi.yml
  format: yaml
  label: Authelia Authorization API
  slug: authelia-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-authorization-api-openapi.yml
- filename: authelia-first-factor-api-openapi.yml
  format: yaml
  label: Authelia First Factor API
  slug: authelia-first-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-first-factor-api-openapi.yml
- filename: authelia-oauth-2-0-api-openapi.yml
  format: yaml
  label: Authelia OAuth 2.0 API
  slug: authelia-oauth-2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-oauth-2-0-api-openapi.yml
- filename: authelia-openid-connect-1-0-api-openapi.yml
  format: yaml
  label: Authelia OpenID Connect 1.0 API
  slug: authelia-openid-connect-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-openid-connect-1-0-api-openapi.yml
- filename: authelia-password-change-api-openapi.yml
  format: yaml
  label: Authelia Password Change API
  slug: authelia-password-change-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-password-change-api-openapi.yml
- filename: authelia-password-reset-api-openapi.yml
  format: yaml
  label: Authelia Password Reset API
  slug: authelia-password-reset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-password-reset-api-openapi.yml
- filename: authelia-second-factor-api-openapi.yml
  format: yaml
  label: Authelia Second Factor API
  slug: authelia-second-factor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-second-factor-api-openapi.yml
- filename: authelia-state-api-openapi.yml
  format: yaml
  label: Authelia State API
  slug: authelia-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-state-api-openapi.yml
- filename: authelia-user-elevation-api-openapi.yml
  format: yaml
  label: Authelia User Elevation API
  slug: authelia-user-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-user-elevation-api-openapi.yml
- filename: authelia-user-information-api-openapi.yml
  format: yaml
  label: Authelia User Information API
  slug: authelia-user-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-user-information-api-openapi.yml
- filename: authelia-utilities-api-openapi.yml
  format: yaml
  label: Authelia Utilities API
  slug: authelia-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/openapi/authelia-utilities-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: authelia.com
  spf: true
hosts:
- cert_expires: Nov 11 00:33:47 2026 GMT
  host: www.authelia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Authelia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authelia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Authelia
provider_slug: authelia
slug: authelia-domain-security
source_filename: authelia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.authelia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 00:33:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: authelia.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/security/authelia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open Source
- OpenID Connect
- Self-Hosted
- SSO
- Identity Federation
---
