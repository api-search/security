---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: notional.finance
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
hosts:
- cert_expires: Oct  4 10:13:18 2026 GMT
  host: notional.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 02:47:01 2026 GMT
  host: docs.notional.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:49:39 2026 GMT
  host: api.thegraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notional Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Notional Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Notional Finance
provider_slug: notional
slug: notional-domain-security
source_filename: notional-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: notional.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:13:18 2026 GMT\n  hsts: false\n- host: docs.notional.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:47:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:49:39 2026 GMT\n  hsts: null\ndomains:\n- domain: notional.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notional/refs/heads/main/security/notional-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Fixed-Rate Lending
- Blockchain
- Ethereum
- Arbitrum
- fCash
- Liquidity Pools
- Leveraged Vaults
- Yield
- Web3
---
