---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trannergy.com
  spf: true
hosts:
- host: trannergy.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trannergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trannergy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Trannergy
provider_slug: trannergy
slug: trannergy-domain-security
source_filename: trannergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trannergy.com\n  https: false\ndomains:\n- domain: trannergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/trannergy/security/trannergy-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Energy
- Analytics
- IoT
- Sustainability
- Utilities
- Company
---
