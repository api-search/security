---
api_key_in:
- header
api_specs:
- filename: amazon-resource-explorer-index-api-openapi.yml
  format: yaml
  label: Amazon Resource Explorer Index API
  slug: amazon-resource-explorer-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/openapi/amazon-resource-explorer-index-api-openapi.yml
- filename: amazon-resource-explorer-resources-api-openapi.yml
  format: yaml
  label: Amazon Resource Explorer Resources API
  slug: amazon-resource-explorer-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/openapi/amazon-resource-explorer-resources-api-openapi.yml
- filename: amazon-resource-explorer-search-api-openapi.yml
  format: yaml
  label: Amazon Resource Explorer Search API
  slug: amazon-resource-explorer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/openapi/amazon-resource-explorer-search-api-openapi.yml
- filename: amazon-resource-explorer-tags-api-openapi.yml
  format: yaml
  label: Amazon Resource Explorer Tags API
  slug: amazon-resource-explorer-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/openapi/amazon-resource-explorer-tags-api-openapi.yml
- filename: amazon-resource-explorer-views-api-openapi.yml
  format: yaml
  label: Amazon Resource Explorer Views API
  slug: amazon-resource-explorer-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/openapi/amazon-resource-explorer-views-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Resource Explorer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Resource Explorer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Resource Explorer
provider_slug: amazon-resource-explorer
scheme_count: 1
schemes:
- description: AWS Signature Version 4
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-resource-explorer-openapi.yml
  type: apiKey
slug: amazon-resource-explorer-authentication
source_filename: amazon-resource-explorer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-resource-explorer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4\n  sources:\n  - openapi/amazon-resource-explorer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-resource-explorer/refs/heads/main/authentication/amazon-resource-explorer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Discovery
- Inventory
- Resource Management
---
