---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getpellet.io
  spf: true
hosts:
- host: getpellet.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getpellet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pellet AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pellet AI
provider_slug: getpellet
slug: getpellet-domain-security
source_filename: getpellet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getpellet.io\n  https: false\ndomains:\n- domain: getpellet.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getpellet/refs/heads/main/security/getpellet-domain-security.yml
summary_line: DMARC
tags:
- Company
---
