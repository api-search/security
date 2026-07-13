---
api_specs:
- filename: moralis-evm-api-openapi.json
  format: json
  label: Moralis EVM API
  slug: evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moralis/refs/heads/main/openapi/moralis-evm-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moralis.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moralis.io
  spf: true
hosts:
- cert_expires: Aug 18 16:43:28 2026 GMT
  host: moralis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 11:46:03 2026 GMT
  host: docs.moralis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:43:14 2026 GMT
  host: deep-index.moralis.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moralis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moralis, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moralis
provider_slug: moralis
slug: moralis-domain-security
source_filename: moralis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moralis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:43:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.moralis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:46:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: deep-index.moralis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:43:14 2026 GMT\n  hsts: null\ndomains:\n- domain: moralis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moralis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moralis/refs/heads/main/security/moralis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- Data API
- Streams
- Indexing
---
