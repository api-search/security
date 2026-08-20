---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trybraid.io
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: www.trybraid.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braid Social Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braid Social, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Braid Social
provider_slug: braid-social
slug: braid-social-domain-security
source_filename: braid-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trybraid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trybraid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braid-social/refs/heads/main/security/braid-social-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Engagement
- Slack
- Collaboration
- Team Building
- HR Tech
- Creator Economy
- Social
- Messaging
- Landing Pages
- Analytics
- Consumer
- Direct-to-Fan
- Software-as-a-Service
---
