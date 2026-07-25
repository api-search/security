---
api_specs:
- filename: deliverart-addresses-api-openapi.yml
  format: yaml
  label: Deliverart Addresses API
  slug: deliverart-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-addresses-api-openapi.yml
- filename: deliverart-companies-api-openapi.yml
  format: yaml
  label: Deliverart Companies API
  slug: deliverart-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-companies-api-openapi.yml
- filename: deliverart-customer-addresses-api-openapi.yml
  format: yaml
  label: Deliverart Customer addresses API
  slug: deliverart-customer-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-customer-addresses-api-openapi.yml
- filename: deliverart-customer-business-profiles-api-openapi.yml
  format: yaml
  label: Deliverart Customer business profiles API
  slug: deliverart-customer-business-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-customer-business-profiles-api-openapi.yml
- filename: deliverart-customers-api-openapi.yml
  format: yaml
  label: Deliverart Customers API
  slug: deliverart-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-customers-api-openapi.yml
- filename: deliverart-deliveries-api-openapi.yml
  format: yaml
  label: Deliverart Deliveries API
  slug: deliverart-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-deliveries-api-openapi.yml
- filename: deliverart-delivery-fee-api-openapi.yml
  format: yaml
  label: Deliverart Delivery fee API
  slug: deliverart-delivery-fee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-delivery-fee-api-openapi.yml
- filename: deliverart-me-api-openapi.yml
  format: yaml
  label: Deliverart Me API
  slug: deliverart-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-me-api-openapi.yml
- filename: deliverart-menu-api-openapi.yml
  format: yaml
  label: Deliverart Menu API
  slug: deliverart-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-menu-api-openapi.yml
- filename: deliverart-orders-api-openapi.yml
  format: yaml
  label: Deliverart Orders API
  slug: deliverart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-orders-api-openapi.yml
- filename: deliverart-password-reset-api-openapi.yml
  format: yaml
  label: Deliverart Password reset API
  slug: deliverart-password-reset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-password-reset-api-openapi.yml
- filename: deliverart-points-of-sale-api-openapi.yml
  format: yaml
  label: Deliverart Points of sale API
  slug: deliverart-points-of-sale-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-points-of-sale-api-openapi.yml
- filename: deliverart-registration-api-openapi.yml
  format: yaml
  label: Deliverart Registration API
  slug: deliverart-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-registration-api-openapi.yml
- filename: deliverart-reservation-api-openapi.yml
  format: yaml
  label: Deliverart Reservation API
  slug: deliverart-reservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-reservation-api-openapi.yml
- filename: deliverart-take-away-api-openapi.yml
  format: yaml
  label: Deliverart Take away API
  slug: deliverart-take-away-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-take-away-api-openapi.yml
- filename: deliverart-workshifts-api-openapi.yml
  format: yaml
  label: Deliverart Workshifts API
  slug: deliverart-workshifts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/openapi/deliverart-workshifts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deliverart.it
  spf: true
hosts:
- cert_expires: Sep 29 12:42:10 2026 GMT
  host: deliverart.it
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: pubapi.deliverart.it
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deliverart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deliverart, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deliverart
provider_slug: deliverart
slug: deliverart-domain-security
source_filename: deliverart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deliverart.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:42:10 2026 GMT\n  hsts: false\n- host: pubapi.deliverart.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: deliverart.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deliverart/refs/heads/main/security/deliverart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Delivery
- Restaurants
- Order Management
- Logistics
- Delivery
- Menu Management
- Point of Sale
---
