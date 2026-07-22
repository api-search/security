---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: myarc.io
  spf: true
hosts:
- cert_expires: Sep 20 18:31:53 2026 GMT
  host: myarc.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Myarc Fitness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyARC Fitness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: MyARC Fitness
provider_slug: myarc-fitness
slug: myarc-fitness-domain-security
source_filename: myarc-fitness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myarc.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 18:31:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myarc.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myarc-fitness/refs/heads/main/security/myarc-fitness-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fitness
- Health and Wellness
- Creator Economy
- Coaching
- Mobile App
- SaaS
---
