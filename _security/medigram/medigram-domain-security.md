---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medigram.com
  spf: true
hosts:
- cert_expires: Sep 10 13:33:15 2026 GMT
  host: www.medigram.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medigram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medigram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Medigram
provider_slug: medigram
slug: medigram-domain-security
source_filename: medigram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medigram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 13:33:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medigram.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medigram/refs/heads/main/security/medigram-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- AI Governance
- Clinical AI
- Compliance
- TIPPSS
- IEEE UL 2933
- Health IT
---
