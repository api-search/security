---
api_key_in: []
api_specs:
- filename: bezero-carbon-projects-api-openapi.yml
  format: yaml
  label: BeZero Carbon Projects API
  slug: bezero-carbon-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/openapi/bezero-carbon-projects-api-openapi.yml
- filename: bezero-carbon-ratings-api-openapi.yml
  format: yaml
  label: BeZero Carbon Ratings API
  slug: bezero-carbon-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/openapi/bezero-carbon-ratings-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bezero Carbon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: BeZero Carbon secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: BeZero Carbon
provider_slug: bezero-carbon
scheme_count: 1
schemes:
- description: This API uses OAuth 2 with Client Credentials
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://login.bezerocarbonmarkets.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/bezero-carbon-ratings-openapi.yml
  type: oauth2
slug: bezero-carbon-authentication
source_filename: bezero-carbon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: derived\nsource: openapi/bezero-carbon-ratings-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.bezerocarbonmarkets.com/oauth2/token\n    scopes: 4\n  description: This API uses OAuth 2 with Client Credentials\n  sources:\n  - openapi/bezero-carbon-ratings-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bezero-carbon/refs/heads/main/authentication/bezero-carbon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Carbon Ratings
- Carbon Markets
- Climate
- Sustainability
- ESG
- Ratings
- Reference Data
- Market Intelligence
- Risk Analysis
---
