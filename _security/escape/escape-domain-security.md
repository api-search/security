---
api_specs:
- filename: escape-asm-api-openapi.yml
  format: yaml
  label: Escape Asm API
  slug: escape-asm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-asm-api-openapi.yml
- filename: escape-assets-api-openapi.yml
  format: yaml
  label: Escape Assets API
  slug: escape-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-assets-api-openapi.yml
- filename: escape-audit-api-openapi.yml
  format: yaml
  label: Escape Audit API
  slug: escape-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-audit-api-openapi.yml
- filename: escape-beta-api-openapi.yml
  format: yaml
  label: Escape Beta API
  slug: escape-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-beta-api-openapi.yml
- filename: escape-customrules-api-openapi.yml
  format: yaml
  label: Escape CustomRules API
  slug: escape-customrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-customrules-api-openapi.yml
- filename: escape-emails-api-openapi.yml
  format: yaml
  label: Escape Emails API
  slug: escape-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-emails-api-openapi.yml
- filename: escape-events-api-openapi.yml
  format: yaml
  label: Escape Events API
  slug: escape-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-events-api-openapi.yml
- filename: escape-integrations-api-openapi.yml
  format: yaml
  label: Escape Integrations API
  slug: escape-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-integrations-api-openapi.yml
- filename: escape-issues-api-openapi.yml
  format: yaml
  label: Escape Issues API
  slug: escape-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-issues-api-openapi.yml
- filename: escape-jobs-api-openapi.yml
  format: yaml
  label: Escape Jobs API
  slug: escape-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-jobs-api-openapi.yml
- filename: escape-locations-api-openapi.yml
  format: yaml
  label: Escape Locations API
  slug: escape-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-locations-api-openapi.yml
- filename: escape-profiles-api-openapi.yml
  format: yaml
  label: Escape Profiles API
  slug: escape-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-profiles-api-openapi.yml
- filename: escape-projects-api-openapi.yml
  format: yaml
  label: Escape Projects API
  slug: escape-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-projects-api-openapi.yml
- filename: escape-roles-api-openapi.yml
  format: yaml
  label: Escape Roles API
  slug: escape-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-roles-api-openapi.yml
- filename: escape-scans-api-openapi.yml
  format: yaml
  label: Escape Scans API
  slug: escape-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-scans-api-openapi.yml
- filename: escape-statistics-api-openapi.yml
  format: yaml
  label: Escape Statistics API
  slug: escape-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-statistics-api-openapi.yml
- filename: escape-tags-api-openapi.yml
  format: yaml
  label: Escape Tags API
  slug: escape-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-tags-api-openapi.yml
- filename: escape-upload-api-openapi.yml
  format: yaml
  label: Escape Upload API
  slug: escape-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-upload-api-openapi.yml
- filename: escape-users-api-openapi.yml
  format: yaml
  label: Escape Users API
  slug: escape-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-users-api-openapi.yml
- filename: escape-workflows-api-openapi.yml
  format: yaml
  label: Escape Workflows API
  slug: escape-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/openapi/escape-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: escape.tech
  spf: true
hosts:
- cert_expires: Aug 31 20:25:53 2026 GMT
  host: escape.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  9 13:30:49 2026 GMT
  host: docs.escape.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: public.escape.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Escape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Escape, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Escape
provider_slug: escape
slug: escape-domain-security
source_filename: escape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: escape.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:25:53 2026 GMT\n  hsts: false\n- host: docs.escape.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 13:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.escape.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: escape.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/escape/refs/heads/main/security/escape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Platform
- Security
---
