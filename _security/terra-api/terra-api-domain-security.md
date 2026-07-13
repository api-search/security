---
api_specs:
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Authentication API
  slug: terra-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra User Management API
  slug: terra-api-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Activity API
  slug: terra-api-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Body API
  slug: terra-api-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Daily API
  slug: terra-api-daily-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Sleep API
  slug: terra-api-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Nutrition API
  slug: terra-api-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Menstruation API
  slug: terra-api-menstruation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Athlete API
  slug: terra-api-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Integrations API
  slug: terra-api-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryterra.co
  spf: true
hosts:
- cert_expires: Aug 24 09:33:32 2026 GMT
  host: tryterra.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 05:29:42 2026 GMT
  host: docs.tryterra.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 04:31:31 2026 GMT
  host: api.tryterra.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terra Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Terra
provider_slug: terra-api
slug: terra-api-domain-security
source_filename: terra-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryterra.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:33:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tryterra.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 05:29:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tryterra.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 04:31:31 2026 GMT\n  hsts: null\ndomains:\n- domain: tryterra.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/security/terra-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wearables
- Health Data
- Fitness
- Aggregator
- Webhooks
- Digital Health
---
