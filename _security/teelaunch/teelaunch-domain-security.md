---
api_specs:
- filename: teelaunch-account-api-openapi.yml
  format: yaml
  label: Teelaunch Account API
  slug: teelaunch-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-account-api-openapi.yml
- filename: teelaunch-account-payment-api-openapi.yml
  format: yaml
  label: Teelaunch Account Payment API
  slug: teelaunch-account-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-account-payment-api-openapi.yml
- filename: teelaunch-account-settings-api-openapi.yml
  format: yaml
  label: Teelaunch Account Settings API
  slug: teelaunch-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-account-settings-api-openapi.yml
- filename: teelaunch-blank-api-openapi.yml
  format: yaml
  label: Teelaunch Blank API
  slug: teelaunch-blank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-blank-api-openapi.yml
- filename: teelaunch-blank-category-api-openapi.yml
  format: yaml
  label: Teelaunch Blank Category API
  slug: teelaunch-blank-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-blank-category-api-openapi.yml
- filename: teelaunch-orders-api-openapi.yml
  format: yaml
  label: Teelaunch Orders API
  slug: teelaunch-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-orders-api-openapi.yml
- filename: teelaunch-platform-store-product-variants-api-openapi.yml
  format: yaml
  label: Teelaunch Platform Store Product Variants API
  slug: teelaunch-platform-store-product-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platform-store-product-variants-api-openapi.yml
- filename: teelaunch-platform-store-products-api-openapi.yml
  format: yaml
  label: Teelaunch Platform Store Products API
  slug: teelaunch-platform-store-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platform-store-products-api-openapi.yml
- filename: teelaunch-platform-stores-api-openapi.yml
  format: yaml
  label: Teelaunch Platform Stores API
  slug: teelaunch-platform-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platform-stores-api-openapi.yml
- filename: teelaunch-platforms-api-openapi.yml
  format: yaml
  label: Teelaunch Platforms API
  slug: teelaunch-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-platforms-api-openapi.yml
- filename: teelaunch-products-api-openapi.yml
  format: yaml
  label: Teelaunch Products API
  slug: teelaunch-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/openapi/teelaunch-products-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: teelaunch.com
  spf: true
hosts:
- cert_expires: Sep 19 08:07:53 2026 GMT
  host: teelaunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 08:07:53 2026 GMT
  host: api.teelaunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teelaunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teelaunch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teelaunch
provider_slug: teelaunch
slug: teelaunch-domain-security
source_filename: teelaunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teelaunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:07:53 2026 GMT\n  hsts: false\n- host: api.teelaunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:07:53 2026 GMT\n  hsts: false\ndomains:\n- domain: teelaunch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teelaunch/refs/heads/main/security/teelaunch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Print on Demand
- POD
- Ecommerce
- Fulfillment
- Dropshipping
- Orders
- Shipping
---
