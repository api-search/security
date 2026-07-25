---
api_specs:
- filename: tally-forms-api-openapi.yml
  format: yaml
  label: Tally Forms API
  slug: tally-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-forms-api-openapi.yml
- filename: tally-organization-api-openapi.yml
  format: yaml
  label: Tally Organization API
  slug: tally-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-organization-api-openapi.yml
- filename: tally-submissions-api-openapi.yml
  format: yaml
  label: Tally Submissions API
  slug: tally-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-submissions-api-openapi.yml
- filename: tally-users-api-openapi.yml
  format: yaml
  label: Tally Users API
  slug: tally-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-users-api-openapi.yml
- filename: tally-webhooks-api-openapi.yml
  format: yaml
  label: Tally Webhooks API
  slug: tally-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-webhooks-api-openapi.yml
- filename: tally-workspaces-api-openapi.yml
  format: yaml
  label: Tally Workspaces API
  slug: tally-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/openapi/tally-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tally.so
  spf: true
hosts:
- cert_expires: Aug 29 20:56:57 2026 GMT
  host: tally.so
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 04:25:35 2026 GMT
  host: developers.tally.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 20:56:57 2026 GMT
  host: api.tally.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tally Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tally, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tally
provider_slug: tally
slug: tally-domain-security
source_filename: tally-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tally.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:56:57 2026 GMT\n  hsts: false\n- host: developers.tally.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:25:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tally.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:56:57 2026 GMT\n  hsts: null\ndomains:\n- domain: tally.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tally/refs/heads/main/security/tally-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Surveys
- No-Code
- Free
- Notion-style
- Webhooks
- MCP
---
