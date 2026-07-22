---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: exa.market
  spf: false
hosts:
- cert_expires: Oct 14 05:32:51 2026 GMT
  host: exa.market
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exa Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exa Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Exa Finance
provider_slug: exa-finance
slug: exa-finance-domain-security
source_filename: exa-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exa.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:32:51 2026 GMT\n  hsts: false\ndomains:\n- domain: exa.market\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exa-finance/refs/heads/main/security/exa-finance-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Web3
- NFT
- Marketplace
- Algorand
- Smart Contracts
- Decentralized Finance
- Governance
- Digital Assets
---
