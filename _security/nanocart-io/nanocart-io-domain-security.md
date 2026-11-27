---
api_specs:
- filename: nanocart-io-openapi-generated.yml
  format: yaml
  label: NanoCart API
  slug: nanocart-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanocart-io/openapi/_ae-authored/nanocart-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nanocart.io
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: nanocart.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NanoCart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NanoCart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NanoCart
provider_slug: nanocart-io
slug: nanocart-io-domain-security
source_filename: nanocart-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanocart.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nanocart.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nanocart-io/security/nanocart-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Checkout
- Artificial Intelligence
- Donations
- Storefront
---
