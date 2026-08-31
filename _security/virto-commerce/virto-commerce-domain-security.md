---
api_specs:
- filename: virto-commerce-catalog-api-openapi.yml
  format: yaml
  label: Virto Commerce Catalog API
  slug: virto-commerce-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-catalog-api-openapi.yml
- filename: virto-commerce-companies-and-contacts-api-openapi.yml
  format: yaml
  label: Virto Commerce Companies and Contacts API
  slug: virto-commerce-companies-and-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-companies-and-contacts-api-openapi.yml
- filename: virto-commerce-inventory-api-openapi.yml
  format: yaml
  label: Virto Commerce Inventory API
  slug: virto-commerce-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-inventory-api-openapi.yml
- filename: virto-commerce-marketing-api-openapi.yml
  format: yaml
  label: Virto Commerce Marketing API
  slug: virto-commerce-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-marketing-api-openapi.yml
- filename: virto-commerce-order-management-api-openapi.yml
  format: yaml
  label: Virto Commerce Order Management API
  slug: virto-commerce-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-order-management-api-openapi.yml
- filename: virto-commerce-pricing-api-openapi.yml
  format: yaml
  label: Virto Commerce Pricing API
  slug: virto-commerce-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-pricing-api-openapi.yml
- filename: virto-commerce-quotes-api-openapi.yml
  format: yaml
  label: Virto Commerce Quotes API
  slug: virto-commerce-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-quotes-api-openapi.yml
- filename: virto-commerce-shopping-cart-api-openapi.yml
  format: yaml
  label: Virto Commerce Shopping Cart API
  slug: virto-commerce-shopping-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-shopping-cart-api-openapi.yml
- filename: virto-commerce-store-api-openapi.yml
  format: yaml
  label: Virto Commerce Store API
  slug: virto-commerce-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-store-api-openapi.yml
- filename: virto-commerce-virtocommerce-platform-api-openapi.yml
  format: yaml
  label: Virto Commerce VirtoCommerce Platform API
  slug: virto-commerce-virtocommerce-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
- filename: virto-commerce-webhooks-api-openapi.yml
  format: yaml
  label: Virto Commerce Webhooks API
  slug: virto-commerce-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-webhooks-api-openapi.yml
- filename: virto-commerce-returns-api-openapi.yml
  format: yaml
  label: Virto Commerce Returns API
  slug: virto-commerce-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-returns-api-openapi.yml
- filename: virto-commerce-event-bus-module-api-openapi.yml
  format: yaml
  label: Virto Commerce Event Bus module API
  slug: virto-commerce-event-bus-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-event-bus-module-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: virtocommerce.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: virtocommerce.org
  spf: false
hosts:
- cert_expires: Sep 28 20:33:33 2026 GMT
  host: virtocommerce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 21:56:21 2026 GMT
  host: docs.virtocommerce.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 04:44:45 2026 GMT
  host: virtostart-demo-admin.govirto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virto Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virto Commerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Virto Commerce
provider_slug: virto-commerce
slug: virto-commerce-domain-security
source_filename: virto-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virtocommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:33:33 2026 GMT\n  hsts: null\n- host: docs.virtocommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:56:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: virtostart-demo-admin.govirto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 04:44:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virtocommerce.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: virtocommerce.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/security/virto-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B E-Commerce
- Catalog Management
- Order Management
- Pricing
- Inventory
- Shopping Cart
- Customer Management
- Marketing
- Payments
- Shipping
- Subscription
- Headless Commerce
- Open-Source
- .NET
- Webhook
- Event-Driven
- CloudEvents
- GraphQL
- Returns
- MCP
- B2B Quotes
---
