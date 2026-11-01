---
api_specs:
- filename: tickerall-com-accounts-api-openapi.yml
  format: yaml
  label: tickerall-com Accounts API
  slug: tickerall-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-accounts-api-openapi.yml
- filename: tickerall-com-bulk-api-openapi.yml
  format: yaml
  label: tickerall-com Bulk API
  slug: tickerall-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-bulk-api-openapi.yml
- filename: tickerall-com-candles-history-api-openapi.yml
  format: yaml
  label: tickerall-com Candles & History API
  slug: tickerall-com-candles-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-candles-history-api-openapi.yml
- filename: tickerall-com-copy-trading-api-openapi.yml
  format: yaml
  label: tickerall-com Copy Trading API
  slug: tickerall-com-copy-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-copy-trading-api-openapi.yml
- filename: tickerall-com-orders-api-openapi.yml
  format: yaml
  label: tickerall-com Orders API
  slug: tickerall-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-orders-api-openapi.yml
- filename: tickerall-com-sessions-api-openapi.yml
  format: yaml
  label: tickerall-com Sessions API
  slug: tickerall-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-sessions-api-openapi.yml
- filename: tickerall-com-symbols-api-openapi.yml
  format: yaml
  label: tickerall-com Symbols API
  slug: tickerall-com-symbols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-symbols-api-openapi.yml
- filename: tickerall-com-trade-history-api-openapi.yml
  format: yaml
  label: tickerall-com Trade History API
  slug: tickerall-com-trade-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tickerall-com/openapi/tickerall-com-trade-history-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tickerall.com
  spf: true
hosts:
- cert_expires: Jan 18 07:21:57 2027 GMT
  host: tickerall.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tickerall Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tickerall-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tickerall-com
provider_slug: tickerall-com
slug: tickerall-com-domain-security
source_filename: tickerall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tickerall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 07:21:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tickerall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tickerall-com/security/tickerall-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Trading
- API
- Forex
- MT5
- MT4
---
