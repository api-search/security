---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 1hai.cn
  spf: true
hosts:
- host: 1hai.cn
  https: false
kind: domain-security
layout: security
method: probed
name: 1Hai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1hai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 1hai
provider_slug: 1hai
slug: 1hai-domain-security
source_filename: 1hai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1hai.cn\n  https: false\ndomains:\n- domain: 1hai.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1hai/refs/heads/main/security/1hai-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Car Rental
- Mobility
- Transportation
- Travel
- China
- Automotive
---
