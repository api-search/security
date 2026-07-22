---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amp.tech
  spf: true
hosts:
- host: amp.tech
  https: false
kind: domain-security
layout: security
method: probed
name: Aimip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aimip, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aimip
provider_slug: aimip
slug: aimip-domain-security
source_filename: aimip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amp.tech\n  https: false\ndomains:\n- domain: amp.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimip/refs/heads/main/security/aimip-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
