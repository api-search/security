---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: numina.co
  spf: true
hosts:
- host: numina.co
  https: false
kind: domain-security
layout: security
method: probed
name: Cty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numina, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Numina
provider_slug: cty
slug: cty-domain-security
source_filename: cty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numina.co\n  https: false\ndomains:\n- domain: numina.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cty/refs/heads/main/security/cty-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Mobility
- Urban Planning
- Smart Cities
- Computer Vision
- Transportation
- GraphQL
- Sensors
- Street Intelligence
---
