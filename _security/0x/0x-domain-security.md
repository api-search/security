---
api_specs:
- filename: 0x-api.yaml
  format: yaml
  label: 0x Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Gasless API
  slug: gasless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-cross-chain.yaml
  format: yaml
  label: 0x Cross-Chain API
  slug: cross-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-cross-chain.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Trade Analytics API
  slug: trade-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
- filename: 0x-api.yaml
  format: yaml
  label: 0x Sources API
  slug: sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/openapi/0x-api.yaml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; validationmethods=dns-01"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org; validationmethods=dns-01,http-01"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: 0x.org
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: 0x.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:01:09 2026 GMT
  host: dashboard.0x.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 13:22:48 2026 GMT
  host: api.0x.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 0X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 0x, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: 0x
provider_slug: 0x
slug: 0x-domain-security
source_filename: 0x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 0x.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dashboard.0x.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:01:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.0x.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:22:48 2026 GMT\n  hsts: false\ndomains:\n- domain: 0x.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; validationmethods=dns-01\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org; validationmethods=dns-01,http-01\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/0x/refs/heads/main/security/0x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- DeFi
- DEX Aggregator
- Swap
- Gasless
- Cross-Chain
- Permit2
- Liquidity
- Trade Analytics
- Web3
- Settlement
- Smart Contracts
---
