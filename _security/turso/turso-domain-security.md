---
api_specs:
- filename: turso-auth-api-openapi.yml
  format: yaml
  label: Turso Auth API
  slug: turso-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-auth-api-openapi.yml
- filename: turso-locations-api-openapi.yml
  format: yaml
  label: Turso Locations API
  slug: turso-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-locations-api-openapi.yml
- filename: turso-organizations-api-openapi.yml
  format: yaml
  label: Turso Organizations API
  slug: turso-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-organizations-api-openapi.yml
- filename: turso-user-api-openapi.yml
  format: yaml
  label: Turso User API
  slug: turso-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/openapi/turso-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: turso.tech
  spf: true
hosts:
- cert_expires: Aug 17 15:15:38 2026 GMT
  host: turso.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 03:25:30 2026 GMT
  host: docs.turso.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.turso.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turso, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Turso
provider_slug: turso
slug: turso-domain-security
source_filename: turso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: turso.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.turso.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 03:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.turso.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: turso.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turso/refs/heads/main/security/turso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Edge Computing
- SQLite
- Developer Tools
- Multi-Tenant
- AI Agents
---
