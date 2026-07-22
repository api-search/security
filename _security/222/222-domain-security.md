---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 222.place
  spf: true
hosts:
- cert_expires: Sep 15 12:28:15 2026 GMT
  host: 222.place
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 222 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 222, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: '222'
provider_slug: '222'
slug: 222-domain-security
source_filename: 222-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 222.place\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 222.place\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/222/refs/heads/main/security/222-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Social
- Community
- Events
- Mobile App
- Friendship
- Experiences
---
