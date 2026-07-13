---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Wormholescan API
  slug: wormholescan-api
  spec_type: OpenAPI
  url: https://docs.wormholescan.io/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wormhole.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wormholescan.io
  spf: false
hosts:
- cert_expires: Oct  8 04:06:25 2026 GMT
  host: wormhole.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.wormholescan.io
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.testnet.wormholescan.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wormhole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wormhole, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wormhole
provider_slug: wormhole
slug: wormhole-domain-security
source_filename: wormhole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wormhole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:06:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wormholescan.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\n- host: api.testnet.wormholescan.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wormhole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wormholescan.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wormhole/refs/heads/main/security/wormhole-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cross-Chain
- Blockchain
- Interoperability
- DeFi
- Token Transfers
- Messaging
- Web3
---
