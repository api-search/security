---
api_key_in: []
api_specs:
- filename: ibisworld-business-environment-api-openapi.yml
  format: yaml
  label: IBISWorld Business Environment API
  slug: ibisworld-business-environment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-business-environment-api-openapi.yml
- filename: ibisworld-classification-api-openapi.yml
  format: yaml
  label: IBISWorld Classification API
  slug: ibisworld-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-classification-api-openapi.yml
- filename: ibisworld-company-api-openapi.yml
  format: yaml
  label: IBISWorld Company API
  slug: ibisworld-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-company-api-openapi.yml
- filename: ibisworld-downloads-api-openapi.yml
  format: yaml
  label: IBISWorld Downloads API
  slug: ibisworld-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-downloads-api-openapi.yml
- filename: ibisworld-industry-api-openapi.yml
  format: yaml
  label: IBISWorld Industry API
  slug: ibisworld-industry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/openapi/ibisworld-industry-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ibisworld Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: IBISWorld secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: IBISWorld
provider_slug: ibisworld
scheme_count: 1
schemes:
- description: OAuth 2.0 bearer token authentication.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.ibisworld.com/oauth/token
  name: OAuth2
  sources:
  - openapi/ibisworld-openapi.yml
  type: oauth2
slug: ibisworld-authentication
source_filename: ibisworld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ibisworld-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ibisworld.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 bearer token authentication.\n  sources:\n  - openapi/ibisworld-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibisworld/refs/heads/main/authentication/ibisworld-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Business Intelligence
- Economics
- Industry Data
- Market Research
---
