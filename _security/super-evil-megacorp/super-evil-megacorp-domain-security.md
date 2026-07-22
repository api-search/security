---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: superevilmegacorp.com
  spf: true
hosts:
- cert_expires: Sep 14 16:33:46 2026 GMT
  host: superevilmegacorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Super Evil Megacorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super Evil Megacorp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Super Evil Megacorp
provider_slug: super-evil-megacorp
slug: super-evil-megacorp-domain-security
source_filename: super-evil-megacorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superevilmegacorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: superevilmegacorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-evil-megacorp/refs/heads/main/security/super-evil-megacorp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Games
- Gaming
- Video Games
- Game Studio
- Mobile Games
- Game Development
- Esports
---
