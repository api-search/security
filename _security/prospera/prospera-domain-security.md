---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prospera.ag
  spf: true
hosts:
- host: www.prospera.ag
  https: false
kind: domain-security
layout: security
method: probed
name: Prospera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prospera, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Prospera
provider_slug: prospera
slug: prospera-domain-security
source_filename: prospera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prospera.ag\n  https: false\ndomains:\n- domain: prospera.ag\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prospera/refs/heads/main/security/prospera-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Ai Ml
- Agriculture
- AgTech
- Machine Learning
- Computer Vision
- Crop Analytics
- Acquired
---
