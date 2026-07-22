---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chingona.ventures
  spf: true
hosts:
- cert_expires: Oct 15 13:38:04 2026 GMT
  host: www.chingona.ventures
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chingona Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chingona Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chingona Ventures
provider_slug: chingona-ventures
slug: chingona-ventures-domain-security
source_filename: chingona-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chingona.ventures\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:38:04 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: chingona.ventures\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chingona-ventures/refs/heads/main/security/chingona-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Capital
- Pre-Seed
- Fintech
- Future of Work
- Future of Learning
- Health Technology
- Early Stage Investing
---
