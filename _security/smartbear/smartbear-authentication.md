---
api_key_in:
- header
api_specs:
- filename: smartbear-apis-api-openapi.yml
  format: yaml
  label: SmartBear APIs API
  slug: smartbear-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-apis-api-openapi.yml
- filename: smartbear-domains-api-openapi.yml
  format: yaml
  label: SmartBear Domains API
  slug: smartbear-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-domains-api-openapi.yml
- filename: smartbear-integrations-api-openapi.yml
  format: yaml
  label: SmartBear Integrations API
  slug: smartbear-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-integrations-api-openapi.yml
- filename: smartbear-organizations-api-openapi.yml
  format: yaml
  label: SmartBear Organizations API
  slug: smartbear-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-organizations-api-openapi.yml
- filename: smartbear-projects-api-openapi.yml
  format: yaml
  label: SmartBear Projects API
  slug: smartbear-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/openapi/smartbear-projects-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smartbear Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmartBear secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SmartBear
provider_slug: smartbear
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/smartbear-swaggerhub-openapi.yml
  type: apiKey
slug: smartbear-authentication
source_filename: smartbear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartbear-swaggerhub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/smartbear-swaggerhub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartbear/refs/heads/main/authentication/smartbear-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Design
- API Documentation
- API Testing
- Contract Testing
- Governance
- Monitoring
- Platform
---
