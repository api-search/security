---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: keysino.cn
  spf: true
hosts:
- host: keysino.cn
  https: false
kind: domain-security
layout: security
method: probed
name: Keysino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for keysino, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: keysino
provider_slug: keysino
slug: keysino-domain-security
source_filename: keysino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keysino.cn\n  https: false\ndomains:\n- domain: keysino.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keysino/refs/heads/main/security/keysino-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
