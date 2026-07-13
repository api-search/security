---
api_specs:
- filename: lowes-product-api-openapi.yml
  format: yaml
  label: Lowe's Product API
  slug: product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lowes/refs/heads/main/openapi/lowes-product-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "sectigo.com"
  - 128 issue "sectigo.com"
  - 128 iodef "mailto:SSL_Certificate_Management@lowes.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lowes.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: portal.apim.lowes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: www.lowes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: apis.lowes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lowes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lowe''s, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lowe's
provider_slug: lowes
slug: lowes-domain-security
source_filename: lowes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.apim.lowes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lowes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\n- host: apis.lowes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lowes.com\n  dnssec: false\n  caa:\n  - 128 issuewild \"sectigo.com\"\n  - 128 issue \"sectigo.com\"\n  - 128 iodef \"mailto:SSL_Certificate_Management@lowes.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lowes/refs/heads/main/security/lowes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ecommerce
- Home Improvement
- Products
- Retail
- Fortune 100
---
