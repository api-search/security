---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: makerdao.com
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skyeco.com
  spf: true
hosts:
- cert_expires: Sep 17 04:12:00 2026 GMT
  host: makerdao.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 17:13:57 2026 GMT
  host: developers.skyeco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maker, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Maker
provider_slug: maker
slug: maker-domain-security
source_filename: maker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makerdao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:12:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.skyeco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 17:13:57 2026 GMT\n  hsts: false\ndomains:\n- domain: makerdao.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skyeco.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maker/refs/heads/main/security/maker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DeFi
- Blockchain
- Ethereum
- Stablecoin
- Smart Contracts
- Cryptocurrency
- Governance
- Web3
---
