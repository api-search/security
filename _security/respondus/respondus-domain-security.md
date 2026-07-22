---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: respondus.com
  spf: true
hosts:
- cert_expires: Sep 15 00:16:22 2026 GMT
  host: web.respondus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Respondus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Respondus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Respondus
provider_slug: respondus
slug: respondus-domain-security
source_filename: respondus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web.respondus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: respondus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/respondus/refs/heads/main/security/respondus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Assessment
- Proctoring
- Online Exams
- LockDown Browser
- Respondus Monitor
- EdTech
- LTI
- LMS Integration
- Exam Integrity
---
