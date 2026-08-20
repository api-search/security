---
api_specs:
- filename: mason-apps-api-openapi.yml
  format: yaml
  label: Mason Apps API
  slug: mason-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-apps-api-openapi.yml
- filename: mason-create-image-api-openapi.yml
  format: yaml
  label: Mason Create Image API
  slug: mason-create-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-create-image-api-openapi.yml
- filename: mason-images-api-openapi.yml
  format: yaml
  label: Mason Images API
  slug: mason-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-images-api-openapi.yml
- filename: mason-retrieve-an-image-api-openapi.yml
  format: yaml
  label: Mason Retrieve an Image API
  slug: mason-retrieve-an-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-retrieve-an-image-api-openapi.yml
- filename: mason-search-api-openapi.yml
  format: yaml
  label: Mason Search API
  slug: mason-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-search-api-openapi.yml
- filename: mason-template-mappings-api-openapi.yml
  format: yaml
  label: Mason Template Mappings API
  slug: mason-template-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-template-mappings-api-openapi.yml
- filename: mason-tiered-discounts-api-openapi.yml
  format: yaml
  label: Mason Tiered Discounts API
  slug: mason-tiered-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-tiered-discounts-api-openapi.yml
- filename: mason-webhooks-api-openapi.yml
  format: yaml
  label: Mason Webhooks API
  slug: mason-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/openapi/mason-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getmason.io
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: getmason.dev
  spf: false
hosts:
- cert_expires: Sep 25 17:32:23 2026 GMT
  host: getmason.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 20:14:14 2026 GMT
  host: www.getmason.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: api.getmason.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mason Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mason, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mason
provider_slug: mason
slug: mason-domain-security
source_filename: mason-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmason.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:32:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.getmason.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 20:14:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getmason.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: getmason.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getmason.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/security/mason-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- E-Commerce
- Commerce
- Artificial Intelligence
- Agents
- Content Generation
- Discounts
- Promotions
- Webhook
- Shopify
---
