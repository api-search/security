---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avec.ai
  spf: true
hosts:
- cert_expires: Sep  8 09:19:45 2026 GMT
  host: www.avec.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avec
provider_slug: avec
slug: avec-domain-security
source_filename: avec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avec.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:19:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avec.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avec/refs/heads/main/security/avec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Productivity
- Artificial Intelligence
- Gmail
- Email Management
- Consumer Application
- iOS
---
