---
api_key_in: []
api_specs:
- filename: havenly-addresses-api-openapi.yml
  format: yaml
  label: Havenly Addresses API
  slug: havenly-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-addresses-api-openapi.yml
- filename: havenly-attribute-types-api-openapi.yml
  format: yaml
  label: Havenly Attribute Types API
  slug: havenly-attribute-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-attribute-types-api-openapi.yml
- filename: havenly-authentication-api-openapi.yml
  format: yaml
  label: Havenly Authentication API
  slug: havenly-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-authentication-api-openapi.yml
- filename: havenly-board-feedback-api-openapi.yml
  format: yaml
  label: Havenly Board Feedback API
  slug: havenly-board-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-board-feedback-api-openapi.yml
- filename: havenly-board-feedback-questions-api-openapi.yml
  format: yaml
  label: Havenly Board Feedback Questions API
  slug: havenly-board-feedback-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-board-feedback-questions-api-openapi.yml
- filename: havenly-board-products-api-openapi.yml
  format: yaml
  label: Havenly Board Products API
  slug: havenly-board-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-board-products-api-openapi.yml
- filename: havenly-searched-vendor-variants-api-openapi.yml
  format: yaml
  label: Havenly Searched Vendor Variants API
  slug: havenly-searched-vendor-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-searched-vendor-variants-api-openapi.yml
- filename: havenly-user-opinions-api-openapi.yml
  format: yaml
  label: Havenly User Opinions API
  slug: havenly-user-opinions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-user-opinions-api-openapi.yml
- filename: havenly-user-profile-api-openapi.yml
  format: yaml
  label: Havenly User Profile API
  slug: havenly-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-user-profile-api-openapi.yml
- filename: havenly-users-api-openapi.yml
  format: yaml
  label: Havenly Users API
  slug: havenly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-users-api-openapi.yml
- filename: havenly-vendor-variants-api-openapi.yml
  format: yaml
  label: Havenly Vendor Variants API
  slug: havenly-vendor-variants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/openapi/havenly-vendor-variants-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Havenly Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Havenly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Havenly
provider_slug: havenly
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'OAuth2 access token from POST /oauth (password grant), sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/havenly-openapi.yml
  type: http
- flows:
  - flow: password
    scopes: 0
    tokenUrl: https://api.havenly.com/oauth
  name: oauth2
  sources:
  - openapi/havenly-openapi.yml
  type: oauth2
slug: havenly-authentication
source_filename: havenly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/havenly-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'OAuth2 access token from POST /oauth (password grant), sent as Authorization:\n    Bearer <token>.'\n  sources:\n  - openapi/havenly-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.havenly.com/oauth\n    scopes: 0\n  sources:\n  - openapi/havenly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/havenly/refs/heads/main/authentication/havenly-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Interior Design
- Home Decor
- Furniture
- E-Commerce
- Marketplace
- Design
- Retail
- Artificial Intelligence
---
