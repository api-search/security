---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: card.io
  spf: true
hosts:
- host: www.card.io
  https: false
kind: domain-security
layout: security
method: probed
name: Cardio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for card.io, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: card.io
provider_slug: cardio
slug: cardio-domain-security
source_filename: cardio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.card.io\n  https: false\ndomains:\n- domain: card.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardio/refs/heads/main/security/cardio-domain-security.yml
summary_line: DMARC
tags:
- Company
- Payments
- Mobile
- SDK
- Credit Cards
- Computer Vision
- Card Scanning
- Defunct
---
