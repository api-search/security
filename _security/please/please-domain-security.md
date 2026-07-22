---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: please.ai
  spf: false
hosts:
- cert_expires: Sep 30 17:44:15 2026 GMT
  host: please.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Please Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Please, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Please
provider_slug: please
slug: please-domain-security
source_filename: please-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: please.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: please.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/please/refs/heads/main/security/please-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Reminders
- Productivity
- Artificial Intelligence
- Consumer App
- Mobile
- iOS
- Task Management
---
