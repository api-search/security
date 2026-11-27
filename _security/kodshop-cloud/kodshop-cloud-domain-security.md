---
api_specs:
- filename: kodshop-cloud-public-api-openapi.yml
  format: yaml
  label: KodShop Public API
  slug: kodshop-cloud-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kodshop-cloud/openapi/kodshop-cloud-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kodshop.cloud
  spf: false
hosts:
- cert_expires: Feb  5 18:11:53 2027 GMT
  host: kodshop.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KodShop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KodShop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: KodShop
provider_slug: kodshop-cloud
slug: kodshop-cloud-domain-security
source_filename: kodshop-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kodshop.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 18:11:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kodshop.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kodshop-cloud/security/kodshop-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Digital Goods
- Gaming
- Payments
- Russia
---
