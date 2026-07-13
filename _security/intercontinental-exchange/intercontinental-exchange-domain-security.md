---
api_specs:
- filename: ice-consolidated-feed-api-openapi.yml
  format: yaml
  label: ICE Consolidated Feed API
  slug: consolidated-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercontinental-exchange/refs/heads/main/openapi/ice-consolidated-feed-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: theice.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ice.com
  spf: true
hosts:
- cert_expires: Sep  6 23:41:37 2026 GMT
  host: developer.theice.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.ice.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.theice.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intercontinental Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intercontinental Exchange, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Intercontinental Exchange
provider_slug: intercontinental-exchange
slug: intercontinental-exchange-domain-security
source_filename: intercontinental-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.theice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:41:37 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: www.ice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: api.theice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: theice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intercontinental-exchange/refs/heads/main/security/intercontinental-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Commodities
- Financial Exchanges
- Market Data
- NYSE
- Trading
- Fortune 1000
---
