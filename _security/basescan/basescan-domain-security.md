---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Basescan API
  slug: basescan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: basescan.org
  spf: true
hosts:
- cert_expires: Sep 25 16:19:07 2026 GMT
  host: docs.basescan.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 16:19:07 2026 GMT
  host: api.basescan.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 16:19:07 2026 GMT
  host: api-sepolia.basescan.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basescan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basescan, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Basescan
provider_slug: basescan
slug: basescan-domain-security
source_filename: basescan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.basescan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:19:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.basescan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:19:07 2026 GMT\n  hsts: false\n- host: api-sepolia.basescan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:19:07 2026 GMT\n  hsts: false\ndomains:\n- domain: basescan.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basescan/refs/heads/main/security/basescan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- blockchain
- Base
- L2
- explorer
- Ethereum
- EVM
- transactions
- tokens
- smart contracts
---
