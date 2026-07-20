---
api_key_in: []
api_specs:
- filename: curated-for-you-openapi-original.yml
  format: yaml
  label: Curated for You API
  slug: curated-for-you-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curated-for-you/refs/heads/main/openapi/curated-for-you-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Curated For You Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Curated for You secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Curated for You
provider_slug: curated-for-you
scheme_count: 1
schemes:
- bearer:
    format: Bearer <token>
    header: Authorization
  flow: password
  name: OAuth2Password
  operation: openapi/curated-for-you-openapi-original.yml#login_api_v2_users_login_post
  sources:
  - openapi/curated-for-you-openapi-original.yml
  token_endpoint: https://api.curatedforyou.io/api/v2/users/login
  token_request:
    content_type: application/x-www-form-urlencoded
    fields:
    - username
    - password
    method: POST
  token_ttl_minutes: 30
  type: oauth2
slug: curated-for-you-authentication
source_filename: curated-for-you-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.curatedforyou.io/docs\ndocs: https://api.curatedforyou.io/docs\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - password\n  note: >-\n    The published OpenAPI (3.1) declares no components.securitySchemes; the\n    authentication contract below is captured from the API Usage Guide in the\n    spec info.description and the live login operation.\nschemes:\n- name: OAuth2Password\n  type: oauth2\n  flow: password\n  token_endpoint: https://api.curatedforyou.io/api/v2/users/login\n  token_request:\n    method: POST\n    content_type: application/x-www-form-urlencoded\n    fields:\n    - username\n    - password\n  bearer:\n    header: Authorization\n    format: Bearer <token>\n  token_ttl_minutes: 30\n  operation: openapi/curated-for-you-openapi-original.yml#login_api_v2_users_login_post\n  sources:\n  - openapi/curated-for-you-openapi-original.yml\nnotes: >-\n  Permissions are provisioned per-organization\
  \ at onboarding; additional\n  permissions are requested through a customer care representative. Access\n  is scoped to the companies a user is granted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curated-for-you/refs/heads/main/authentication/curated-for-you-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Product Discovery
- Personalization
- Artificial Intelligence
- Curation
- Shopify
- Lifestyle Commerce
---
