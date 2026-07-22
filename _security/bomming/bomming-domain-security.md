---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bomming.com
  spf: true
hosts:
- host: bomming.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bomming Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bomming, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: bomming
provider_slug: bomming
slug: bomming-domain-security
source_filename: bomming-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bomming.com\n  https: false\ndomains:\n- domain: bomming.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bomming/refs/heads/main/security/bomming-domain-security.yml
summary_line: DMARC
tags:
- Company
- Machine Vision
- Industrial Inspection
- 3D Sensors
- Optical Measurement
- Computer Vision
- Manufacturing
- Quality Control
- China
---
