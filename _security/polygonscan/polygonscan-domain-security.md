---
api_specs:
- filename: openapi.json
  format: json
  label: PolygonScan API
  slug: polygonscan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polygonscan/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: polygonscan.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: etherscan.io
  spf: true
hosts:
- cert_expires: Sep 26 04:30:28 2026 GMT
  host: polygonscan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 04:30:28 2026 GMT
  host: api.polygonscan.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polygonscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PolygonScan, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: PolygonScan
provider_slug: polygonscan
slug: polygonscan-domain-security
source_filename: polygonscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polygonscan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:30:28 2026 GMT\n  hsts: false\n- host: api.etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\n- host: api.polygonscan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:30:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: polygonscan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: etherscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polygonscan/refs/heads/main/security/polygonscan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Polygon
- Explorer
- Web3
- EVM
- Smart Contracts
- DeFi
- Cryptocurrency
---
