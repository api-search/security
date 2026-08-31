---
api_specs:
- filename: airtable-bases-api-openapi.yml
  format: yaml
  label: Airtable Bases API
  slug: airtable-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-bases-api-openapi.yml
- filename: airtable-comments-api-openapi.yml
  format: yaml
  label: Airtable Comments API
  slug: airtable-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-comments-api-openapi.yml
- filename: airtable-fields-api-openapi.yml
  format: yaml
  label: Airtable Fields API
  slug: airtable-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-fields-api-openapi.yml
- filename: airtable-groups-api-openapi.yml
  format: yaml
  label: Airtable Groups API
  slug: airtable-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-groups-api-openapi.yml
- filename: airtable-records-api-openapi.yml
  format: yaml
  label: Airtable Records API
  slug: airtable-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-records-api-openapi.yml
- filename: airtable-tables-api-openapi.yml
  format: yaml
  label: Airtable Tables API
  slug: airtable-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-tables-api-openapi.yml
- filename: airtable-users-api-openapi.yml
  format: yaml
  label: Airtable Users API
  slug: airtable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-users-api-openapi.yml
- filename: airtable-webhooks-api-openapi.yml
  format: yaml
  label: Airtable Webhooks API
  slug: airtable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airtable.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: airtable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.airtable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.airtable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Airtable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airtable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Airtable
provider_slug: airtable
slug: airtable-domain-security
source_filename: airtable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airtable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.airtable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.airtable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: airtable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/security/airtable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
---
