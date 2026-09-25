---
api_specs:
- filename: canal-csv-api-openapi.yml
  format: yaml
  label: Canal CSV API
  slug: canal-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-csv-api-openapi.yml
- filename: canal-fulfillments-api-openapi.yml
  format: yaml
  label: Canal Fulfillments API
  slug: canal-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-fulfillments-api-openapi.yml
- filename: canal-markets-api-openapi.yml
  format: yaml
  label: Canal Markets API
  slug: canal-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-markets-api-openapi.yml
- filename: canal-max-shipping-rates-api-openapi.yml
  format: yaml
  label: Canal Max Shipping Rates API
  slug: canal-max-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-max-shipping-rates-api-openapi.yml
- filename: canal-orders-api-openapi.yml
  format: yaml
  label: Canal Orders API
  slug: canal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-orders-api-openapi.yml
- filename: canal-product-sets-api-openapi.yml
  format: yaml
  label: Canal Product Sets API
  slug: canal-product-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-product-sets-api-openapi.yml
- filename: canal-products-api-openapi.yml
  format: yaml
  label: Canal Products API
  slug: canal-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-products-api-openapi.yml
- filename: canal-refunds-api-openapi.yml
  format: yaml
  label: Canal Refunds API
  slug: canal-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-refunds-api-openapi.yml
- filename: canal-returns-api-openapi.yml
  format: yaml
  label: Canal Returns API
  slug: canal-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-returns-api-openapi.yml
- filename: canal-selection-api-openapi.yml
  format: yaml
  label: Canal Selection API
  slug: canal-selection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-selection-api-openapi.yml
- filename: canal-shipping-api-openapi.yml
  format: yaml
  label: Canal Shipping API
  slug: canal-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-shipping-api-openapi.yml
- filename: canal-shipping-rates-api-openapi.yml
  format: yaml
  label: Canal Shipping Rates API
  slug: canal-shipping-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-shipping-rates-api-openapi.yml
- filename: canal-shops-api-openapi.yml
  format: yaml
  label: Canal Shops API
  slug: canal-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-shops-api-openapi.yml
- filename: canal-tax-and-shipping-api-openapi.yml
  format: yaml
  label: Canal Tax And Shipping API
  slug: canal-tax-and-shipping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-tax-and-shipping-api-openapi.yml
- filename: canal-tax-api-openapi.yml
  format: yaml
  label: Canal Tax API
  slug: canal-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-tax-api-openapi.yml
- filename: canal-variants-api-openapi.yml
  format: yaml
  label: Canal Variants API
  slug: canal-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-variants-api-openapi.yml
- filename: canal-webhooks-api-openapi.yml
  format: yaml
  label: Canal Webhooks API
  slug: canal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/openapi/canal-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shopcanal.com
  spf: true
hosts:
- cert_expires: Aug 23 02:46:25 2026 GMT
  host: api.shopcanal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Canal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Canal
provider_slug: canal
slug: canal-domain-security
source_filename: canal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.shopcanal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 02:46:25 2026 GMT\n  hsts: false\ndomains:\n- domain: shopcanal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canal/refs/heads/main/security/canal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Dropshipping
- Marketplace
- Commerce
- Retail
- Fulfillment
- Order
- Product
- Webhook
---
