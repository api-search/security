---
api_key_in:
- header
api_specs:
- filename: the-predictive-index-integrations-openapi.yml
  format: yaml
  label: The Predictive Index Integration API
  slug: the-predictive-index-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-predictive-index/refs/heads/main/openapi/the-predictive-index-integrations-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: The Predictive Index Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Predictive Index secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Predictive Index
provider_slug: the-predictive-index
scheme_count: 1
schemes:
- description: 'API key sent in the api-key request header (api-key: YOUR_APIKEY_GOES_HERE). The key is generated in the PI Software under a user with organization-admin permissions and cognitive access enabled. If that user is disabled, a new API key must be generated under a different active user. A key generated under a user lacking org-admin permissions yields "Authorization has been denied for this request."'
  in: header
  name: apiKeyAuth
  parameter: api-key
  sources:
  - openapi/the-predictive-index-integrations-openapi.yml
  type: apiKey
slug: the-predictive-index-authentication
source_filename: the-predictive-index-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.predictiveindex.com/getting-started\ndocs: https://developers.predictiveindex.com/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: api-key\n    description: >-\n      API key sent in the api-key request header (api-key: YOUR_APIKEY_GOES_HERE).\n      The key is generated in the PI Software under a user with organization-admin\n      permissions and cognitive access enabled. If that user is disabled, a new\n      API key must be generated under a different active user. A key generated\n      under a user lacking org-admin permissions yields \"Authorization has been\n      denied for this request.\"\n    sources: [openapi/the-predictive-index-integrations-openapi.yml]\nnotes: >-\n  Key-based auth only; no OAuth 2.0 / OpenID Connect scope surface is documented,\n  so no scopes/ artifact is\
  \ produced. Webhook listeners (outbound) authenticate\n  the reverse direction with HTTP Basic credentials embedded in the webhook URL —\n  see asyncapi/the-predictive-index-webhooks.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-predictive-index/refs/heads/main/authentication/the-predictive-index-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Talent Optimization
- HR
- Human Resources
- Assessments
- Behavioral Science
- Hiring
- Recruiting
- Employee Engagement
- Integration API
---
