---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: braid.network
  spf: true
hosts:
- host: braid.network
  https: false
kind: domain-security
layout: security
method: probed
name: Braid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braid, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Braid
provider_slug: braid
slug: braid-domain-security
source_filename: braid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: braid.network\n  https: false\ndomains:\n- domain: braid.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braid/refs/heads/main/security/braid-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Creator Economy
- Landing Pages
- Consumer
- Fintech
- Acquired
- Defunct
---
