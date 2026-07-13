---
api_key_in:
- query
api_specs:
- filename: storyblok-content-delivery-api-v2-openapi.yml
  format: yaml
  label: Storyblok Content Delivery API
  slug: storyblok-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-content-delivery-api-v2-openapi.yml
- filename: storyblok-management-api-openapi.yml
  format: yaml
  label: Storyblok Management API
  slug: storyblok-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-management-api-openapi.yml
- filename: storyblok-image-service-openapi.yml
  format: yaml
  label: Storyblok Image Service
  slug: storyblok-image-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-image-service-openapi.yml
- filename: storyblok-webhooks-asyncapi.yml
  format: yaml
  label: Storyblok Webhooks
  slug: storyblok-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/asyncapi/storyblok-webhooks-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Storyblok Authentication
name_suffix: Authentication
oauth_flows: []
overview: Storyblok secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Storyblok
provider_slug: storyblok
scheme_count: 2
schemes:
- description: Public API token for accessing published content, or Preview API token for accessing draft and published content. Tokens are scoped to a specific Storyblok space.
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/storyblok-content-delivery-api-v2-openapi.yml
  type: apiKey
- description: Personal access token generated in the Storyblok account settings. Provides access to all spaces the account has permissions for.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/storyblok-management-api-openapi.yml
  type: http
slug: storyblok-authentication
source_filename: storyblok-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/storyblok-content-delivery-api-v2-openapi.yml, openapi/storyblok-management-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Public API token for accessing published content, or Preview API token for accessing\n    draft and published content. Tokens are scoped to a specific Storyblok space.\n  sources:\n  - openapi/storyblok-content-delivery-api-v2-openapi.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: Personal access token generated in the Storyblok account settings. Provides access\n    to all spaces the account has permissions for.\n  sources:\n  - openapi/storyblok-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/authentication/storyblok-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- CMS
- Content Delivery
- Content Management
- Headless CMS
- Image Optimization
- REST API
- Visual Editor
- Webhooks
---
