---
api_key_in:
- header
api_specs:
- filename: supaglue-management-api-openapi.yml
  format: yaml
  label: Supaglue Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-management-api-openapi.yml
- filename: supaglue-crm-api-openapi.yml
  format: yaml
  label: Supaglue Unified CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-crm-api-openapi.yml
- filename: supaglue-engagement-api-openapi.yml
  format: yaml
  label: Supaglue Unified Engagement API
  slug: engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-engagement-api-openapi.yml
- filename: supaglue-ticketing-api-openapi.yml
  format: yaml
  label: Supaglue Unified Ticketing API
  slug: ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/openapi/supaglue-ticketing-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Supaglue Authentication
name_suffix: Authentication
oauth_flows: []
overview: Supaglue secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Supaglue
provider_slug: supaglue
scheme_count: 1
schemes:
- description: API key to allow developers to access the API
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/supaglue-crm-api-openapi.yml
  - openapi/supaglue-engagement-api-openapi.yml
  - openapi/supaglue-management-api-openapi.yml
  - openapi/supaglue-ticketing-api-openapi.yml
  type: apiKey
slug: supaglue-authentication
source_filename: supaglue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/supaglue-crm-api-openapi.yml, openapi/supaglue-engagement-api-openapi.yml, openapi/supaglue-management-api-openapi.yml,\n  openapi/supaglue-ticketing-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key to allow developers to access the API\n  sources:\n  - openapi/supaglue-crm-api-openapi.yml\n  - openapi/supaglue-engagement-api-openapi.yml\n  - openapi/supaglue-management-api-openapi.yml\n  - openapi/supaglue-ticketing-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/supaglue/refs/heads/main/authentication/supaglue-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CRM
- HRIS
- Unified API
- Open Source
- Integrations
- Sales Engagement
---
