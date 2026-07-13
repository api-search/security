---
api_specs:
- filename: shopify-storefront-openapi.yml
  format: yaml
  label: Shopify Storefront API
  slug: shopify-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify-storefront/refs/heads/main/openapi/shopify-storefront-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
hosts:
- cert_expires: Aug 12 05:59:10 2026 GMT
  host: shopify.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopify Storefront Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopify Storefront API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Shopify Storefront API
provider_slug: shopify-storefront
slug: shopify-storefront-domain-security
source_filename: shopify-storefront-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 05:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopify-storefront/refs/heads/main/security/shopify-storefront-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Ecommerce
- Headless
- GraphQL
- Storefront
- Products
- Cart
- Checkout
---
