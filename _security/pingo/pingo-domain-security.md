---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mypingoai.com
  spf: true
hosts:
- cert_expires: Oct 10 08:20:10 2026 GMT
  host: mypingoai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pingo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pingo AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pingo AI
provider_slug: pingo
slug: pingo-domain-security
source_filename: pingo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mypingoai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 08:20:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mypingoai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pingo/refs/heads/main/security/pingo-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Language Learning
- Education
- Conversational AI
- Mobile App
- EdTech
---
