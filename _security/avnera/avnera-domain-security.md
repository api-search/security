---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avnera.com
  spf: true
hosts:
- host: www.avnera.com
  https: false
kind: domain-security
layout: security
method: probed
name: Avnera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avnera, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Avnera
provider_slug: avnera
slug: avnera-domain-security
source_filename: avnera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avnera.com\n  https: false\ndomains:\n- domain: avnera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avnera/refs/heads/main/security/avnera-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Semiconductors
- Hardware
- Audio
- Analog
- Mixed-Signal
- Integrated Circuits
---
