---
api_specs:
- filename: shippingeasy-customer-api-openapi.yml
  format: yaml
  label: ShippingEasy Customer API
  slug: shippingeasy-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shippingeasy/refs/heads/main/openapi/shippingeasy-customer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shippingeasy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 14 03:09:15 2026 GMT
  host: shippingeasy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: shippingeasy.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 19:14:31 2026 GMT
  host: app.shippingeasy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shippingeasy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShippingEasy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShippingEasy
provider_slug: shippingeasy
slug: shippingeasy-domain-security
source_filename: shippingeasy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shippingeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:09:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shippingeasy.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.shippingeasy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:14:31 2026 GMT\n  hsts: false\ndomains:\n- domain: shippingeasy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shippingeasy/refs/heads/main/security/shippingeasy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Logistics
- Multi-Carrier
- Labels
- Order Management
- Ecommerce
- Auctane
- Stamps.com
---
