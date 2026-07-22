---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digitalmortar.com
  spf: true
hosts:
- host: digitalmortar.com
  https: false
kind: domain-security
layout: security
method: probed
name: Digital Mortar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Mortar, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digital Mortar
provider_slug: digital-mortar
slug: digital-mortar-domain-security
source_filename: digital-mortar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalmortar.com\n  https: false\ndomains:\n- domain: digitalmortar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-mortar/refs/heads/main/security/digital-mortar-domain-security.yml
summary_line: DMARC
tags:
- Company
- Retail Analytics
- Location Analytics
- People Counting
- Queue Management
- Occupancy Analytics
- Computer Vision
- Shopper Journey
- Physical Retail
- SaaS
---
