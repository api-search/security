---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: umoja.xyz
  spf: true
hosts:
- host: umoja.xyz
  https: false
kind: domain-security
layout: security
method: probed
name: Umoja Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umoja Labs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Umoja Labs
provider_slug: umoja-labs
slug: umoja-labs-domain-security
source_filename: umoja-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umoja.xyz\n  https: false\ndomains:\n- domain: umoja.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umoja-labs/refs/heads/main/security/umoja-labs-domain-security.yml
summary_line: DNSSEC
tags:
- Company
- Cryptocurrency
- DeFi
- Blockchain
- Yield
- Hedging
- Web3
---
