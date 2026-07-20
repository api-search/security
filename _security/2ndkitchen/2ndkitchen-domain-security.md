---
api_specs:
- filename: 2ndkitchen-authservice.yaml
  format: yaml
  label: 2ndKitchen Authentication Service
  slug: 2ndkitchen-authentication-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-authservice.yaml
- filename: 2ndkitchen-businessservice.yaml
  format: yaml
  label: 2ndKitchen Business Service
  slug: 2ndkitchen-business-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-businessservice.yaml
- filename: 2ndkitchen-userservice.yaml
  format: yaml
  label: 2ndKitchen User Service
  slug: 2ndkitchen-user-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-userservice.yaml
- filename: 2ndkitchen-restaurantservice.yaml
  format: yaml
  label: 2ndKitchen Restaurant Service
  slug: 2ndkitchen-restaurant-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-restaurantservice.yaml
- filename: 2ndkitchen-orderservice.yaml
  format: yaml
  label: 2ndKitchen Order Service
  slug: 2ndkitchen-order-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-orderservice.yaml
- filename: 2ndkitchen-pricingservice.yaml
  format: yaml
  label: 2ndKitchen Pricing Service
  slug: 2ndkitchen-pricing-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-pricingservice.yaml
- filename: 2ndkitchen-paymentservice.yaml
  format: yaml
  label: 2ndKitchen Payment Service
  slug: 2ndkitchen-payment-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-paymentservice.yaml
- filename: 2ndkitchen-deliveryservice.yaml
  format: yaml
  label: 2ndKitchen Delivery Service
  slug: 2ndkitchen-delivery-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-deliveryservice.yaml
- filename: 2ndkitchen-indexingservice.yaml
  format: yaml
  label: 2ndKitchen Indexing Service
  slug: 2ndkitchen-indexing-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2ndkitchen/refs/heads/main/openapi/2ndkitchen-indexingservice.yaml
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
