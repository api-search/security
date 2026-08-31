---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sonantic.io
  spf: true
hosts:
- host: www.sonantic.io
  https: false
kind: domain-security
layout: security
method: probed
name: Sonantic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonantic, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sonantic
provider_slug: sonantic
slug: sonantic-domain-security
source_filename: sonantic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sonantic.io\n  https: false\ndomains:\n- domain: sonantic.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonantic/refs/heads/main/security/sonantic-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Voice
- Text to Speech
- Emotive AI
- Acquired
- Spotify
- Audio
- Entertainment
- Historical
---
