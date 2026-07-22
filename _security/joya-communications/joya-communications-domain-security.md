---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marcopolo.me
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.marcopolo.me
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joya Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joya Communications, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Joya Communications
provider_slug: joya-communications
slug: joya-communications-domain-security
source_filename: joya-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marcopolo.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: marcopolo.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joya-communications/refs/heads/main/security/joya-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Video Chat
- Video Messaging
- Messaging
- Communications
- Consumer
- Privacy
- Mobile App
---
