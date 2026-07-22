---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gosmith.com
  spf: true
hosts:
- host: gosmith.com
  https: false
kind: domain-security
layout: security
method: probed
name: Smith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smith, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Smith
provider_slug: smith
slug: smith-domain-security
source_filename: smith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gosmith.com\n  https: false\ndomains:\n- domain: gosmith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smith/refs/heads/main/security/smith-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Home Improvement
- Home Services
- Marketplace
- Contractors
- Consumer
- Mobile App
---
