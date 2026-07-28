---
api_specs:
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Tariff API
  slug: genability-signal-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Load Serving Entity API
  slug: genability-signal-load-serving-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Territory API
  slug: genability-signal-territory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Cost Calculation API
  slug: genability-signal-cost-calculation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Smart Price API
  slug: genability-signal-smart-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Time of Use API
  slug: genability-signal-time-of-use-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Calendar API
  slug: genability-signal-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Season API
  slug: genability-signal-season-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Property and Lookup API
  slug: genability-signal-property-and-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Typical Baseline API
  slug: genability-signal-typical-baseline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal ZIP Code API
  slug: genability-signal-zip-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Utility Tax API
  slug: genability-signal-utility-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Organization Usage API
  slug: genability-signal-organization-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
- filename: genability-signal-openapi.json
  format: json
  label: Genability Signal Echo API
  slug: genability-signal-echo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/openapi/genability-signal-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genability.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arcadia.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: genability.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:20:02 2026 GMT
  host: docs.arcadia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.genability.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Genability Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genability, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Genability
provider_slug: genability
slug: genability-domain-security
source_filename: genability-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genability.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.arcadia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.genability.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: genability.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: arcadia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genability/refs/heads/main/security/genability-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Tariffs
- Energy Rates
- Rate Calculation
- Energy Data Platform
- Solar
- Grid
---
