---
api_specs:
- filename: evm-swaps
  format: yaml
  label: KyberSwap Aggregator API
  slug: kyberswap-aggregator-api
  spec_type: OpenAPI
  url: https://docs.kyberswap.com/kyberswap-solutions/kyberswap-aggregator/aggregator-api-specification/evm-swaps
- filename: limit-order-api-specification
  format: yaml
  label: KyberSwap Limit Order API
  slug: kyberswap-limit-order-api
  spec_type: OpenAPI
  url: https://docs.kyberswap.com/kyberswap-solutions/limit-order/limit-order-api-specification
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kyberswap.com
  spf: true
hosts:
- cert_expires: Sep  6 22:59:05 2026 GMT
  host: docs.kyberswap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 23:30:27 2026 GMT
  host: aggregator-api.kyberswap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 23:30:27 2026 GMT
  host: limit-order.kyberswap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kyberswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KyberSwap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: KyberSwap
provider_slug: kyberswap
slug: kyberswap-domain-security
source_filename: kyberswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.kyberswap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:59:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: aggregator-api.kyberswap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:30:27 2026 GMT\n  hsts: null\n- host: limit-order.kyberswap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:30:27 2026 GMT\n  hsts: null\ndomains:\n- domain: kyberswap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyberswap/refs/heads/main/security/kyberswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- DEX
- Aggregator
- Swap
- Liquidity
- Blockchain
- Web3
- Multi-chain
- EVM
---
