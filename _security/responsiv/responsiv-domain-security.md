---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: responsiv.ai
  spf: true
hosts:
- cert_expires: Oct  4 12:10:58 2026 GMT
  host: responsiv.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Responsiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Responsiv, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Responsiv
provider_slug: responsiv
slug: responsiv-domain-security
source_filename: responsiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: responsiv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:10:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: responsiv.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/responsiv/refs/heads/main/security/responsiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applications
- Regulatory Compliance
- RegTech
- Governance Risk and Compliance
- Legal Research
- Artificial Intelligence
- Financial Services
- Insurance
---
