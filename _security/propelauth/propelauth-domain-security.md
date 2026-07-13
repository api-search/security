---
api_specs:
- filename: propelauth-user-api-openapi.yml
  format: yaml
  label: PropelAuth User API
  slug: propelauth-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-user-api-openapi.yml
- filename: propelauth-org-api-openapi.yml
  format: yaml
  label: PropelAuth Organization API
  slug: propelauth-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-org-api-openapi.yml
- filename: propelauth-api-keys-api-openapi.yml
  format: yaml
  label: PropelAuth End-User API Keys API
  slug: propelauth-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-api-keys-api-openapi.yml
- filename: propelauth-oauth2-api-openapi.yml
  format: yaml
  label: PropelAuth OAuth2 API
  slug: propelauth-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-oauth2-api-openapi.yml
- filename: propelauth-mcp-api-openapi.yml
  format: yaml
  label: PropelAuth MCP Authentication API
  slug: propelauth-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/openapi/propelauth-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: propelauth.com
  spf: true
hosts:
- cert_expires: Sep 15 05:31:17 2026 GMT
  host: www.propelauth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 01:52:26 2026 GMT
  host: docs.propelauth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propelauth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PropelAuth, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PropelAuth
provider_slug: propelauth
slug: propelauth-domain-security
source_filename: propelauth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propelauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.propelauth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:52:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: propelauth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propelauth/refs/heads/main/security/propelauth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Identity
- B2B
- Multi-Tenancy
- Authorization
- RBAC
- SSO
- SCIM
- MCP
- API Keys
---
