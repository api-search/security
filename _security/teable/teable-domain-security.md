---
api_specs:
- filename: teable-openapi.yml
  format: yaml
  label: Teable Spaces API
  slug: teable-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Bases API
  slug: teable-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Tables API
  slug: teable-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Fields API
  slug: teable-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Records API
  slug: teable-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Views API
  slug: teable-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
- filename: teable-openapi.yml
  format: yaml
  label: Teable Attachments API
  slug: teable-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/openapi/teable-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teable.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teable.ai
  spf: true
hosts:
- cert_expires: Sep 14 19:21:25 2026 GMT
  host: teable.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 19:17:43 2026 GMT
  host: help.teable.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 03:01:27 2026 GMT
  host: app.teable.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teable, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Teable
provider_slug: teable
slug: teable-domain-security
source_filename: teable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:21:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.teable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:17:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.teable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 03:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: teable.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: teable.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teable/refs/heads/main/security/teable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No-Code
- Database
- Airtable Alternative
- Postgres
- Open Source
---
