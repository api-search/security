---
api_specs:
- filename: 2ndkitchen-authentication-api-openapi.yml
  format: yaml
  label: 2ndKitchen Authentication API
  slug: 2ndkitchen-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-authentication-api-openapi.yml
- filename: 2ndkitchen-brand-api-openapi.yml
  format: yaml
  label: 2ndKitchen Brand API
  slug: 2ndkitchen-brand-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-brand-api-openapi.yml
- filename: 2ndkitchen-business-api-openapi.yml
  format: yaml
  label: 2ndKitchen Business API
  slug: 2ndkitchen-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-business-api-openapi.yml
- filename: 2ndkitchen-coupons-api-openapi.yml
  format: yaml
  label: 2ndKitchen Coupons API
  slug: 2ndkitchen-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-coupons-api-openapi.yml
- filename: 2ndkitchen-deliveries-api-openapi.yml
  format: yaml
  label: 2ndKitchen Deliveries API
  slug: 2ndkitchen-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-deliveries-api-openapi.yml
- filename: 2ndkitchen-orders-api-openapi.yml
  format: yaml
  label: 2ndKitchen Orders API
  slug: 2ndkitchen-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-orders-api-openapi.yml
- filename: 2ndkitchen-payment-api-openapi.yml
  format: yaml
  label: 2ndKitchen Payment API
  slug: 2ndkitchen-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-payment-api-openapi.yml
- filename: 2ndkitchen-product-api-openapi.yml
  format: yaml
  label: 2ndKitchen Product API
  slug: 2ndkitchen-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-product-api-openapi.yml
- filename: 2ndkitchen-products-api-openapi.yml
  format: yaml
  label: 2ndKitchen Products API
  slug: 2ndkitchen-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-products-api-openapi.yml
- filename: 2ndkitchen-restaurant-api-openapi.yml
  format: yaml
  label: 2ndKitchen Restaurant API
  slug: 2ndkitchen-restaurant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-restaurant-api-openapi.yml
- filename: 2ndkitchen-restaurants-api-openapi.yml
  format: yaml
  label: 2ndKitchen Restaurants API
  slug: 2ndkitchen-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-restaurants-api-openapi.yml
- filename: 2ndkitchen-users-api-openapi.yml
  format: yaml
  label: 2ndKitchen Users API
  slug: 2ndkitchen-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 2ndkitchen.com
  spf: false
hosts:
- cert_expires: Aug 26 11:57:42 2026 GMT
  host: 2ndkitchen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: docs.2ndkitchen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: auth-staging.2ndkitchen.com
  https: false
kind: domain-security
layout: security
method: probed
name: 2Ndkitchen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2ndKitchen, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: 2ndKitchen
provider_slug: 2ndkitchen
slug: 2ndkitchen-domain-security
source_filename: 2ndkitchen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 2ndkitchen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:57:42 2026 GMT\n  hsts: false\n- host: docs.2ndkitchen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: auth-staging.2ndkitchen.com\n  https: false\ndomains:\n- domain: 2ndkitchen.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/security/2ndkitchen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Technology
- Ghost Kitchen
- Restaurant
- Food Delivery
- Ordering
- Payments
- Hospitality
- Techstars
- Acquired
---
