---
api_specs:
- filename: oumla-ltd-openapi-original.json
  format: json
  label: Oumla Core Server API
  slug: oumla-core-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/openapi/oumla-ltd-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oumla.com
  spf: true
hosts:
- cert_expires: Sep 13 08:26:27 2026 GMT
  host: oumla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 02:41:44 2026 GMT
  host: sandbox.oumla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oumla Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oumla Ltd, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oumla Ltd
provider_slug: oumla-ltd
slug: oumla-ltd-domain-security
source_filename: oumla-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oumla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:26:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sandbox.oumla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:41:44 2026 GMT\n  hsts: null\ndomains:\n- domain: oumla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oumla-ltd/refs/heads/main/security/oumla-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Digital Assets
- Wallet Infrastructure
- Custody
- Tokenization
- Smart Contracts
- Web3
- Fintech
- Saudi Arabia
---
