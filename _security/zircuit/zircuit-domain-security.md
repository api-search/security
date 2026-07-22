---
api_specs:
- filename: zircuit-gud-trading-engine-openapi.yml
  format: yaml
  label: Zircuit GUD Trading Engine API (Beta)
  slug: zircuit-gud-trading-engine-api-beta
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zircuit/refs/heads/main/openapi/zircuit-gud-trading-engine-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zircuit.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.zircuit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 17:57:01 2026 GMT
  host: docs.zircuit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: mainnet.zircuit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zircuit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zircuit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zircuit
provider_slug: zircuit
slug: zircuit-domain-security
source_filename: zircuit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zircuit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.zircuit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mainnet.zircuit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zircuit.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zircuit/refs/heads/main/security/zircuit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Layer 2
- Rollup
- Zero Knowledge
- EVM
- DeFi
- JSON-RPC
- Web3
---
