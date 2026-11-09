---
api_specs:
- filename: cryptoetf-today-v1-openapi.json
  format: json
  label: CryptoETF API V1 API
  slug: cryptoetf-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoetf-today/openapi/_original/cryptoetf-today-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cryptoetf.today
  spf: true
hosts:
- cert_expires: Jan 26 14:52:45 2027 GMT
  host: cryptoetf.today
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cryptoetf Today Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CryptoETF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CryptoETF
provider_slug: cryptoetf-today
slug: cryptoetf-today-domain-security
source_filename: cryptoetf-today-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptoetf.today\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 14:52:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cryptoetf.today\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cryptoetf-today/security/cryptoetf-today-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- ETFs
- Market Data
- Analytics
- Finance
---
