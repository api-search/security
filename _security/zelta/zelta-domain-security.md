---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zelta.ai
  spf: true
hosts:
- host: zelta.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Zelta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zelta, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zelta
provider_slug: zelta
slug: zelta-domain-security
source_filename: zelta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zelta.ai\n  https: false\ndomains:\n- domain: zelta.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zelta/refs/heads/main/security/zelta-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Techstars
---
