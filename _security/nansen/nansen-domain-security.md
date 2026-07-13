---
api_specs:
- filename: nansen-openapi.yml
  format: yaml
  label: Nansen REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nansen/refs/heads/main/openapi/nansen-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nansen.ai
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.nansen.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 17:11:51 2026 GMT
  host: docs.nansen.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 01:56:08 2026 GMT
  host: api.nansen.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nansen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nansen, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nansen
provider_slug: nansen
slug: nansen-domain-security
source_filename: nansen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nansen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nansen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:11:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nansen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:56:08 2026 GMT\n  hsts: false\ndomains:\n- domain: nansen.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nansen/refs/heads/main/security/nansen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Crypto
- On-Chain
- Wallet Labels
- Smart Money
- Analytics
- Multi-chain
---
