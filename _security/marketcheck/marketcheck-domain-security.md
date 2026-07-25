---
api_specs:
- filename: marketcheck-vin-decoder-api-openapi.yml
  format: yaml
  label: MarketCheck VIN Decoder API
  slug: marketcheck-vin-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-vin-decoder-api-openapi.yml
- filename: marketcheck-dealer-api-openapi.yml
  format: yaml
  label: MarketCheck Dealer API
  slug: marketcheck-dealer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-dealer-api-openapi.yml
- filename: marketcheck-dealer-api-openapi.yml
  format: yaml
  label: MarketCheck Dealer API
  slug: marketcheck-dealer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-dealer-api-openapi.yml
- filename: marketcheck-facets-api-openapi.yml
  format: yaml
  label: MarketCheck Facets API
  slug: marketcheck-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-facets-api-openapi.yml
- filename: marketcheck-graphs-api-openapi.yml
  format: yaml
  label: MarketCheck Graphs API
  slug: marketcheck-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-graphs-api-openapi.yml
- filename: marketcheck-history-api-openapi.yml
  format: yaml
  label: MarketCheck History API
  slug: marketcheck-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-history-api-openapi.yml
- filename: marketcheck-inventory-api-openapi.yml
  format: yaml
  label: MarketCheck Inventory API
  slug: marketcheck-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-inventory-api-openapi.yml
- filename: marketcheck-listings-api-openapi.yml
  format: yaml
  label: MarketCheck Listings API
  slug: marketcheck-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-listings-api-openapi.yml
- filename: marketcheck-market-api-openapi.yml
  format: yaml
  label: MarketCheck Market API
  slug: marketcheck-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-market-api-openapi.yml
- filename: marketcheck-vin-decoder-api-openapi.yml
  format: yaml
  label: MarketCheck VIN Decoder API
  slug: marketcheck-vin-decoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/openapi/marketcheck-vin-decoder-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketcheck.com
  spf: true
hosts:
- cert_expires: Sep  4 19:18:55 2026 GMT
  host: www.marketcheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: mc-api.marketcheck.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marketcheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketCheck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MarketCheck
provider_slug: marketcheck
slug: marketcheck-domain-security
source_filename: marketcheck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marketcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 19:18:55 2026 GMT\n  hsts: false\n- host: mc-api.marketcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: marketcheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marketcheck/refs/heads/main/security/marketcheck-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Vehicle Data
- VIN Decoder
- Car Inventory
- Market Data
- Dealer Inventory
- Vehicle Valuation
- Vehicle History
- Price Analytics
- Automotive Intelligence
---
