---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medunes.net
  spf: true
hosts:
- host: battuta.medunes.net
  https: false
kind: domain-security
layout: security
method: probed
name: Battuta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Battuta, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Battuta
provider_slug: battuta
slug: battuta-domain-security
source_filename: battuta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: battuta.medunes.net\n  https: false\ndomains:\n- domain: medunes.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/battuta/refs/heads/main/security/battuta-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Geocoding
- Public APIs
---
