---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 51talk.ph
  spf: false
hosts:
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: 51talk.ph
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 51Talk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 51Talk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 51Talk
provider_slug: 51talk
slug: 51talk-domain-security
source_filename: 51talk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 51talk.ph\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 51talk.ph\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/51talk/refs/heads/main/security/51talk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Education
- EdTech
- Online Learning
- English Language
- E-Learning
- Tutoring
---
