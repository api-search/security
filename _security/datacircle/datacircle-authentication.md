---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datacircle-datacircle-api-openapi.yml
  format: yaml
  label: Datacircle Datacircle API
  slug: datacircle-datacircle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-datacircle-api-openapi.yml
- filename: datacircle-harvestapi-api-openapi.yml
  format: yaml
  label: Datacircle Harvest API
  slug: datacircle-harvestapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-harvestapi-api-openapi.yml
- filename: datacircle-up2data-api-openapi.yml
  format: yaml
  label: Datacircle Up2 Data API
  slug: datacircle-up2data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/openapi/datacircle-up2data-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Datacircle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datacircle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datacircle
provider_slug: datacircle
scheme_count: 1
schemes:
- description: 'Your API key: `Authorization: Bearer <your API key>`. `Authorization: Token <your API key>` works too.'
  name: token
  scheme: bearer
  sources:
  - openapi/datacircle-openapi.yml
  type: http
slug: datacircle-authentication
source_filename: datacircle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/datacircle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: 'Your API key: `Authorization: Bearer <your API key>`. `Authorization: Token\n    <your API key>` works too.'\n  sources:\n  - openapi/datacircle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacircle/refs/heads/main/authentication/datacircle-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- B2B Data
- Data Enrichment
- LinkedIn
- Profiles
- MCP
- Data Co-op
---
