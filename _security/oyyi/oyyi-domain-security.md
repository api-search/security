---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: oyyi.xyz
  spf: true
hosts:
- host: oyyi.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Oyyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for oyyi, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: oyyi
provider_slug: oyyi
slug: oyyi-domain-security
source_filename: oyyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oyyi.xyz\n  https: false\ndomains:\n- domain: oyyi.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oyyi/refs/heads/main/security/oyyi-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Development
- Public APIs
---
