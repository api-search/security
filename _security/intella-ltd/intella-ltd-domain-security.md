---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intella.me
  spf: false
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: intella.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intella Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intella, LTD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Intella, LTD
provider_slug: intella-ltd
slug: intella-ltd-domain-security
source_filename: intella-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intella.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intella.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intella-ltd/refs/heads/main/security/intella-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Speech Recognition
- Speech to Text
- Voice AI
- Conversational AI
- Call Center Analytics
- Arabic NLP
- MENA
---
