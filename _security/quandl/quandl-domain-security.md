---
api_specs:
- filename: nasdaq-data-link-timeseries-openapi.yml
  format: yaml
  label: Nasdaq Data Link REST API (Time-Series)
  slug: nasdaq-data-link-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandl/refs/heads/main/openapi/nasdaq-data-link-timeseries-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
hosts:
- cert_expires: Jul 16 01:27:07 2026 GMT
  host: data.nasdaq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 09:28:08 2026 GMT
  host: docs.data.nasdaq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quandl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quandl (Nasdaq Data Link), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quandl (Nasdaq Data Link)
provider_slug: quandl
slug: quandl-domain-security
source_filename: quandl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 16 01:27:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandl/refs/heads/main/security/quandl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Market Data
- Economic Data
- Time Series
- Streaming
---
