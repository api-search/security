---
api_specs:
- filename: goody-brands-api-openapi.yml
  format: yaml
  label: Goody Brands API
  slug: goody-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-brands-api-openapi.yml
- filename: goody-cards-api-openapi.yml
  format: yaml
  label: Goody Cards API
  slug: goody-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-cards-api-openapi.yml
- filename: goody-collections-api-openapi.yml
  format: yaml
  label: Goody Collections API
  slug: goody-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-collections-api-openapi.yml
- filename: goody-commerce-user-payment-methods-api-openapi.yml
  format: yaml
  label: Goody Commerce User Payment Methods API
  slug: goody-commerce-user-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-commerce-user-payment-methods-api-openapi.yml
- filename: goody-me-api-openapi.yml
  format: yaml
  label: Goody Me API
  slug: goody-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-me-api-openapi.yml
- filename: goody-order-activities-api-openapi.yml
  format: yaml
  label: Goody Order Activities API
  slug: goody-order-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-order-activities-api-openapi.yml
- filename: goody-order-batches-api-openapi.yml
  format: yaml
  label: Goody Order Batches API
  slug: goody-order-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-order-batches-api-openapi.yml
- filename: goody-orders-api-openapi.yml
  format: yaml
  label: Goody Orders API
  slug: goody-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-orders-api-openapi.yml
- filename: goody-payment-methods-api-openapi.yml
  format: yaml
  label: Goody Payment Methods API
  slug: goody-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-payment-methods-api-openapi.yml
- filename: goody-products-api-openapi.yml
  format: yaml
  label: Goody Products API
  slug: goody-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-products-api-openapi.yml
- filename: goody-webhooks-api-openapi.yml
  format: yaml
  label: Goody Webhooks API
  slug: goody-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-webhooks-api-openapi.yml
- filename: goody-workspaces-api-openapi.yml
  format: yaml
  label: Goody Workspaces API
  slug: goody-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/openapi/goody-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ongoody.com
  spf: true
hosts:
- cert_expires: Oct  9 03:52:46 2026 GMT
  host: www.ongoody.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goody Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goody, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goody
provider_slug: goody
slug: goody-domain-security
source_filename: goody-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ongoody.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:52:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: ongoody.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goody/refs/heads/main/security/goody-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Gifting
- Gift Cards
- E-Commerce
- Commerce
- Payments
- MCP
- Webhook
- Rewards
---
