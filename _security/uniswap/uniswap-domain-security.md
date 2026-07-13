---
api_specs:
- filename: uniswap-trading-openapi.yaml
  format: yaml
  label: Uniswap Trading API
  slug: uniswap-trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/openapi/uniswap-trading-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uniswap.org
  spf: true
hosts:
- cert_expires: Sep 13 23:13:31 2026 GMT
  host: developers.uniswap.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 21:34:21 2026 GMT
  host: docs.uniswap.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 18:39:18 2026 GMT
  host: trade-api.gateway.uniswap.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uniswap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uniswap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Uniswap
provider_slug: uniswap
slug: uniswap-domain-security
source_filename: uniswap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.uniswap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:13:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.uniswap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:34:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: trade-api.gateway.uniswap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:39:18 2026 GMT\n  hsts: null\ndomains:\n- domain: uniswap.org\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniswap/refs/heads/main/security/uniswap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- DeFi
- Decentralized Exchange
- Liquidity
- Swaps
---
