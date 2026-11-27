---
api_specs:
- filename: eterna-exchange-openapi-generated.yml
  format: yaml
  label: Eterna Exchange API
  slug: eterna-exchange-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eterna-exchange/openapi/_ae-authored/eterna-exchange-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eterna.exchange
  spf: true
hosts:
- cert_expires: Dec  8 17:42:55 2026 GMT
  host: eterna.exchange
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eterna Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eterna Exchange, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eterna Exchange
provider_slug: eterna-exchange
slug: eterna-exchange-domain-security
source_filename: eterna-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eterna.exchange\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 17:42:55 2026 GMT\n  hsts: false\ndomains:\n- domain: eterna.exchange\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/eterna-exchange/security/eterna-exchange-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Hybrid
- Perpetual Futures
- NoKYC
---
