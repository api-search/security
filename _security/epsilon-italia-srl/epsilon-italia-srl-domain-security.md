---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: epsilon-italia.it
  spf: true
hosts:
- host: www.epsilon-italia.it
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Epsilon Italia Srl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epsilon Italia srl, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Epsilon Italia srl
provider_slug: epsilon-italia-srl
slug: epsilon-italia-srl-domain-security
source_filename: epsilon-italia-srl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epsilon-italia.it\n  https: false\ndomains:\n- domain: epsilon-italia.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/epsilon-italia-srl/security/epsilon-italia-srl-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Geospatial
- Consulting
- OGC
- INSPIRE
---
