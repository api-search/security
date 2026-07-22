---
api_specs:
- filename: syndicate-transaction-cloud-openapi-original.yml
  format: yaml
  label: Syndicate Transaction Cloud API
  slug: syndicate-transaction-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/openapi/syndicate-transaction-cloud-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: syndicate.io
  spf: true
hosts:
- cert_expires: Oct  3 21:22:34 2026 GMT
  host: syndicate.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 07:56:34 2026 GMT
  host: tc.docs.syndicate.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 06:25:51 2026 GMT
  host: api.syndicate.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Syndicate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syndicate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Syndicate
provider_slug: syndicate
slug: syndicate-domain-security
source_filename: syndicate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syndicate.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 21:22:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: tc.docs.syndicate.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 28 07:56:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.syndicate.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 06:25:51 2026 GMT\n  hsts: null\ndomains:\n- domain: syndicate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syndicate/refs/heads/main/security/syndicate-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Blockchain
- Web3
- Ethereum
- Transactions
- Wallets
- EVM
- Infrastructure
- Signing
- Webhooks
- Cryptography
---
