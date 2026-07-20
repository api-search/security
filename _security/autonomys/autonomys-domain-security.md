---
api_specs:
- filename: autonomys-auto-drive-openapi.json
  format: json
  label: Autonomys Auto Drive API
  slug: autonomys-auto-drive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autonomys/refs/heads/main/openapi/autonomys-auto-drive-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autonomys.xyz
  spf: true
hosts:
- cert_expires: Oct  2 23:43:07 2026 GMT
  host: www.autonomys.xyz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autonomys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autonomys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autonomys
provider_slug: autonomys
slug: autonomys-domain-security
source_filename: autonomys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autonomys.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: autonomys.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autonomys/refs/heads/main/security/autonomys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Blockchain
- Web3
- Decentralized Storage
- Storage
- AI Agents
- IPFS
- TypeScript SDK
---
