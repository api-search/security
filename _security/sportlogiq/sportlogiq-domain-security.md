---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sportlogiq.com
  spf: true
hosts:
- cert_expires: Aug 22 23:39:08 2026 GMT
  host: www.sportlogiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportlogiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sportlogiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sportlogiq
provider_slug: sportlogiq
slug: sportlogiq-domain-security
source_filename: sportlogiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sportlogiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:39:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sportlogiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportlogiq/refs/heads/main/security/sportlogiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Sports Analytics
- Computer Vision
- Machine Learning
- Artificial Intelligence
- Player Tracking
- Event Data
- Hockey
- Ice Hockey
- NHL
- Soccer
- Football
- NFL
- Youth Sports
- Broadcast
- Video Analytics
- Officiating
- Performance Analysis
---
