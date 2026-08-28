---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: campanja.com
  spf: true
hosts:
- host: campanja.com
  https: false
kind: domain-security
layout: security
method: probed
name: Campanja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Campanja, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Campanja
provider_slug: campanja
slug: campanja-domain-security
source_filename: campanja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: campanja.com\n  https: false\ndomains:\n- domain: campanja.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/campanja/refs/heads/main/security/campanja-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Advertising
- AdTech
- Search Advertising
- Bid Management
- Marketing Technology
- PPC
- Sweden
---
