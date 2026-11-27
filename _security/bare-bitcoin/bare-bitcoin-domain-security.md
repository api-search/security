---
api_specs:
- filename: bare-bitcoin-developers-openapi.json
  format: json
  label: Bare Bitcoin API Developers API
  slug: bare-bitcoin-api-developers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bare-bitcoin/openapi/_original/bare-bitcoin-developers-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: barebitcoin.no
  spf: true
hosts:
- cert_expires: Jan  8 13:02:39 2027 GMT
  host: barebitcoin.no
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bare Bitcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bare Bitcoin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bare Bitcoin
provider_slug: bare-bitcoin
slug: bare-bitcoin-domain-security
source_filename: bare-bitcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barebitcoin.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 13:02:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: barebitcoin.no\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bare-bitcoin/security/bare-bitcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Finance
- Payments
- Norway
---
