---
api_key_in:
- header
api_specs:
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Customers API
  slug: smartmoving-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Opportunities API
  slug: smartmoving-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Leads API
  slug: smartmoving-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Lead Provider API
  slug: smartmoving-lead-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Jobs & Moves API
  slug: smartmoving-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Reference Data API
  slug: smartmoving-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
- filename: smartmoving-openapi.yml
  format: yaml
  label: SmartMoving Webhooks API
  slug: smartmoving-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/openapi/smartmoving-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smartmoving Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmartMoving secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SmartMoving
provider_slug: smartmoving
scheme_count: 1
schemes:
- description: Open API key issued at Settings > Integrations > SmartMoving API. The Azure API Management gateway may additionally require an Ocp-Apim-Subscription-Key header.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/smartmoving-openapi.yml
  type: apiKey
slug: smartmoving-authentication
source_filename: smartmoving-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smartmoving-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Open API key issued at Settings > Integrations > SmartMoving API. The Azure API\n    Management gateway may additionally require an Ocp-Apim-Subscription-Key header.\n  sources:\n  - openapi/smartmoving-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartmoving/refs/heads/main/authentication/smartmoving-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Moving Software
- CRM
- Field Service
- Moving Company
- Operations
- Lead Management
- Dispatch
---
