---
api_specs:
- filename: api
  format: yaml
  label: Tenderly REST API
  slug: tenderly-rest-api
  spec_type: OpenAPI
  url: https://docs.tenderly.co/reference/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tenderly.co
  spf: true
hosts:
- cert_expires: Sep 24 15:33:17 2026 GMT
  host: tenderly.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 09:34:09 2026 GMT
  host: docs.tenderly.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 07:45:30 2026 GMT
  host: api.tenderly.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenderly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenderly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tenderly
provider_slug: tenderly
slug: tenderly-domain-security
source_filename: tenderly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenderly.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:33:17 2026 GMT\n  hsts: null\n- host: docs.tenderly.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:34:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tenderly.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:45:30 2026 GMT\n  hsts: null\ndomains:\n- domain: tenderly.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenderly/refs/heads/main/security/tenderly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Blockchain
- Smart Contracts
- Ethereum
- EVM
- Debugging
- Simulation
- Developer Tools
---
