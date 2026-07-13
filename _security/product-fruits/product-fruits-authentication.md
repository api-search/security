---
api_key_in: []
api_specs:
- filename: rest-api-authentication
  format: yaml
  label: Product Fruits REST API
  slug: product-fruits-rest-api
  spec_type: OpenAPI
  url: https://help.productfruits.com/en/article/rest-api-authentication
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Product Fruits Authentication
name_suffix: Authentication
oauth_flows: []
overview: Product Fruits secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Product Fruits
provider_slug: product-fruits
scheme_count: 1
schemes:
- description: API key generated from the Integrations section in Product Fruits. Should never be exposed in front-end environments.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: product-fruits-authentication
source_filename: product-fruits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key generated from the Integrations section in Product Fruits. Should never\n    be exposed in front-end environments.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/product-fruits/refs/heads/main/authentication/product-fruits-authentication.yml
summary_line: http · 1 scheme
tags:
- Product Adoption
- User Onboarding
- In-App Guidance
- Checklists
- NPS Surveys
- Announcements
- User Segmentation
- SaaS
---
