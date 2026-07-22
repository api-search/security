---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: one-chip.com
  spf: true
hosts:
- host: one-chip.com
  https: false
kind: domain-security
layout: security
method: probed
name: One Chip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for one-chip, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: one-chip
provider_slug: one-chip
slug: one-chip-domain-security
source_filename: one-chip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: one-chip.com\n  https: false\ndomains:\n- domain: one-chip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-chip/refs/heads/main/security/one-chip-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
