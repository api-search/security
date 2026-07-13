---
api_specs:
- filename: descope-openapi.yml
  format: yaml
  label: Descope Authentication API
  slug: descope-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope Management API
  slug: descope-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope OAuth Applications API
  slug: descope-oauth-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope SCIM 2.0 API
  slug: descope-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
- filename: descope-openapi.yml
  format: yaml
  label: Descope JWKS and Discovery API
  slug: descope-jwks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: descope.com
  spf: true
hosts:
- cert_expires: Sep 23 05:09:31 2026 GMT
  host: www.descope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 05:13:28 2026 GMT
  host: docs.descope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:08:04 2026 GMT
  host: api.descope.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Descope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Descope, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Descope
provider_slug: descope
slug: descope-domain-security
source_filename: descope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.descope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 05:09:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.descope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 05:13:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.descope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:08:04 2026 GMT\n  hsts: null\ndomains:\n- domain: descope.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/security/descope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Identity
- CIAM
- Passwordless
- Passkeys
- MFA
- SSO
- OAuth
- OIDC
- SAML
- SCIM
- Authorization
- FGA
- Agentic Identity
- MCP
---
