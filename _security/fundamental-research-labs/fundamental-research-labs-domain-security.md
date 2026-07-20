---
api_specs:
- filename: fundamental-research-labs-openapi-original.json
  format: json
  label: Shortcut API
  slug: shortcut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fundamental-research-labs/refs/heads/main/openapi/fundamental-research-labs-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fundamentalresearchlabs.ai
  spf: false
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: shortcut.ai
  spf: true
hosts:
- cert_expires: Sep 14 01:05:58 2026 GMT
  host: fundamentalresearchlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: shortcut.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 01:30:43 2026 GMT
  host: api.shortcut.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fundamental Research Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fundamental Research Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fundamental Research Labs
provider_slug: fundamental-research-labs
slug: fundamental-research-labs-domain-security
source_filename: fundamental-research-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundamentalresearchlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:05:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: shortcut.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.shortcut.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:30:43 2026 GMT\n  hsts: null\ndomains:\n- domain: fundamentalresearchlabs.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: shortcut.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundamental-research-labs/refs/heads/main/security/fundamental-research-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Spreadsheets
- Excel
- Financial Modeling
- Agents
- Automation
- Productivity
- Data Analysis
---
