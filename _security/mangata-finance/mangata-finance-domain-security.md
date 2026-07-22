---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mangata.finance
  spf: true
hosts:
- host: mangata.finance
  https: false
kind: domain-security
layout: security
method: probed
name: Mangata Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mangata Finance, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mangata Finance
provider_slug: mangata-finance
slug: mangata-finance-domain-security
source_filename: mangata-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mangata.finance\n  https: false\ndomains:\n- domain: mangata.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mangata-finance/refs/heads/main/security/mangata-finance-domain-security.yml
summary_line: DMARC
tags:
- Company
- Defi
- Decentralized Exchange
- Blockchain
- Polkadot
- Substrate
- Trading
- SDK
---
