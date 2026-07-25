---
api_specs:
- filename: tiendanube-categories-api-openapi.yml
  format: yaml
  label: Tiendanube Categories API
  slug: tiendanube-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-categories-api-openapi.yml
- filename: tiendanube-coupons-api-openapi.yml
  format: yaml
  label: Tiendanube Coupons API
  slug: tiendanube-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-coupons-api-openapi.yml
- filename: tiendanube-customers-api-openapi.yml
  format: yaml
  label: Tiendanube Customers API
  slug: tiendanube-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-customers-api-openapi.yml
- filename: tiendanube-fulfillment-orders-api-openapi.yml
  format: yaml
  label: Tiendanube Fulfillment Orders API
  slug: tiendanube-fulfillment-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-fulfillment-orders-api-openapi.yml
- filename: tiendanube-orders-api-openapi.yml
  format: yaml
  label: Tiendanube Orders API
  slug: tiendanube-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-orders-api-openapi.yml
- filename: tiendanube-payment-providers-api-openapi.yml
  format: yaml
  label: Tiendanube Payment Providers API
  slug: tiendanube-payment-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-payment-providers-api-openapi.yml
- filename: tiendanube-product-images-api-openapi.yml
  format: yaml
  label: Tiendanube Product Images API
  slug: tiendanube-product-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-product-images-api-openapi.yml
- filename: tiendanube-product-variants-api-openapi.yml
  format: yaml
  label: Tiendanube Product Variants API
  slug: tiendanube-product-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-product-variants-api-openapi.yml
- filename: tiendanube-products-api-openapi.yml
  format: yaml
  label: Tiendanube Products API
  slug: tiendanube-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-products-api-openapi.yml
- filename: tiendanube-scripts-api-openapi.yml
  format: yaml
  label: Tiendanube Scripts API
  slug: tiendanube-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-scripts-api-openapi.yml
- filename: tiendanube-shipping-carriers-api-openapi.yml
  format: yaml
  label: Tiendanube Shipping Carriers API
  slug: tiendanube-shipping-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-shipping-carriers-api-openapi.yml
- filename: tiendanube-webhooks-api-openapi.yml
  format: yaml
  label: Tiendanube Webhooks API
  slug: tiendanube-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/openapi/tiendanube-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tiendanube.com
  spf: true
hosts:
- cert_expires: Aug 22 06:31:23 2026 GMT
  host: www.tiendanube.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiendanube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tiendanube, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tiendanube
provider_slug: tiendanube
slug: tiendanube-domain-security
source_filename: tiendanube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tiendanube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:31:23 2026 GMT\n  hsts: false\ndomains:\n- domain: tiendanube.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiendanube/refs/heads/main/security/tiendanube-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-commerce
- Retail
- Latin America
- Storefront
- Products
- Orders
---
