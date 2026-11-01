---
api_specs:
- filename: birdeye-so-data-openapi-generated.yml
  format: yaml
  label: Birdeye (Solana data) data API
  slug: data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdeye-so/openapi/_ae-authored/birdeye-so-data-openapi-generated.yml
- filename: birdeye-so-resources-openapi-generated.yml
  format: yaml
  label: Birdeye (Solana data) resources API
  slug: resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/birdeye-so/openapi/_ae-authored/birdeye-so-resources-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: birdeye.so
  spf: true
hosts:
- cert_expires: Jan  4 12:30:36 2027 GMT
  host: birdeye.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Birdeye So Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Birdeye (Solana data), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Birdeye (Solana data)
provider_slug: birdeye-so
slug: birdeye-so-domain-security
source_filename: birdeye-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: birdeye.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 12:30:36 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: birdeye.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/birdeye-so/security/birdeye-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Data
- Analytics
- Token
---
