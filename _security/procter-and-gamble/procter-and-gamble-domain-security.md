---
api_specs:
- filename: procter-and-gamble-api-marketplace-openapi.yml
  format: yaml
  label: Procter & Gamble API Marketplace
  slug: api-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procter-and-gamble/refs/heads/main/openapi/procter-and-gamble-api-marketplace-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pg.com
  spf: true
hosts:
- cert_expires: Apr  2 23:59:59 2027 GMT
  host: developer.pg.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Procter And Gamble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Procter & Gamble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Procter & Gamble
provider_slug: procter-and-gamble
slug: procter-and-gamble-domain-security
source_filename: procter-and-gamble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.pg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procter-and-gamble/refs/heads/main/security/procter-and-gamble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Goods
- Manufacturing
- Retail
- Supply Chain
- Fortune 100
---
