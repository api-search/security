---
api_specs:
- filename: immutable-zkevm-openapi.json
  format: json
  label: Immutable zkEVM API
  slug: immutable-zkevm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-zkevm-openapi.json
- filename: immutable-audience-openapi.json
  format: json
  label: Immutable Audience API
  slug: immutable-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-audience-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immutable.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.immutable.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 20:58:09 2026 GMT
  host: docs.immutable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.immutable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Immutable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immutable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Immutable
provider_slug: immutable
slug: immutable-domain-security
source_filename: immutable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.immutable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: docs.immutable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 20:58:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.immutable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: immutable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/security/immutable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Blockchain
- NFT
- Web3
- Wallets
- Marketplace
- Analytics
- Attribution
- Customer Data Platform
- Authentication
- Developer Platform
---
