---
api_specs:
- filename: tendermint-rpc-openapi-original.yml
  format: yaml
  label: Tendermint RPC
  slug: tendermint-rpc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tendermint/refs/heads/main/openapi/tendermint-rpc-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tendermint.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmos.network
  spf: true
hosts:
- cert_expires: Oct 12 21:13:48 2026 GMT
  host: tendermint.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 05:48:49 2026 GMT
  host: docs.tendermint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:46:44 2026 GMT
  host: rpc.cosmos.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tendermint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tendermint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: Tendermint
provider_slug: tendermint
slug: tendermint-domain-security
source_filename: tendermint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tendermint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:13:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tendermint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:48:49 2026 GMT\n  hsts: false\n- host: rpc.cosmos.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:46:44 2026 GMT\n  hsts: null\ndomains:\n- domain: tendermint.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cosmos.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tendermint/refs/heads/main/security/tendermint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Infrastructure
- Blockchain
- Consensus
- Cosmos
- Web3
- JSON-RPC
- Node
---
