---
api_specs:
- filename: syndica-io-asyncapi.yml
  format: yaml
  label: Syndica Solana RPC (WebSocket) API
  slug: syndica-solana-rpc-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndica-io/refs/heads/main/asyncapi/syndica-io-asyncapi.yml
- filename: syndica-io-asyncapi.yml
  format: yaml
  label: Syndica ChainStream API
  slug: syndica-chainstream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndica-io/refs/heads/main/asyncapi/syndica-io-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: syndica.io
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: syndica.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: docs.syndica.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: solana-mainnet.api.syndica.io
  https: false
kind: domain-security
layout: security
method: probed
name: Syndica Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syndica, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Syndica
provider_slug: syndica
slug: syndica-io-domain-security
source_filename: syndica-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syndica.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: docs.syndica.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: solana-mainnet.api.syndica.io\n  https: false\ndomains:\n- domain: syndica.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syndica/refs/heads/main/security/syndica-io-domain-security.yml
summary_line: TLSv1.2
tags:
- Solana
- Blockchain
- Web3
- RPC
- Streaming
- Infrastructure
- Validator
- Staking
---
