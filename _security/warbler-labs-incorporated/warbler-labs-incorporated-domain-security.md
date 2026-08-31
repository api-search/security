---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: warblerlabs.com
  spf: true
hosts:
- host: www.warblerlabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Warbler Labs Incorporated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warbler Labs Incorporated, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Warbler Labs Incorporated
provider_slug: warbler-labs-incorporated
slug: warbler-labs-incorporated-domain-security
source_filename: warbler-labs-incorporated-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.warblerlabs.com\n  https: false\ndomains:\n- domain: warblerlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warbler-labs-incorporated/refs/heads/main/security/warbler-labs-incorporated-domain-security.yml
summary_line: DMARC
tags:
- Company
- DeFi
- Blockchain
- Crypto
- Lending
- Credit
- Ethereum
- Web3
- Smart Contracts
- Identity
- Stablecoin
---
