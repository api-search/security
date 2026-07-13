---
api_specs:
- filename: block-square-api-openapi.yaml
  format: yaml
  label: Square API
  slug: block-square-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/openapi/block-square-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: block.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: squareup.com
  spf: true
hosts:
- cert_expires: Aug 20 15:48:54 2026 GMT
  host: www.block.xyz
  hsts: true
  hsts_max_age: 631152000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 09:11:31 2026 GMT
  host: developer.squareup.com
  hsts: true
  hsts_max_age: 631152000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:16:18 2026 GMT
  host: connect.squareup.com
  hsts: true
  hsts_max_age: 631152000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Block Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Block, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Block
provider_slug: block
slug: block-domain-security
source_filename: block-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.block.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 15:48:54 2026 GMT\n  hsts: true\n  hsts_max_age: 631152000\n- host: developer.squareup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 09:11:31 2026 GMT\n  hsts: true\n  hsts_max_age: 631152000\n- host: connect.squareup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:16:18 2026 GMT\n  hsts: true\n  hsts_max_age: 631152000\ndomains:\n- domain: block.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: squareup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/block/refs/heads/main/security/block-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Cryptocurrency
- eCommerce
- Fintech
- Payments
- Point Of Sale
- Square
---
