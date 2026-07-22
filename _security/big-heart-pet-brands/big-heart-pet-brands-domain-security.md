---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigheartpet.com
  spf: true
hosts:
- host: www.bigheartpet.com
  https: false
kind: domain-security
layout: security
method: probed
name: Big Heart Pet Brands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Heart Pet Brands, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Big Heart Pet Brands
provider_slug: big-heart-pet-brands
slug: big-heart-pet-brands-domain-security
source_filename: big-heart-pet-brands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bigheartpet.com\n  https: false\ndomains:\n- domain: bigheartpet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-heart-pet-brands/refs/heads/main/security/big-heart-pet-brands-domain-security.yml
summary_line: DMARC
tags:
- Pet Food
- Consumer Goods
- Retail
- Acquired
- Pet Snacks
- CPG
---
