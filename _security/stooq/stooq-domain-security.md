---
api_specs:
- filename: stooq-historical-data-api-openapi.yml
  format: yaml
  label: Stooq Historical Data API
  slug: historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stooq/refs/heads/main/openapi/stooq-historical-data-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stooq.com
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: stooq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stooq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stooq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stooq
provider_slug: stooq
slug: stooq-domain-security
source_filename: stooq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stooq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: stooq.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stooq/refs/heads/main/security/stooq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Market Data
- Stocks
- Indices
- Currencies
- Crypto
- Commodities
- Historical Data
- Free
---
