---
api_specs:
- filename: topi-catalog-api-openapi.yml
  format: yaml
  label: Topi catalog API
  slug: topi-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-catalog-api-openapi.yml
- filename: topi-offer-api-openapi.yml
  format: yaml
  label: Topi offer API
  slug: topi-offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-offer-api-openapi.yml
- filename: topi-order-api-openapi.yml
  format: yaml
  label: Topi order API
  slug: topi-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-order-api-openapi.yml
- filename: topi-shipment-api-openapi.yml
  format: yaml
  label: Topi shipment API
  slug: topi-shipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-shipment-api-openapi.yml
- filename: topi-shippingmethod-api-openapi.yml
  format: yaml
  label: Topi shippingMethod API
  slug: topi-shippingmethod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/openapi/topi-shippingmethod-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: topi.eu
  spf: true
hosts:
- cert_expires: Sep 29 21:43:21 2026 GMT
  host: www.topi.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Topi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Topi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Topi
provider_slug: topi
slug: topi-domain-security
source_filename: topi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.topi.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:43:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: topi.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/topi/refs/heads/main/security/topi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Hardware as a Service
- Rental
- Embedded Finance
- B2B Payments
- Financing
- Checkout
- Germany
---
