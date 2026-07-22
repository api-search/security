---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blinkist.com
  spf: true
hosts:
- cert_expires: Oct 12 14:47:39 2026 GMT
  host: www.blinkist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blinkist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blinkist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blinkist
provider_slug: blinkist
slug: blinkist-domain-security
source_filename: blinkist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blinkist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:47:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blinkist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blinkist/refs/heads/main/security/blinkist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Learning
- Books
- Audiobooks
- Microlearning
- Productivity
- Subscription
- EdTech
- Mobile App
---
