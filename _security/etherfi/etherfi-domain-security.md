---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ether.fi
  spf: true
hosts:
- cert_expires: Aug 12 08:37:43 2026 GMT
  host: www.ether.fi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Etherfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ether.fi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ether.fi
provider_slug: etherfi
slug: etherfi-domain-security
source_filename: etherfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ether.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 08:37:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ether.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etherfi/refs/heads/main/security/etherfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ethereum
- Liquid Restaking
- Liquid Staking
- Restaking
- LRT
- EigenLayer
- Symbiotic
- Karak
- DeFi
- Smart Contracts
- eETH
- weETH
- eBTC
- eUSD
- ETHFI
- AVS
- LayerZero
- Cross-Chain
- Cash Card
- Liquid Vaults
- Open Source
---
