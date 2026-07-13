---
api_specs:
- filename: lit-protocol-core-v1-openapi.json
  format: json
  label: Lit Protocol Chipotle Express API (Core v1)
  slug: chipotle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lit-protocol/refs/heads/main/openapi/lit-protocol-core-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: litprotocol.com
  spf: true
hosts:
- cert_expires: Sep  3 07:57:47 2026 GMT
  host: www.litprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 13:29:56 2026 GMT
  host: developer.litprotocol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 02:20:26 2026 GMT
  host: api.chipotle.litprotocol.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lit Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lit Protocol, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lit Protocol
provider_slug: lit-protocol
slug: lit-protocol-domain-security
source_filename: lit-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.litprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:57:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.litprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:29:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.chipotle.litprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 02:20:26 2026 GMT\n  hsts: false\ndomains:\n- domain: litprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lit-protocol/refs/heads/main/security/lit-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3
- Key Management
- MPC
- Programmable Keys
- Lit Actions
---
