---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thruster.finance
  spf: true
hosts:
- host: www.thruster.finance
  https: false
kind: domain-security
layout: security
method: probed
name: Thruster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thruster, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Thruster
provider_slug: thruster
slug: thruster-domain-security
source_filename: thruster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thruster.finance\n  https: false\ndomains:\n- domain: thruster.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thruster/refs/heads/main/security/thruster-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Crypto
- DeFi
- DEX
- Blast
- AMM
- Ethereum
---
