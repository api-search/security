---
api_specs:
- filename: etherscan-openapi.yml
  format: yaml
  label: Etherscan API
  slug: etherscan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/openapi/etherscan-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: etherscan.io
  spf: true
hosts:
- cert_expires: Sep 20 03:43:38 2026 GMT
  host: etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 12:02:09 2026 GMT
  host: docs.etherscan.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.etherscan.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Etherscan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Etherscan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Etherscan
provider_slug: etherscan
slug: etherscan-domain-security
source_filename: etherscan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:43:38 2026 GMT\n  hsts: false\n- host: docs.etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:02:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.etherscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: etherscan.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etherscan/refs/heads/main/security/etherscan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- Ethereum
- EVM
- Web3
---
