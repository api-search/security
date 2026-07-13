---
api_specs:
- filename: starknet-asyncapi.yml
  format: yaml
  label: Starknet JSON-RPC Specification
  slug: json-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/starknet/refs/heads/main/asyncapi/starknet-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: starknet.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blastapi.io
  spf: true
hosts:
- cert_expires: Aug 21 23:21:34 2026 GMT
  host: www.starknet.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 18:05:29 2026 GMT
  host: docs.starknet.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 03:42:57 2026 GMT
  host: starknet-mainnet.public.blastapi.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Starknet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Starknet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Starknet
provider_slug: starknet
slug: starknet-domain-security
source_filename: starknet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.starknet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:21:34 2026 GMT\n  hsts: false\n- host: docs.starknet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:05:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: starknet-mainnet.public.blastapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 03:42:57 2026 GMT\n  hsts: null\ndomains:\n- domain: starknet.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: blastapi.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starknet/refs/heads/main/security/starknet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Layer 2
- Ethereum
- Validity Rollup
- ZK
- Cairo
- STARK
- JSON-RPC
- Bridge
---
