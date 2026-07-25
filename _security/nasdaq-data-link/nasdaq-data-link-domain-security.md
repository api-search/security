---
api_specs:
- filename: postman
  format: yaml
  label: Nasdaq Data Link REST API for Real-Time or Delayed Data
  slug: nasdaq-data-link-rest-api-for-real-time-or-delayed-data
  spec_type: Postman
  url: https://github.com/Nasdaq/NasdaqCloudDataService-REST-API/tree/main/restapi/postman
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
hosts:
- cert_expires: Oct 11 01:52:45 2026 GMT
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
name: Nasdaq Data Link Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nasdaq Data Link, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nasdaq Data Link
provider_slug: nasdaq-data-link
slug: nasdaq-data-link-domain-security
source_filename: nasdaq-data-link-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 01:52:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-data-link/refs/heads/main/security/nasdaq-data-link-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Data
- Stock Market
- Market Data
- Economic Data
- Alternative Data
- Time Series
- Open Data
- Public APIs
---
