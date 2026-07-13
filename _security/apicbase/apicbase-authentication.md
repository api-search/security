---
api_key_in: []
api_specs:
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Ingredients API
  slug: ingredients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Recipes API
  slug: recipes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Products API
  slug: products
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Inventory & Stock API
  slug: inventory-stock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Purchase Orders API
  slug: purchase-orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Suppliers API
  slug: suppliers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Outlets API
  slug: outlets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
- filename: apicbase-openapi.yml
  format: yaml
  label: Apicbase Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/openapi/apicbase-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Apicbase Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Apicbase secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Apicbase
provider_slug: apicbase
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow. Access tokens are bearer tokens valid for 7 days; refresh tokens obtain new access tokens. Include the token in the Authorization header as "Bearer ACCESS_TOKEN".
  flows:
  - authorizationUrl: https://app.apicbase.com/oauth/authorize/
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.apicbase.com/oauth/token/
  name: oauth2
  sources:
  - openapi/apicbase-openapi.yml
  type: oauth2
slug: apicbase-authentication
source_filename: apicbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicbase-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.apicbase.com/oauth/authorize/\n    tokenUrl: https://api.apicbase.com/oauth/token/\n    scopes: 2\n  description: OAuth 2.0 authorization code flow. Access tokens are bearer tokens valid for\n    7 days; refresh tokens obtain new access tokens. Include the token in the Authorization\n    header as \"Bearer ACCESS_TOKEN\".\n  sources:\n  - openapi/apicbase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicbase/refs/heads/main/authentication/apicbase-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Food and Beverage
- Restaurant
- Back of House
- Inventory
- Procurement
- Recipes
---
