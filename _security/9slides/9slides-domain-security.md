---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 9slides.com
  spf: true
hosts:
- cert_expires: Sep 15 04:19:40 2026 GMT
  host: 9slides.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 9Slides Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 9Slides, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 9Slides
provider_slug: 9slides
slug: 9slides-domain-security
source_filename: 9slides-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 9slides.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:19:40 2026 GMT\n  hsts: null\ndomains:\n- domain: 9slides.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/9slides/refs/heads/main/security/9slides-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Presentations
- Video
- E-Learning
- Training
- Content Management
- SaaS
---
