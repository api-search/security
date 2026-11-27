---
api_specs:
- filename: himarket-hk-openapi-generated.yml
  format: yaml
  label: HiMarket API
  slug: himarket-hk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/himarket-hk/openapi/_ae-authored/himarket-hk-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: himarket.hk
  spf: true
hosts:
- cert_expires: Jan  1 11:22:47 2027 GMT
  host: himarket.hk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HiMarket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiMarket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HiMarket
provider_slug: himarket-hk
slug: himarket-hk-domain-security
source_filename: himarket-hk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: himarket.hk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 11:22:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: himarket.hk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/himarket-hk/security/himarket-hk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trading Cards
- Marketplace
- Riftbound
- Hong Kong
- Fixed‑price Listings
---
