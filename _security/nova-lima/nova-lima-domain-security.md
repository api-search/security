---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: runrun.it
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: runrun.it
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nova Lima Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nova Lima, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nova Lima
provider_slug: nova-lima
slug: nova-lima-domain-security
source_filename: nova-lima-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runrun.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: runrun.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-lima/refs/heads/main/security/nova-lima-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Project Management
- Task Management
- Work Management
- Productivity
- Time Tracking
- Team Collaboration
- SaaS
- Brazil
---
