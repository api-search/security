---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liveboard.online
  spf: true
hosts:
- cert_expires: Oct  3 18:06:22 2026 GMT
  host: liveboard.online
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liveboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liveboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liveboard
provider_slug: liveboard
slug: liveboard-domain-security
source_filename: liveboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liveboard.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:06:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: liveboard.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveboard/refs/heads/main/security/liveboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- Tutoring
- Virtual Classroom
- Online Whiteboard
- Scheduling
- Billing
- SaaS
---
