---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: realy.pro
  spf: true
hosts:
- host: realy.pro
  https: false
kind: domain-security
layout: security
method: probed
name: Realy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Realy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Realy
provider_slug: realy
slug: realy-domain-security
source_filename: realy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: realy.pro\n  https: false\ndomains:\n- domain: realy.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realy/refs/heads/main/security/realy-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Crypto Web3
- Blockchain
- Web3
- Cryptocurrency
---
