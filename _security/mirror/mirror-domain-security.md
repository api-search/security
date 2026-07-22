---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mirror.finance
  spf: true
hosts:
- host: mirror.finance
  https: false
kind: domain-security
layout: security
method: probed
name: Mirror Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirror, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mirror
provider_slug: mirror
slug: mirror-domain-security
source_filename: mirror-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mirror.finance\n  https: false\ndomains:\n- domain: mirror.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirror/refs/heads/main/security/mirror-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- DeFi
- Cryptocurrency
- Blockchain
- Synthetic Assets
- GraphQL
- Terra
- Web3
- Financial Services
---
