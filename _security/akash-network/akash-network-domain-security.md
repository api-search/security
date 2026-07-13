---
api_specs:
- filename: akash-network-openapi.yml
  format: yaml
  label: Akash Console API
  slug: console-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash-network/refs/heads/main/openapi/akash-network-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: akash.network
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudmos.io
  spf: false
hosts:
- cert_expires: Sep  3 18:16:30 2026 GMT
  host: akash.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 18:16:30 2026 GMT
  host: console.akash.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.cloudmos.io
  https: false
kind: domain-security
layout: security
method: probed
name: Akash Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akash Network, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Akash Network
provider_slug: akash-network
slug: akash-network-domain-security
source_filename: akash-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akash.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:16:30 2026 GMT\n  hsts: false\n- host: console.akash.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:16:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloudmos.io\n  https: false\ndomains:\n- domain: akash.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cloudmos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akash-network/refs/heads/main/security/akash-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Decentralized Cloud
- GPU
- Compute
- DePIN
- Cosmos
- Crypto
- Marketplace
---
