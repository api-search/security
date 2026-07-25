---
api_key_in:
- header
- query
api_specs:
- filename: dpla-authentication-api-openapi.yml
  format: yaml
  label: Digital Public Library of America Authentication API
  slug: dpla-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/openapi/dpla-authentication-api-openapi.yml
- filename: dpla-items-api-openapi.yml
  format: yaml
  label: Digital Public Library of America Items API
  slug: dpla-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/openapi/dpla-items-api-openapi.yml
- filename: dpla-primary-source-sets-api-openapi.yml
  format: yaml
  label: Digital Public Library of America Primary Source Sets API
  slug: dpla-primary-source-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/openapi/dpla-primary-source-sets-api-openapi.yml
- filename: dpla-utilities-api-openapi.yml
  format: yaml
  label: Digital Public Library of America Utilities API
  slug: dpla-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/openapi/dpla-utilities-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dpla Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Public Library of America secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Digital Public Library of America
provider_slug: dpla
scheme_count: 2
schemes:
- description: DPLA API key passed as a query parameter. Obtain a free key by sending a POST to /api_key/{email}.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: DPLA API key passed as an Authorization header value (not Bearer scheme — just the raw 32-character key).
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: dpla-authentication
source_filename: dpla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: DPLA API key passed as a query parameter. Obtain a free key by sending a POST\n    to /api_key/{email}.\n  sources:\n  - openapi/openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: DPLA API key passed as an Authorization header value (not Bearer scheme — just\n    the raw 32-character key).\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dpla/refs/heads/main/authentication/dpla-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cultural Heritage
- Libraries
- Archives
- Museums
- Open Data
- Metadata
- Digital Collections
- Public Domain
---
