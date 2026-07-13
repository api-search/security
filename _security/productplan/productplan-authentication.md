---
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: ProductPlan REST API
  slug: productplan-rest-api
  spec_type: OpenAPI
  url: https://productplan.readme.io/reference/overview
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Productplan Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProductPlan secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ProductPlan
provider_slug: productplan
scheme_count: 1
schemes:
- description: 'Personal Access Token (64-character hash). Generate in ProductPlan under Settings > Integrations. Include as: Authorization: Bearer <token>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/productplan-rest-api-openapi.yml
  type: http
slug: productplan-authentication
source_filename: productplan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/productplan-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Personal Access Token (64-character hash). Generate in ProductPlan under Settings\n    > Integrations. Include as: Authorization: Bearer <token>'\n  sources:\n  - openapi/productplan-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/productplan/refs/heads/main/authentication/productplan-authentication.yml
summary_line: http · 1 scheme
tags:
- Road Mapping
- Product Management
- OKR
- Roadmaps
- Features
- Product Strategy
- Launches
- Discovery
- Integrations
---
