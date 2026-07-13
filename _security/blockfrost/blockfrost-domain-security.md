---
api_specs:
- filename: blockfrost-openapi.yaml
  format: yaml
  label: Blockfrost API
  slug: blockfrost
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/openapi/blockfrost-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blockfrost.io
  spf: true
hosts:
- cert_expires: Sep 18 14:17:05 2026 GMT
  host: blockfrost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 14:17:05 2026 GMT
  host: cardano-mainnet.blockfrost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 14:02:20 2026 GMT
  host: cardano-preprod.blockfrost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockfrost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockfrost, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blockfrost
provider_slug: blockfrost
slug: blockfrost-domain-security
source_filename: blockfrost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockfrost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cardano-mainnet.blockfrost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:17:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cardano-preprod.blockfrost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 14:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blockfrost.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockfrost/refs/heads/main/security/blockfrost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Cardano
- Cryptocurrency
- DApps
- NFT
- Web3
---
