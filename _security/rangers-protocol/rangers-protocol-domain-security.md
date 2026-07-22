---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rangersprotocol.com
  spf: true
hosts:
- host: www.rangersprotocol.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rangers Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rangers Protocol, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rangers Protocol
provider_slug: rangers-protocol
slug: rangers-protocol-domain-security
source_filename: rangers-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rangersprotocol.com\n  https: false\ndomains:\n- domain: rangersprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rangers-protocol/refs/heads/main/security/rangers-protocol-domain-security.yml
summary_line: DMARC
tags:
- Company
- Crypto
- Blockchain
- Web3
- EVM
- Layer 1
- NFT
- Cross-Chain
- Oracle
- Gaming
---
