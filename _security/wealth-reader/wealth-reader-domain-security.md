---
api_specs:
- filename: api-for-ai.yaml
  format: yaml
  label: Wealth Reader API
  slug: wealth-reader-api
  spec_type: OpenAPI
  url: https://www.wealthreader.com/api-reference/api-for-ai.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wealthreader.com
  spf: true
hosts:
- cert_expires: Oct 12 04:23:36 2026 GMT
  host: www.wealthreader.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api.wealthreader.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealth Reader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wealth Reader, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wealth Reader
provider_slug: wealth-reader
slug: wealth-reader-domain-security
source_filename: wealth-reader-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wealthreader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:23:36 2026 GMT\n  hsts: false\n- host: api.wealthreader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wealthreader.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-reader/refs/heads/main/security/wealth-reader-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Bank Aggregation
- Open Banking
- PSD2
- Financial Data
- Account Aggregation
- Investment Portfolios
- Wealth Management
- Banking
- Fintech
---
