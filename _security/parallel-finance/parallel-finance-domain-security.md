---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: parallel.fi
  spf: true
hosts:
- host: rpc.parallel.fi
  https: false
kind: domain-security
layout: security
method: probed
name: Parallel Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parallel Finance, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Parallel Finance
provider_slug: parallel-finance
slug: parallel-finance-domain-security
source_filename: parallel-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rpc.parallel.fi\n  https: false\ndomains:\n- domain: parallel.fi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parallel-finance/refs/heads/main/security/parallel-finance-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- DeFi
- Blockchain
- Polkadot
- Lending
- Staking
- Money Market
- Substrate
- Web3
- Cryptocurrency
---
