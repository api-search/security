---
api_specs:
- filename: futureverse-campaigns-api-openapi.yml
  format: yaml
  label: Futureverse Campaigns API
  slug: futureverse-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/openapi/futureverse-campaigns-api-openapi.yml
- filename: futureverse-quests-api-openapi.yml
  format: yaml
  label: Futureverse Quests API
  slug: futureverse-quests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/openapi/futureverse-quests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: futureverse.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: therootnetwork.com
  spf: false
hosts:
- host: www.futureverse.com
  https: false
- cert_expires: Oct 21 06:26:44 2026 GMT
  host: docs.therootnetwork.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: ar-api.futureverse.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Futureverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Futureverse, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Futureverse
provider_slug: futureverse
slug: futureverse-domain-security
source_filename: futureverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.futureverse.com\n  https: false\n- host: docs.therootnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 06:26:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ar-api.futureverse.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: futureverse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: therootnetwork.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/futureverse/refs/heads/main/security/futureverse-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Blockchain
- Web3
- Metaverse
- Digital Assets
- NFT
- GraphQL
- Identity
- OpenID Connect
- asset-registry
- Layer 1
- EVM
- Gaming
- agent-native
- MCP
---
