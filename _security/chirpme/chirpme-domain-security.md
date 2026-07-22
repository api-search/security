---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chirpme.com
  spf: true
hosts:
- host: chirpme.com
  https: false
kind: domain-security
layout: security
method: probed
name: Chirpme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChirpMe, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ChirpMe
provider_slug: chirpme
slug: chirpme-domain-security
source_filename: chirpme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chirpme.com\n  https: false\ndomains:\n- domain: chirpme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chirpme/refs/heads/main/security/chirpme-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
