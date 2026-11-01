---
api_specs:
- filename: bold-commerce-customers-api-openapi.yml
  format: yaml
  label: Bold Commerce Customers API
  slug: bold-commerce-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-customers-api-openapi.yml
- filename: bold-commerce-shops-api-openapi.yml
  format: yaml
  label: Bold Commerce Shops API
  slug: bold-commerce-shops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-shops-api-openapi.yml
- filename: bold-commerce-subscriptions-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscriptions API
  slug: bold-commerce-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscriptions-api-openapi.yml
- filename: bold-commerce-convertible-adjustments-api-openapi.yml
  format: yaml
  label: Bold Commerce Convertible Adjustments API
  slug: bold-commerce-convertible-adjustments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-convertible-adjustments-api-openapi.yml
- filename: bold-commerce-future-orders-api-openapi.yml
  format: yaml
  label: Bold Commerce Future Orders API
  slug: bold-commerce-future-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-future-orders-api-openapi.yml
- filename: bold-commerce-payment-methods-api-openapi.yml
  format: yaml
  label: Bold Commerce Payment Methods API
  slug: bold-commerce-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-payment-methods-api-openapi.yml
- filename: bold-commerce-subscription-adjustments-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Adjustments API
  slug: bold-commerce-subscription-adjustments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-adjustments-api-openapi.yml
- filename: bold-commerce-subscription-groups-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Groups API
  slug: bold-commerce-subscription-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-groups-api-openapi.yml
- filename: bold-commerce-subscription-line-items-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Line Items API
  slug: bold-commerce-subscription-line-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-line-items-api-openapi.yml
- filename: bold-commerce-subscription-orders-api-openapi.yml
  format: yaml
  label: Bold Commerce Subscription Orders API
  slug: bold-commerce-subscription-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-subscription-orders-api-openapi.yml
- filename: bold-commerce-webhook-events-api-openapi.yml
  format: yaml
  label: Bold Commerce Webhook Events API
  slug: bold-commerce-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-webhook-events-api-openapi.yml
- filename: bold-commerce-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Bold Commerce Webhook Subscriptions API
  slug: bold-commerce-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-webhook-subscriptions-api-openapi.yml
- filename: bold-commerce-webhook-topics-api-openapi.yml
  format: yaml
  label: Bold Commerce Webhook Topics API
  slug: bold-commerce-webhook-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bold-commerce/openapi/bold-commerce-webhook-topics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: boldcommerce.com
  spf: true
hosts:
- cert_expires: Sep 20 03:20:30 2026 GMT
  host: boldcommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:07:15 2026 GMT
  host: developer.boldcommerce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:00:41 2026 GMT
  host: api.boldcommerce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bold Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bold Commerce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bold Commerce
provider_slug: bold-commerce
slug: bold-commerce-domain-security
source_filename: bold-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boldcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 03:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.boldcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:07:15 2026 GMT\n  hsts: false\n- host: api.boldcommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:00:41 2026 GMT\n  hsts: false\ndomains:\n- domain: boldcommerce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bold-commerce/security/bold-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- E-Commerce
- Subscription
- Checkout
- Pricing
- Headless Commerce
- Shopify
---
