---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: roadgoat.com
  spf: true
hosts:
- host: www.roadgoat.com
  https: false
kind: domain-security
layout: security
method: probed
name: Roadgoat Cities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RoadGoat Cities, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RoadGoat Cities
provider_slug: roadgoat-cities
slug: roadgoat-cities-domain-security
source_filename: roadgoat-cities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.roadgoat.com\n  https: false\ndomains:\n- domain: roadgoat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadgoat-cities/refs/heads/main/security/roadgoat-cities-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Geocoding
- Public APIs
---
