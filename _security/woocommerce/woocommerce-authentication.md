---
api_key_in: []
api_specs:
- filename: woocommerce-rest-api-openapi.yml
  format: yaml
  label: WooCommerce REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/openapi/woocommerce-rest-api-openapi.yml
- filename: woocommerce-store-api-openapi.yml
  format: yaml
  label: WooCommerce Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/openapi/woocommerce-store-api-openapi.yml
- filename: woocommerce-webhooks-asyncapi.yml
  format: yaml
  label: WooCommerce Webhook Events
  slug: webhook-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/asyncapi/woocommerce-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Woocommerce Authentication
name_suffix: Authentication
oauth_flows: []
overview: WooCommerce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WooCommerce
provider_slug: woocommerce
scheme_count: 1
schemes:
- description: HTTP Basic Auth using the WooCommerce Consumer Key as the username and Consumer Secret as the password over HTTPS. Over plain HTTP use OAuth 1.0a one-legged authentication instead.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/woocommerce-rest-api-openapi.yml
  type: http
slug: woocommerce-authentication
source_filename: woocommerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/woocommerce-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using the WooCommerce Consumer Key as the username and Consumer\n    Secret as the password over HTTPS. Over plain HTTP use OAuth 1.0a one-legged authentication\n    instead.\n  sources:\n  - openapi/woocommerce-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/authentication/woocommerce-authentication.yml
summary_line: http · 1 scheme
tags:
- eCommerce
- Open Source
- Orders
- Products
- WordPress
---
