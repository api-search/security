---
api_specs:
- filename: level2-hub-controller-openapi.json
  format: json
  label: Level2 Hub API
  slug: level2-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-hub-controller-openapi.json
- filename: level2-backtesting-api-openapi.yml
  format: yaml
  label: level2 Backtesting API
  slug: level2-backtesting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-backtesting-api-openapi.yml
- filename: level2-discovery-api-openapi.yml
  format: yaml
  label: level2 Discovery API
  slug: level2-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-discovery-api-openapi.yml
- filename: level2-market-data-api-openapi.yml
  format: yaml
  label: level2 Market Data API
  slug: level2-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-market-data-api-openapi.yml
- filename: level2-strategies-api-openapi.yml
  format: yaml
  label: level2 Strategies API
  slug: level2-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-strategies-api-openapi.yml
- filename: level2-technical-analysis-api-openapi.yml
  format: yaml
  label: level2 Technical Analysis API
  slug: level2-technical-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-technical-analysis-api-openapi.yml
- filename: level2-users-api-openapi.yml
  format: yaml
  label: level2 Users API
  slug: level2-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trylevel2.com
  spf: true
hosts:
- cert_expires: Nov 13 19:41:05 2026 GMT
  host: www.trylevel2.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 12:39:03 2026 GMT
  host: learn.trylevel2.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 15:25:58 2026 GMT
  host: hub2.trylevel2.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Level2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Level2, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Level2
provider_slug: level2
slug: level2-domain-security
source_filename: level2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trylevel2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 19:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: learn.trylevel2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 12:39:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: hub2.trylevel2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 15:25:58 2026 GMT\n  hsts: null\ndomains:\n- domain: trylevel2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/security/level2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trading
- Fintech
- Financial-Services
- Automation
- No-Code
- Backtesting
- Strategies
- Brokerage
- Market Data
- Prediction Markets
---
