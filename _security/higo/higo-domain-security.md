---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: higo.io
  spf: true
hosts:
- host: higo.io
  https: false
kind: domain-security
layout: security
method: probed
name: Higo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Higo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Higo
provider_slug: higo
slug: higo-domain-security
source_filename: higo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: higo.io\n  https: false\ndomains:\n- domain: higo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/higo/refs/heads/main/security/higo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Payments
---
