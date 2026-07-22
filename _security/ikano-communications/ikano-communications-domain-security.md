---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ikano.com
  spf: true
hosts:
- host: www.ikano.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ikano Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IKANO Communications, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IKANO Communications
provider_slug: ikano-communications
slug: ikano-communications-domain-security
source_filename: ikano-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ikano.com\n  https: false\ndomains:\n- domain: ikano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ikano-communications/refs/heads/main/security/ikano-communications-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Telecommunications
- Broadband
- Internet Service Provider
- Hosted Voice
- VoIP
---
