---
api_specs:
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Spaces API
  slug: y42-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Orchestration API
  slug: y42-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Runs API
  slug: y42-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
- filename: y42-openapi.yml
  format: yaml
  label: Y42 Manifest API
  slug: y42-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/openapi/y42-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: y42.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep  1 15:56:29 2026 GMT
  host: www.y42.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: y42-public-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 12:33:57 2026 GMT
  host: api.y42.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Y42 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Y42, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Y42
provider_slug: y42
slug: y42-domain-security
source_filename: y42-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.y42.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:56:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: y42-public-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.y42.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:33:57 2026 GMT\n  hsts: null\ndomains:\n- domain: y42.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/y42/refs/heads/main/security/y42-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DataOps
- Data Pipelines
- Orchestration
- dbt
- Snowflake
- BigQuery
- GitOps
---
