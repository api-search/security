---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pylonlending.com
  spf: true
hosts:
- cert_expires: Sep  8 22:47:52 2026 GMT
  host: pylonlending.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braid Lending Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pylon (formerly Braid Lending), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pylon (formerly Braid Lending)
provider_slug: braid-lending
slug: braid-lending-domain-security
source_filename: braid-lending-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pylonlending.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:47:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pylonlending.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braid-lending/refs/heads/main/security/braid-lending-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mortgage
- Lending
- Fintech
- Mortgage Origination
- Capital Markets
- Compliance
- API-First
- MCP-Native
---
