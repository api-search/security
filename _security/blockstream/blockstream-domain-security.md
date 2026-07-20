---
api_specs:
- filename: blockstream-esplora-openapi.yml
  format: yaml
  label: Blockstream Esplora HTTP API
  slug: blockstream-esplora-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/openapi/blockstream-esplora-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: blockstream.info
  spf: true
hosts:
- cert_expires: Oct  6 00:48:23 2026 GMT
  host: blockstream.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockstream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Blockstream
provider_slug: blockstream
slug: blockstream-domain-security
source_filename: blockstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockstream.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:48:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blockstream.info\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockstream/refs/heads/main/security/blockstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Bitcoin
- Blockchain
- Cryptocurrency
- Block Explorer
- Financial Services
- Infrastructure
---
