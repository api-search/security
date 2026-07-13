---
api_specs:
- filename: deliveroo-order-api-openapi.yml
  format: yaml
  label: Deliveroo Order API
  slug: order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-order-api-openapi.yml
- filename: deliveroo-menu-api-openapi.yml
  format: yaml
  label: Deliveroo Menu API
  slug: menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-menu-api-openapi.yml
- filename: deliveroo-site-api-openapi.yml
  format: yaml
  label: Deliveroo Site API
  slug: site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-site-api-openapi.yml
- filename: deliveroo-catalogue-api-openapi.yml
  format: yaml
  label: Deliveroo Catalogue API
  slug: catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-catalogue-api-openapi.yml
- filename: deliveroo-picking-api-openapi.yml
  format: yaml
  label: Deliveroo Picking API
  slug: picking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-picking-api-openapi.yml
- filename: deliveroo-signature-api-openapi.yml
  format: yaml
  label: Deliveroo Signature API
  slug: signature-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/openapi/deliveroo-signature-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deliveroo.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deliveroo.com
  spf: true
hosts:
- cert_expires: Aug 30 18:55:50 2026 GMT
  host: deliveroo.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 17:14:58 2026 GMT
  host: api-docs.deliveroo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 09:59:46 2026 GMT
  host: api.developers.deliveroo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deliveroo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deliveroo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deliveroo
provider_slug: deliveroo
slug: deliveroo-domain-security
source_filename: deliveroo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deliveroo.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:55:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.deliveroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:14:58 2026 GMT\n  hsts: null\n- host: api.developers.deliveroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:59:46 2026 GMT\n  hsts: null\ndomains:\n- domain: deliveroo.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: deliveroo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliveroo/refs/heads/main/security/deliveroo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food Delivery
- Grocery
- Marketplace
- Logistics
- Restaurants
---
