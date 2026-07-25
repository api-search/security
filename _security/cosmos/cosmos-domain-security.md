---
api_specs:
- filename: cosmos-query-api-openapi.yml
  format: yaml
  label: Cosmos Query API
  slug: cosmos-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmos/refs/heads/main/openapi/cosmos-query-api-openapi.yml
- filename: cosmos-service-api-openapi.yml
  format: yaml
  label: Cosmos Service API
  slug: cosmos-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmos/refs/heads/main/openapi/cosmos-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cosmos.network
  spf: true
hosts:
- cert_expires: Sep 28 04:56:56 2026 GMT
  host: docs.cosmos.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:46:44 2026 GMT
  host: lcd.cosmos.network
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:46:44 2026 GMT
  host: ibc.cosmos.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cosmos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cosmos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cosmos
provider_slug: cosmos
slug: cosmos-domain-security
source_filename: cosmos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.cosmos.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:56:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: lcd.cosmos.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:46:44 2026 GMT\n  hsts: null\n- host: ibc.cosmos.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:46:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cosmos.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmos/refs/heads/main/security/cosmos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Cosmos
- IBC
- Staking
- Governance
- DeFi
- Web3
---
