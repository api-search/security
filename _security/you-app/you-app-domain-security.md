---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: you-app.com
  spf: true
hosts:
- cert_expires: Oct  5 12:19:40 2026 GMT
  host: you-app.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: You App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YOU-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: YOU-app
provider_slug: you-app
slug: you-app-domain-security
source_filename: you-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: you-app.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:19:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: you-app.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/you-app/refs/heads/main/security/you-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Wellbeing
- Health
- Wellness
- Mobile App
- Consumer
- Habit Tracking
- Acquired
---
