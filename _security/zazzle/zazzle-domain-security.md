---
api_specs:
- filename: zazzle-create-a-product-api-openapi.yml
  format: yaml
  label: Zazzle Create a Product API
  slug: zazzle-create-a-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/openapi/zazzle-create-a-product-api-openapi.yml
- filename: zazzle-realview-api-openapi.yml
  format: yaml
  label: Zazzle Real View API
  slug: zazzle-realview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/openapi/zazzle-realview-api-openapi.yml
- filename: zazzle-vendor-api-openapi.yml
  format: yaml
  label: Zazzle Vendor API
  slug: zazzle-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/openapi/zazzle-vendor-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@zazzle.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zazzle.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.zazzle.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: rlv.zazzle.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:59:59 2026 GMT
  host: makerhelp.zazzle.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zazzle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zazzle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zazzle
provider_slug: zazzle
slug: zazzle-domain-security
source_filename: zazzle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zazzle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: rlv.zazzle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: makerhelp.zazzle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: zazzle.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@zazzle.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zazzle/refs/heads/main/security/zazzle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Print On Demand
- Manufacturing
- Retail
- Affiliates
- Custom Products
- Order Management
- Shipping
---
