---
api_specs:
- filename: eodhd-eod-historical-data-openapi.yml
  format: yaml
  label: EODHD End-Of-Day Historical Data API
  slug: eod-historical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/openapi/eodhd-eod-historical-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eodhd.com
  spf: true
hosts:
- cert_expires: Sep 24 11:27:55 2026 GMT
  host: eodhd.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eodhd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EODHD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EODHD
provider_slug: eodhd
slug: eodhd-domain-security
source_filename: eodhd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eodhd.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 11:27:55 2026 GMT\n  hsts: false\ndomains:\n- domain: eodhd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eodhd/refs/heads/main/security/eodhd-domain-security.yml
summary_line: TLSv1.2
tags:
- Financial
- Market Data
- Stock Options
- Stocks
---
