---
api_specs:
- filename: hakuna-absences-api-openapi.yml
  format: yaml
  label: Hakuna Absences API
  slug: hakuna-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-absences-api-openapi.yml
- filename: hakuna-company-api-openapi.yml
  format: yaml
  label: Hakuna Company API
  slug: hakuna-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-company-api-openapi.yml
- filename: hakuna-management-api-openapi.yml
  format: yaml
  label: Hakuna Management API
  slug: hakuna-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-management-api-openapi.yml
- filename: hakuna-organization-api-openapi.yml
  format: yaml
  label: Hakuna Organization API
  slug: hakuna-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-organization-api-openapi.yml
- filename: hakuna-overview-api-openapi.yml
  format: yaml
  label: Hakuna Overview API
  slug: hakuna-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-overview-api-openapi.yml
- filename: hakuna-projects-api-openapi.yml
  format: yaml
  label: Hakuna Projects API
  slug: hakuna-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-projects-api-openapi.yml
- filename: hakuna-tasks-api-openapi.yml
  format: yaml
  label: Hakuna Tasks API
  slug: hakuna-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-tasks-api-openapi.yml
- filename: hakuna-time-entries-api-openapi.yml
  format: yaml
  label: Hakuna Time Entries API
  slug: hakuna-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-time-entries-api-openapi.yml
- filename: hakuna-timer-api-openapi.yml
  format: yaml
  label: Hakuna Timer API
  slug: hakuna-timer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-timer-api-openapi.yml
- filename: hakuna-users-api-openapi.yml
  format: yaml
  label: Hakuna Users API
  slug: hakuna-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/openapi/hakuna-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hakuna.ch
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.hakuna.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: app.hakuna.ch
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hakuna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hakuna, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hakuna
provider_slug: hakuna
slug: hakuna-domain-security
source_filename: hakuna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hakuna.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.hakuna.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hakuna.ch\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hakuna/refs/heads/main/security/hakuna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Time Tracking
- HR
- Workforce Management
- Absence Management
- Project Tracking
- SaaS
- Switzerland
- SME
---
