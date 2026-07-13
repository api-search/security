---
api_specs:
- filename: arbitrum-asyncapi.yml
  format: yaml
  label: Arbitrum One JSON-RPC
  slug: one-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbitrum/refs/heads/main/asyncapi/arbitrum-asyncapi.yml
- filename: arbitrum-asyncapi.yml
  format: yaml
  label: Arbitrum Nova JSON-RPC
  slug: nova-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbitrum/refs/heads/main/asyncapi/arbitrum-asyncapi.yml
- filename: arbitrum-asyncapi.yml
  format: yaml
  label: Arbitrum Sepolia JSON-RPC
  slug: sepolia-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/arbitrum/refs/heads/main/asyncapi/arbitrum-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arbitrum.io
  spf: true
hosts:
- cert_expires: Oct  1 14:26:32 2026 GMT
  host: arbitrum.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:26:32 2026 GMT
  host: portal.arbitrum.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 02:59:23 2026 GMT
  host: docs.arbitrum.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arbitrum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbitrum, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arbitrum
provider_slug: arbitrum
slug: arbitrum-domain-security
source_filename: arbitrum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arbitrum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:26:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.arbitrum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:26:32 2026 GMT\n  hsts: null\n- host: docs.arbitrum.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:59:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arbitrum.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbitrum/refs/heads/main/security/arbitrum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Layer 2
- Ethereum
- Rollup
- JSON-RPC
- Stylus
- Nitro
- Orbit
- Bridge
---
