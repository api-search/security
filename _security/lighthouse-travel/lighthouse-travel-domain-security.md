---
api_specs:
- filename: lighthouse-travel-demand-api-openapi.yml
  format: yaml
  label: Lighthouse Demand API
  slug: lighthouse-travel-demand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-demand-api-openapi.yml
- filename: lighthouse-travel-hotels-api-openapi.yml
  format: yaml
  label: Lighthouse Hotels API
  slug: lighthouse-travel-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-hotels-api-openapi.yml
- filename: lighthouse-travel-market-insight-api-openapi.yml
  format: yaml
  label: Lighthouse Market Insight API
  slug: lighthouse-travel-market-insight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-market-insight-api-openapi.yml
- filename: lighthouse-travel-markets-api-openapi.yml
  format: yaml
  label: Lighthouse Markets API
  slug: lighthouse-travel-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-markets-api-openapi.yml
- filename: lighthouse-travel-parity-api-openapi.yml
  format: yaml
  label: Lighthouse Parity API
  slug: lighthouse-travel-parity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-parity-api-openapi.yml
- filename: lighthouse-travel-ranking-api-openapi.yml
  format: yaml
  label: Lighthouse Ranking API
  slug: lighthouse-travel-ranking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-ranking-api-openapi.yml
- filename: lighthouse-travel-rates-api-openapi.yml
  format: yaml
  label: Lighthouse Rates API
  slug: lighthouse-travel-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-rates-api-openapi.yml
- filename: lighthouse-travel-reviews-api-openapi.yml
  format: yaml
  label: Lighthouse Reviews API
  slug: lighthouse-travel-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/openapi/lighthouse-travel-reviews-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issuewild "pki.goog"
  - 0 issue "Digicert.com"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mylighthouse.com
  spf: true
hosts:
- cert_expires: Aug  5 00:23:50 2026 GMT
  host: www.mylighthouse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 25 23:59:59 2026 GMT
  host: api.mylighthouse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lighthouse Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lighthouse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lighthouse
provider_slug: lighthouse-travel
slug: lighthouse-travel-domain-security
source_filename: lighthouse-travel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mylighthouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 00:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mylighthouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mylighthouse.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"Digicert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lighthouse-travel/refs/heads/main/security/lighthouse-travel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hospitality
- Hotels
- Travel
- Revenue Management
- Market Intelligence
- Business Intelligence
- Pricing
- Rate Shopping
- Competitive Intelligence
- Distribution
- Parity
- Channel Manager
- Demand Forecasting
- Software-as-a-Service
- Artificial Intelligence
---
