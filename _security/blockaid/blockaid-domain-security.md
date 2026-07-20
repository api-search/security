---
api_specs:
- filename: blockaid-openapi-original.yml
  format: yaml
  label: Blockaid API
  slug: blockaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockaid/refs/heads/main/openapi/blockaid-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blockaid.io
  spf: true
hosts:
- cert_expires: Sep 28 18:35:38 2026 GMT
  host: blockaid.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:11:32 2026 GMT
  host: api.blockaid.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 21:03:31 2026 GMT
  host: client.blockaid.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockaid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Blockaid
provider_slug: blockaid
slug: blockaid-domain-security
source_filename: blockaid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockaid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:35:38 2026 GMT\n  hsts: false\n- host: api.blockaid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:11:32 2026 GMT\n  hsts: null\n- host: client.blockaid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:03:31 2026 GMT\n  hsts: null\ndomains:\n- domain: blockaid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockaid/refs/heads/main/security/blockaid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Web3 Security
- Blockchain
- Crypto
- Fraud Prevention
- Transaction Scanning
- Wallet Security
- Compliance
- Threat Detection
---
