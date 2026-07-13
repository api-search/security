---
api_specs:
- filename: shopify-api-openapi.yml
  format: yaml
  label: Shopify Admin REST API
  slug: shopify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-api-openapi.yml
- filename: shopify-ajax-api-openapi.yml
  format: yaml
  label: Shopify Ajax API
  slug: ajax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-ajax-api-openapi.yml
- filename: shopify-webhooks-api-openapi.yml
  format: yaml
  label: Shopify Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-webhooks-api-openapi.yml
- filename: shopify-multipass-api-openapi.yml
  format: yaml
  label: Shopify Multipass API
  slug: multipass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/openapi/shopify-multipass-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shopify.com
  spf: true
hosts:
- cert_expires: Aug 12 05:59:10 2026 GMT
  host: shopify.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 19:08:28 2026 GMT
  host: www.shopify.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shopify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shopify, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Shopify
provider_slug: shopify
slug: shopify-domain-security
source_filename: shopify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shopify.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 05:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.shopify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 19:08:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: shopify.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: shopify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shopify/refs/heads/main/security/shopify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Ecommerce
- Payments
- Retail
- Shopping Cart
- T1
---
