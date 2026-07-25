---
api_key_in:
- header
api_specs:
- filename: holded-accounting-api-openapi.yml
  format: yaml
  label: Holded Accounting API
  slug: holded-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-accounting-api-openapi.yml
- filename: holded-crm-api-openapi.yml
  format: yaml
  label: Holded Crm API
  slug: holded-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-crm-api-openapi.yml
- filename: holded-invoicing-api-openapi.yml
  format: yaml
  label: Holded Invoicing API
  slug: holded-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-invoicing-api-openapi.yml
- filename: holded-projects-api-openapi.yml
  format: yaml
  label: Holded Projects API
  slug: holded-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-projects-api-openapi.yml
- filename: holded-team-api-openapi.yml
  format: yaml
  label: Holded Team API
  slug: holded-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/openapi/holded-team-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Holded Authentication
name_suffix: Authentication
oauth_flows: []
overview: Holded secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Holded
provider_slug: holded
scheme_count: 1
schemes:
- description: Holded tenant API key, generated in account settings.
  in: header
  name: ApiKeyAuth
  parameter: key
  sources:
  - openapi/holded-openapi.yml
  type: apiKey
slug: holded-authentication
source_filename: holded-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/holded-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: key\n  description: Holded tenant API key, generated in account settings.\n  sources:\n  - openapi/holded-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holded/refs/heads/main/authentication/holded-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ERP
- CRM
- Accounting
- Invoicing
- Business Management
- SMB
- Spain
---
