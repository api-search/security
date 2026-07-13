---
api_specs:
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Holidays
  slug: holidays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Countries
  slug: countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Languages
  slug: languages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Workdays
  slug: workdays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: holidayapi.com
  spf: true
hosts:
- cert_expires: Sep  5 18:02:01 2026 GMT
  host: holidayapi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holidays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holiday API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Holiday API
provider_slug: holidays
slug: holidays-domain-security
source_filename: holidays-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: holidayapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 18:02:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: holidayapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/security/holidays-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Calendar
- Holidays
- Public Holidays
- Observances
- Reference Data
- Countries
- Languages
- Workdays
- Business Days
- Localization
---
