---
api_specs:
- filename: primis-auth-api-openapi.yml
  format: yaml
  label: PRIMIS Auth API
  slug: primis-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-auth-api-openapi.yml
- filename: primis-billing-api-openapi.yml
  format: yaml
  label: PRIMIS Billing API
  slug: primis-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-billing-api-openapi.yml
- filename: primis-campaign-api-openapi.yml
  format: yaml
  label: PRIMIS Campaign API
  slug: primis-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-campaign-api-openapi.yml
- filename: primis-document-api-openapi.yml
  format: yaml
  label: PRIMIS Document API
  slug: primis-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-document-api-openapi.yml
- filename: primis-faq-api-openapi.yml
  format: yaml
  label: PRIMIS FAQ API
  slug: primis-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-faq-api-openapi.yml
- filename: primis-index-api-openapi.yml
  format: yaml
  label: PRIMIS Index API
  slug: primis-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-index-api-openapi.yml
- filename: primis-invitation-api-openapi.yml
  format: yaml
  label: PRIMIS Invitation API
  slug: primis-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-invitation-api-openapi.yml
- filename: primis-order-api-openapi.yml
  format: yaml
  label: PRIMIS Order API
  slug: primis-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-order-api-openapi.yml
- filename: primis-product-api-openapi.yml
  format: yaml
  label: PRIMIS Product API
  slug: primis-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-product-api-openapi.yml
- filename: primis-retailer-api-openapi.yml
  format: yaml
  label: PRIMIS Retailer API
  slug: primis-retailer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-retailer-api-openapi.yml
- filename: primis-tracking-api-openapi.yml
  format: yaml
  label: PRIMIS Tracking API
  slug: primis-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-tracking-api-openapi.yml
- filename: primis-user-api-openapi.yml
  format: yaml
  label: PRIMIS User API
  slug: primis-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/openapi/primis-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: primis.cx
  spf: true
hosts:
- cert_expires: Sep  9 21:08:22 2026 GMT
  host: primis.cx
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.primis.cx
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: api.qa.primis.cx
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Primis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PRIMIS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PRIMIS
provider_slug: primis
slug: primis-domain-security
source_filename: primis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: primis.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:08:22 2026 GMT\n  hsts: false\n- host: api.primis.cx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.qa.primis.cx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: primis.cx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primis/refs/heads/main/security/primis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- Logistics
- Shipping
- Returns
- Order Tracking
- Post-Purchase
- Customer Experience
- Fulfillment
---
