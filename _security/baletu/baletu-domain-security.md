---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baletu.com
  spf: true
hosts:
- host: baletu.com
  https: false
kind: domain-security
layout: security
method: probed
name: Baletu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baletu, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Baletu
provider_slug: baletu
slug: baletu-domain-security
source_filename: baletu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baletu.com\n  https: false\ndomains:\n- domain: baletu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baletu/refs/heads/main/security/baletu-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Real Estate
- Rental Housing
- Proptech
- Marketplace
- China
- Mobile
---
