---
api_specs:
- filename: uniblock-unified-api-openapi.yml
  format: yaml
  label: Uniblock Unified API
  slug: unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/openapi/uniblock-unified-api-openapi.yml
- filename: uniblock-direct-api-openapi.yml
  format: yaml
  label: Uniblock Direct API
  slug: direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/openapi/uniblock-direct-api-openapi.yml
- filename: uniblock-json-rpc-api-openapi.yml
  format: yaml
  label: Uniblock JSON-RPC API
  slug: json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/openapi/uniblock-json-rpc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uniblock.dev
  spf: true
hosts:
- cert_expires: Aug 13 03:14:29 2026 GMT
  host: uniblock.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 21:07:54 2026 GMT
  host: docs.uniblock.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 20:02:19 2026 GMT
  host: api.uniblock.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uniblock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uniblock, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Uniblock
provider_slug: uniblock
slug: uniblock-domain-security
source_filename: uniblock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uniblock.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 03:14:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.uniblock.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:07:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.uniblock.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:02:19 2026 GMT\n  hsts: null\ndomains:\n- domain: uniblock.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uniblock/refs/heads/main/security/uniblock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Web3
---
