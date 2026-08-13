---
api_specs:
- filename: crypto-com-exchange-openapi.yml
  format: yaml
  label: Crypto.com Exchange REST API v1
  slug: cryptocom-exchange-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/openapi/crypto-com-exchange-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crypto.com
  spf: true
hosts:
- cert_expires: Oct 26 02:33:53 2026 GMT
  host: crypto.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 06:04:11 2026 GMT
  host: exchange-developer.crypto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 06:04:11 2026 GMT
  host: api.crypto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crypto Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crypto.com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Crypto.com
provider_slug: crypto-com
slug: crypto-com-domain-security
source_filename: crypto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crypto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 02:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: exchange-developer.crypto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:04:11 2026 GMT\n  hsts: false\n- host: api.crypto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:04:11 2026 GMT\n  hsts: null\ndomains:\n- domain: crypto.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crypto-com/refs/heads/main/security/crypto-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- cryptocurrency
- crypto-exchange
- trading
- derivatives
- market-data
- digital-assets
- payments
- merchant-payments
- blockchain
- cronos
- defi
- staking
- fintech
- mcp
- agent-native
---
