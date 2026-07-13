---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Safe Transaction Service API
  slug: transaction-service
  spec_type: OpenAPI
  url: https://safe-transaction-mainnet.safe.global/api/schema/swagger-ui/
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: safe.global
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: safe.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: developer.safe.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: docs.safe.global
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gnosis Safe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safe (Gnosis Safe), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Safe (Gnosis Safe)
provider_slug: gnosis-safe
slug: gnosis-safe-domain-security
source_filename: gnosis-safe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safe.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.safe.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.safe.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: safe.global\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnosis-safe/refs/heads/main/security/gnosis-safe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Multisig
- Smart Contract
- Ethereum
- Web3
- Blockchain
- DeFi
- Safe
- Gnosis
- Wallet
---
