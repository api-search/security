---
api_specs:
- filename: nasdaq-omx-group-openapi.yml
  format: yaml
  label: Nasdaq Data Link Time-series API
  slug: data-link-time-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq-omx-group/refs/heads/main/openapi/nasdaq-omx-group-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.nasdaq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
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
name: Nasdaq Omx Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nasdaq, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nasdaq
provider_slug: nasdaq-omx-group
slug: nasdaq-omx-group-domain-security
source_filename: nasdaq-omx-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: false\n- host: data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 16 01:27:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 09:28:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-omx-group/refs/heads/main/security/nasdaq-omx-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Capital Markets
- Stock Exchange
- Market Data
- Economics
- Fortune 1000
---
