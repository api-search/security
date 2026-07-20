---
api_specs:
- filename: dflow-openapi-original.json
  format: json
  label: DFlow Trading API (Aggregator)
  slug: dflow-trading-api-aggregator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/openapi/dflow-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dflow.net
  spf: true
hosts:
- cert_expires: Sep 12 03:03:49 2026 GMT
  host: dflow.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: quote-api.dflow.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DFlow, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DFlow
provider_slug: dflow
slug: dflow-domain-security
source_filename: dflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dflow.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: quote-api.dflow.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dflow.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dflow/refs/heads/main/security/dflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Solana
- Trading API
- DeFi
- DEX Aggregator
- Token Swap
- Blockchain
- MEV Protection
- Prediction Markets
- Agent Ready
---
