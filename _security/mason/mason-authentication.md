---
api_key_in: []
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
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mason Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Mason secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Mason
provider_slug: mason
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 0
    tokenUrl: token
  name: OAuth2PasswordBearer
  sources:
  - openapi/mason-apps-openapi.json
  - openapi/mason-generation-openapi.json
  - openapi/mason-search-openapi.json
  - openapi/mason-webhooks-openapi.json
  type: oauth2
slug: mason-authentication
source_filename: mason-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mason-apps-openapi.json, openapi/mason-generation-openapi.json, openapi/mason-search-openapi.json,\n  openapi/mason-webhooks-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2PasswordBearer\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: token\n    scopes: 0\n  sources:\n  - openapi/mason-apps-openapi.json\n  - openapi/mason-generation-openapi.json\n  - openapi/mason-search-openapi.json\n  - openapi/mason-webhooks-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mason/refs/heads/main/authentication/mason-authentication.yml
summary_line: oauth2 · 1 scheme
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
