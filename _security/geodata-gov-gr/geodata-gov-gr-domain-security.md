---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geodata.gov.gr
  spf: true
hosts:
- host: geodata.gov.gr
  https: false
kind: domain-security
layout: security
method: probed
name: Geodata Gov Gr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geodata.gov.gr, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Geodata.gov.gr
provider_slug: geodata-gov-gr
slug: geodata-gov-gr-domain-security
source_filename: geodata-gov-gr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geodata.gov.gr\n  https: false\ndomains:\n- domain: geodata.gov.gr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geodata-gov-gr/refs/heads/main/security/geodata-gov-gr-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Geocoding
- Public APIs
---
