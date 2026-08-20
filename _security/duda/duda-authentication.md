---
api_key_in: []
api_specs:
- filename: duda-accounts-api-openapi.yml
  format: yaml
  label: Duda Accounts API
  slug: duda-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-accounts-api-openapi.yml
- filename: duda-authentication-api-openapi.yml
  format: yaml
  label: Duda Authentication API
  slug: duda-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-authentication-api-openapi.yml
- filename: duda-blog-api-openapi.yml
  format: yaml
  label: Duda Blog API
  slug: duda-blog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-blog-api-openapi.yml
- filename: duda-collections-api-openapi.yml
  format: yaml
  label: Duda Collections API
  slug: duda-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-collections-api-openapi.yml
- filename: duda-ecommerce-orders-api-openapi.yml
  format: yaml
  label: Duda eCommerce - Orders API
  slug: duda-ecommerce-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-ecommerce-orders-api-openapi.yml
- filename: duda-ecommerce-products-api-openapi.yml
  format: yaml
  label: Duda eCommerce - Products API
  slug: duda-ecommerce-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-ecommerce-products-api-openapi.yml
- filename: duda-pages-api-openapi.yml
  format: yaml
  label: Duda Pages API
  slug: duda-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-pages-api-openapi.yml
- filename: duda-sites-api-openapi.yml
  format: yaml
  label: Duda Sites API
  slug: duda-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-sites-api-openapi.yml
- filename: duda-templates-api-openapi.yml
  format: yaml
  label: Duda Templates API
  slug: duda-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-templates-api-openapi.yml
- filename: duda-webhooks-api-openapi.yml
  format: yaml
  label: Duda Webhooks API
  slug: duda-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/openapi/duda-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Duda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Duda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Duda
provider_slug: duda
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using API user credentials (base64 encoded user:pass)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/duda-partner-api.json
  type: http
slug: duda-authentication
source_filename: duda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/duda-partner-api.json\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using API user credentials (base64 encoded user:pass)\n  sources:\n  - openapi/duda-partner-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duda/refs/heads/main/authentication/duda-authentication.yml
summary_line: http · 1 scheme
tags:
- Website Builder
- Agencies
- White Label
- Software-as-a-Service
- E-Commerce
- CMS
---
