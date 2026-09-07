---
api_specs:
- filename: eliq-auth-api-openapi.yaml
  format: yaml
  label: Eliq Auth API
  slug: auth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-auth-api-openapi.yaml
- filename: eliq-data-management-api-openapi.json
  format: json
  label: Eliq Data Management API
  slug: data-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-data-management-api-openapi.json
- filename: eliq-insights-api-openapi.yaml
  format: yaml
  label: Eliq Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-insights-api-openapi.yaml
- filename: eliq-intelligence-api-openapi.json
  format: json
  label: Eliq Intelligence API
  slug: intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/openapi/eliq-intelligence-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eliq.com
  spf: true
hosts:
- cert_expires: Nov 25 11:59:37 2026 GMT
  host: eliq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 15:00:19 2026 GMT
  host: developer.eliq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 04:26:54 2026 GMT
  host: auth-api.eliq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Eliq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eliq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eliq
provider_slug: eliq
slug: eliq-domain-security
source_filename: eliq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 11:59:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.eliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:00:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth-api.eliq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 04:26:54 2026 GMT\n  hsts: null\ndomains:\n- domain: eliq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eliq/refs/heads/main/security/eliq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Utilities
- Analytics
- Sustainability
- Energy Data
- Smart Meter
- Disaggregation
- Forecasting
- Segmentation
- Consumption
- Tariffs
- Insights
---
