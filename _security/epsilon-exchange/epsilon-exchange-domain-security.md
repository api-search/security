---
api_specs:
- filename: epsilon-exchange-api-openapi.json
  format: json
  label: Epsilon Public API API
  slug: epsilon-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epsilon-exchange/openapi/_original/epsilon-exchange-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epsilon.exchange
  spf: true
hosts:
- cert_expires: Feb  4 17:13:48 2027 GMT
  host: epsilon.exchange
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Epsilon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epsilon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Epsilon
provider_slug: epsilon-exchange
slug: epsilon-exchange-domain-security
source_filename: epsilon-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epsilon.exchange\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 17:13:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epsilon.exchange\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/epsilon-exchange/security/epsilon-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trading
- DeFi
- Cryptocurrency
- AdvancedOrders
- Robinhood Chain
---
