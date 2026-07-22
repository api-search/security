---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: diapers.com
  spf: true
hosts:
- host: www.diapers.com
  https: false
kind: domain-security
layout: security
method: probed
name: Diaperscom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diapers.com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Diapers.com
provider_slug: diaperscom
slug: diaperscom-domain-security
source_filename: diaperscom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diapers.com\n  https: false\ndomains:\n- domain: diapers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diaperscom/refs/heads/main/security/diaperscom-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Ecommerce
- Retail
- Baby Products
- Consumer Goods
- Online Shopping
---
