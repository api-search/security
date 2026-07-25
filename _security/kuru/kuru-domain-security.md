---
api_specs:
- filename: kuru-generate-token-api-openapi.yml
  format: yaml
  label: Kuru Generate Token API
  slug: kuru-generate-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kuru/refs/heads/main/openapi/kuru-generate-token-api-openapi.yml
- filename: kuru-quote-api-openapi.yml
  format: yaml
  label: Kuru Quote API
  slug: kuru-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kuru/refs/heads/main/openapi/kuru-quote-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kuru.io
  spf: true
hosts:
- cert_expires: Sep  2 19:38:37 2026 GMT
  host: www.kuru.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 19:56:55 2026 GMT
  host: ws.kuru.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kuru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuru, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kuru
provider_slug: kuru
slug: kuru-domain-security
source_filename: kuru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kuru.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 19:38:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ws.kuru.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:56:55 2026 GMT\n  hsts: null\ndomains:\n- domain: kuru.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuru/refs/heads/main/security/kuru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- DeFi
- Decentralized Exchange
- Order Book
- Trading
- Blockchain
- Monad
- Liquidity
- Swaps
- Web3
---
