---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caliberstrong.com
  spf: true
hosts:
- cert_expires: Aug 23 01:03:05 2026 GMT
  host: caliberstrong.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caliber Fitness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caliber Fitness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Caliber Fitness
provider_slug: caliber-fitness
slug: caliber-fitness-domain-security
source_filename: caliber-fitness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caliberstrong.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 01:03:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: caliberstrong.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caliber-fitness/refs/heads/main/security/caliber-fitness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fitness
- Health
- Strength Training
- Coaching
- Nutrition
- Mobile App
---
