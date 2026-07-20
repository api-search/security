---
api_specs:
- filename: komerce-shipping-cost-openapi.yml
  format: yaml
  label: RajaOngkir Shipping Cost API
  slug: shipping-cost
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-shipping-cost-openapi.yml
- filename: komerce-shipping-delivery-openapi.yml
  format: yaml
  label: Komerce Shipping Delivery API (Komship)
  slug: shipping-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-shipping-delivery-openapi.yml
- filename: komerce-payment-openapi.yml
  format: yaml
  label: Komerce Payment Service API
  slug: payment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-payment-openapi.yml
- filename: komerce-qrisly-openapi.yml
  format: yaml
  label: Komerce QRISLY API
  slug: qrisly
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/openapi/komerce-qrisly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: komerce.id
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rajaongkir.com
  spf: true
hosts:
- cert_expires: Oct  9 00:03:29 2026 GMT
  host: komerce.id
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 08:22:57 2026 GMT
  host: rajaongkir.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 00:03:29 2026 GMT
  host: rajaongkir.komerce.id
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Komerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Komerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Komerce
provider_slug: komerce
slug: komerce-domain-security
source_filename: komerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: komerce.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:03:29 2026 GMT\n  hsts: false\n- host: rajaongkir.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:22:57 2026 GMT\n  hsts: false\n- host: rajaongkir.komerce.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 00:03:29 2026 GMT\n  hsts: null\ndomains:\n- domain: komerce.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rajaongkir.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/komerce/refs/heads/main/security/komerce-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Shipping
- Logistics
- E-Commerce
- Payments
- QRIS
- Indonesia
- Couriers
- Tracking
- Fulfillment
---
