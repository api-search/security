---
api_specs:
- filename: wincl-openapi-original.json
  format: json
  label: Wincl API
  slug: wincl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/openapi/wincl-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wincl.io
  spf: true
hosts:
- cert_expires: Sep  3 10:44:31 2026 GMT
  host: wincl.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wincl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WinCL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WinCL
provider_slug: wincl
slug: wincl-domain-security
source_filename: wincl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wincl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: wincl.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wincl/refs/heads/main/security/wincl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Carbon Management
- Sustainability
- Greenhouse Gas
- Carbon Credits
- Carbon Offset
- ESG
- Climate
- Marketplace
- Payments
- Blockchain
- Hedera
---
