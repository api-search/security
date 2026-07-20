---
api_specs:
- filename: conduit-nodes-openapi.json
  format: json
  label: Conduit Nodes
  slug: conduit-nodes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conduit/refs/heads/main/openapi/conduit-nodes-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: conduit.xyz
  spf: true
hosts:
- cert_expires: Sep  6 00:16:30 2026 GMT
  host: conduit.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conduit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conduit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Conduit
provider_slug: conduit
slug: conduit-domain-security
source_filename: conduit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conduit.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:16:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: conduit.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conduit/refs/heads/main/security/conduit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Infrastructure
- Blockchain
- Rollups
- RPC Nodes
- Web3
- Ethereum
- Node Infrastructure
---
