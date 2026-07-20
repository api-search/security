---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fluidity.money
  spf: true
hosts:
- cert_expires: Sep 14 05:25:12 2026 GMT
  host: fluidity.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fluidity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluidity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fluidity
provider_slug: fluidity
slug: fluidity-domain-security
source_filename: fluidity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluidity.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:25:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluidity.money\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluidity/refs/heads/main/security/fluidity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- DeFi
- GraphQL
- Ethereum
- Solana
- Blockchain
- Tokenization
- Rewards
---
