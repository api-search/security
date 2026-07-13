---
api_specs:
- filename: opencart-rest-api.yml
  format: yaml
  label: OpenCart REST API
  slug: opencart-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencart/refs/heads/main/openapi/opencart-rest-api.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opencart.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: yourstore.com
  spf: true
hosts:
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.opencart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 21:32:18 2026 GMT
  host: docs.opencart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 14:52:39 2027 GMT
  host: yourstore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCart, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenCart
provider_slug: opencart
slug: opencart-domain-security
source_filename: opencart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opencart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: docs.opencart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 21:32:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourstore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 14:52:39 2027 GMT\n  hsts: null\ndomains:\n- domain: opencart.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: yourstore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencart/refs/heads/main/security/opencart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Shopping Cart
- Open Source
- Self-Hosted
- Products
- Orders
- Customers
- Categories
---
