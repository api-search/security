---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: simsim.in
  spf: true
hosts:
- host: simsim.in
  https: false
kind: domain-security
layout: security
method: probed
name: Simsim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for simsim, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: simsim
provider_slug: simsim
slug: simsim-domain-security
source_filename: simsim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simsim.in\n  https: false\ndomains:\n- domain: simsim.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simsim/refs/heads/main/security/simsim-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Social Commerce
- Video Commerce
- E-commerce
- India
- Acquired
---
