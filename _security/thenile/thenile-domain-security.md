---
api_specs:
- filename: thenile-auth-api-openapi.yml
  format: yaml
  label: Nile Auth API
  slug: thenile-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-auth-api-openapi.yml
- filename: thenile-authentication-api-openapi.yml
  format: yaml
  label: Nile Authentication API
  slug: thenile-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-authentication-api-openapi.yml
- filename: thenile-compute-api-openapi.yml
  format: yaml
  label: Nile Compute API
  slug: thenile-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-compute-api-openapi.yml
- filename: thenile-credentials-api-openapi.yml
  format: yaml
  label: Nile Credentials API
  slug: thenile-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-credentials-api-openapi.yml
- filename: thenile-databases-api-openapi.yml
  format: yaml
  label: Nile Databases API
  slug: thenile-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-databases-api-openapi.yml
- filename: thenile-developers-api-openapi.yml
  format: yaml
  label: Nile Developers API
  slug: thenile-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-developers-api-openapi.yml
- filename: thenile-internal-api-openapi.yml
  format: yaml
  label: Nile Internal API
  slug: thenile-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-internal-api-openapi.yml
- filename: thenile-tenants-api-openapi.yml
  format: yaml
  label: Nile Tenants API
  slug: thenile-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-tenants-api-openapi.yml
- filename: thenile-users-api-openapi.yml
  format: yaml
  label: Nile Users API
  slug: thenile-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-users-api-openapi.yml
- filename: thenile-workspaces-api-openapi.yml
  format: yaml
  label: Nile Workspaces API
  slug: thenile-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/openapi/thenile-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thenile.dev
  spf: false
hosts:
- cert_expires: Nov 30 07:16:10 2026 GMT
  host: www.thenile.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thenile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nile
provider_slug: thenile
slug: thenile-domain-security
source_filename: thenile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thenile.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 07:16:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thenile.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thenile/refs/heads/main/security/thenile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Database
- PostgreSQL
- Serverless
- Multi-Tenant
- Authentication
- B2B SaaS
---
