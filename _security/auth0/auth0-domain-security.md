---
api_specs:
- filename: auth0-management-api-openapi.yml
  format: yaml
  label: Auth0 Management API
  slug: auth0-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-management-api-openapi.yml
- filename: auth0-authentication-api-openapi.yml
  format: yaml
  label: Auth0 Authentication API
  slug: auth0-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-authentication-api-openapi.yml
- filename: auth0-fga-openapi.yml
  format: yaml
  label: Auth0 FGA (Fine-Grained Authorization)
  slug: auth0-fga
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-fga-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: auth0.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fga.dev
  spf: true
hosts:
- cert_expires: Sep 22 11:43:42 2026 GMT
  host: auth0.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:43:42 2026 GMT
  host: your-tenant.auth0.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 00:31:17 2026 GMT
  host: docs.fga.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auth0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auth0, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Auth0
provider_slug: auth0
slug: auth0-domain-security
source_filename: auth0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auth0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:43:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-tenant.auth0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:43:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fga.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: auth0.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: fga.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/security/auth0-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Authentication
- Authorization
- FGA
- Identity Management
- MCP
- OAuth
- Okta
- OpenID Connect
- SAML
- Security
- SCIM
---
