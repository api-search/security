---
api_key_in:
- header
api_specs:
- filename: strapi-rest-api-openapi.yml
  format: yaml
  label: Strapi REST API
  slug: strapi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/openapi/strapi-rest-api-openapi.yml
- filename: strapi-admin-panel-api-openapi.yml
  format: yaml
  label: Strapi Admin Panel API
  slug: strapi-admin-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/openapi/strapi-admin-panel-api-openapi.yml
- filename: strapi-users-and-permissions-api-openapi.yml
  format: yaml
  label: Strapi Users and Permissions API
  slug: strapi-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/openapi/strapi-users-and-permissions-api-openapi.yml
- filename: strapi-webhooks-asyncapi.yml
  format: yaml
  label: Strapi Webhooks
  slug: strapi-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/asyncapi/strapi-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Strapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Strapi secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Strapi
provider_slug: strapi
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Admin JWT token obtained from the /admin/login endpoint. Include as Authorization: Bearer {token}.'
  name: adminBearerAuth
  scheme: bearer
  sources:
  - openapi/strapi-admin-panel-api-openapi.yml
  - openapi/strapi-rest-api-openapi.yml
  - openapi/strapi-users-and-permissions-api-openapi.yml
  type: http
- description: 'API token created in the Strapi admin panel under Settings > Global settings > API Tokens. Include as Authorization: Bearer {token}.'
  in: header
  name: apiTokenAuth
  parameter: Authorization
  sources:
  - openapi/strapi-rest-api-openapi.yml
  type: apiKey
slug: strapi-authentication
source_filename: strapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/strapi-admin-panel-api-openapi.yml, openapi/strapi-rest-api-openapi.yml, openapi/strapi-users-and-permissions-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: adminBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Admin JWT token obtained from the /admin/login endpoint. Include as Authorization:\n    Bearer {token}.'\n  sources:\n  - openapi/strapi-admin-panel-api-openapi.yml\n  - openapi/strapi-rest-api-openapi.yml\n  - openapi/strapi-users-and-permissions-api-openapi.yml\n- name: apiTokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token created in the Strapi admin panel under Settings > Global settings\n    > API Tokens. Include as Authorization: Bearer {token}.'\n  sources:\n  - openapi/strapi-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strapi/refs/heads/main/authentication/strapi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CMS
- Content Management
- Headless CMS
- Node.js
- Open Source
---
