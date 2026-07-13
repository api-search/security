---
api_key_in: []
api_specs:
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Product API
  slug: scalablepress-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Quote API
  slug: scalablepress-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Order API
  slug: scalablepress-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Event API
  slug: scalablepress-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Design API
  slug: scalablepress-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Mockup API
  slug: scalablepress-mockup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
- filename: scalablepress-openapi.yml
  format: yaml
  label: Scalable Press Billing API
  slug: scalablepress-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/openapi/scalablepress-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Scalablepress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Press secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Press
provider_slug: scalablepress
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Supply your private Scalable Press API key as the password; the username is left blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/scalablepress-openapi.yml
  type: http
slug: scalablepress-authentication
source_filename: scalablepress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalablepress-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Supply your private Scalable Press API key as the\n    password; the username is left blank.\n  sources:\n  - openapi/scalablepress-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalablepress/refs/heads/main/authentication/scalablepress-authentication.yml
summary_line: http · 1 scheme
tags:
- Print on Demand
- Fulfillment
- Apparel
- Custom Printing
- E-Commerce
- Wholesale
---
