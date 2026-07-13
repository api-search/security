---
api_specs:
- filename: checkout
  format: yaml
  label: Verifone Checkout API
  slug: verifone-checkout-api
  spec_type: OpenAPI
  url: https://docs.verifone.com/api-reference/open-api-references/checkout
- filename: ecommerce-api.json
  format: json
  label: Verifone eCommerce API
  slug: verifone-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verifone/refs/heads/main/openapi/ecommerce-api.json
- filename: customer
  format: yaml
  label: Verifone Customer API
  slug: verifone-customer-api
  spec_type: OpenAPI
  url: https://docs.verifone.com/api-reference/open-api-references/customer
- filename: order-service
  format: yaml
  label: Verifone Order Service API
  slug: verifone-order-service-api
  spec_type: OpenAPI
  url: https://docs.verifone.com/api-reference/open-api-references/order-service
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verifone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verifone.cloud
  spf: true
hosts:
- cert_expires: Oct  4 13:22:53 2026 GMT
  host: docs.verifone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: us.gsc.verifone.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: vhq.verifone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verifone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verifone, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verifone
provider_slug: verifone
slug: verifone-domain-security
source_filename: verifone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.verifone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:22:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: us.gsc.verifone.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\n- host: vhq.verifone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verifone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: verifone.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verifone/refs/heads/main/security/verifone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- POS
- Terminal Management
- eCommerce
- FinTech
- Payment Processing
- Omnichannel
---
