---
api_specs:
- filename: halliday-openapi-original.yml
  format: yaml
  label: Halliday API V2
  slug: halliday-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halliday/refs/heads/main/openapi/halliday-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: halliday.xyz
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: v2.prod.halliday.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halliday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halliday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Halliday
provider_slug: halliday
slug: halliday-domain-security
source_filename: halliday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v2.prod.halliday.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: halliday.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halliday/refs/heads/main/security/halliday-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Cryptocurrency
- Blockchain
- Web3
- Onramp
- Swaps
- DeFi
- Agentic Workflows
- Fintech
---
