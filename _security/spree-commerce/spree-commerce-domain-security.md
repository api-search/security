---
api_specs:
- filename: spree-commerce-store-api-openapi.yml
  format: yaml
  label: Spree Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-store-api-openapi.yml
- filename: spree-commerce-admin-api-openapi.yml
  format: yaml
  label: Spree Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-admin-api-openapi.yml
- filename: spree-commerce-platform-api-openapi.yml
  format: yaml
  label: Spree Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-platform-api-openapi.yml
- filename: spree-commerce-storefront-api-openapi.yml
  format: yaml
  label: Spree Storefront API (JSON:API)
  slug: storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-storefront-api-openapi.yml
- filename: spree-commerce-oauth-api-openapi.yml
  format: yaml
  label: Spree OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/openapi/spree-commerce-oauth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spreecommerce.org
  spf: true
hosts:
- cert_expires: Sep  2 20:24:06 2026 GMT
  host: spreecommerce.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:24:06 2026 GMT
  host: dev-docs.spreecommerce.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 06:42:20 2026 GMT
  host: demo.spreecommerce.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spree Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spree Commerce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spree Commerce
provider_slug: spree-commerce
slug: spree-commerce-domain-security
source_filename: spree-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spreecommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:24:06 2026 GMT\n  hsts: false\n- host: dev-docs.spreecommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:24:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.spreecommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:42:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: spreecommerce.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spree-commerce/refs/heads/main/security/spree-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Commerce
- Headless
- eCommerce
- Open Source
- Ruby on Rails
- Ruby
- TypeScript
---
