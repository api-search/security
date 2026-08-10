---
api_specs:
- filename: tapcart-development-api-block-templates-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Block Templates API
  slug: tapcart-development-api-block-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-block-templates-api-openapi.yml
- filename: tapcart-development-api-blocks-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Blocks API
  slug: tapcart-development-api-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-blocks-api-openapi.yml
- filename: tapcart-development-api-components-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Components API
  slug: tapcart-development-api-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-components-api-openapi.yml
- filename: tapcart-development-api-dependencies-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Dependencies API
  slug: tapcart-development-api-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-dependencies-api-openapi.yml
- filename: tapcart-development-api-layouts-api-openapi.yml
  format: yaml
  label: Tapcart Development API - Layouts API
  slug: tapcart-development-api-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/openapi/tapcart-development-api-layouts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tapcart.com
  spf: true
hosts:
- cert_expires: Oct  2 15:27:10 2026 GMT
  host: www.tapcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 16:03:18 2026 GMT
  host: dev.tapcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 07:37:06 2026 GMT
  host: api.tapcart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tapcart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tapcart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tapcart
provider_slug: tapcart
slug: tapcart-domain-security
source_filename: tapcart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tapcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:27:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.tapcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 16:03:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tapcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:37:06 2026 GMT\n  hsts: null\ndomains:\n- domain: tapcart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapcart/refs/heads/main/security/tapcart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Commerce
- Shopify
- Ecommerce
- Mobile Apps
- Push Notifications
- Analytics
- Webhooks
- Developer Tools
---
