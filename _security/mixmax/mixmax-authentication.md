---
api_key_in:
- header
- query
api_specs:
- filename: mixmax-openapi.yml
  format: yaml
  label: Mixmax REST API
  slug: mixmax-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/openapi/mixmax-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mixmax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mixmax secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mixmax
provider_slug: mixmax
scheme_count: 1
schemes:
- alt_in: query
  alt_parameter: apiToken
  description: Mixmax authenticates every REST request with an API token. Create the token under Settings > Integrations (app.mixmax.com/dashboard/settings/personal/integrations); it is displayed only once. Send it as the X-API-Token request header, or as the apiToken query-string parameter.
  in: header
  name: apiToken
  parameter: X-API-Token
  sources:
  - openapi/mixmax-openapi.yml
  - https://developer.mixmax.com/reference/getting-started-with-the-api
  type: apiKey
slug: mixmax-authentication
source_filename: mixmax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.mixmax.com/reference/getting-started-with-the-api\ndocs: https://developer.mixmax.com/reference/getting-started-with-the-api\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter: X-API-Token\n    alt_in: query\n    alt_parameter: apiToken\n    description: >-\n      Mixmax authenticates every REST request with an API token. Create the token\n      under Settings > Integrations (app.mixmax.com/dashboard/settings/personal/integrations);\n      it is displayed only once. Send it as the X-API-Token request header, or as\n      the apiToken query-string parameter.\n    sources: [openapi/mixmax-openapi.yml, https://developer.mixmax.com/reference/getting-started-with-the-api]\nnotes:\n  - Some endpoints (meeting summaries/transcripts) additionally require the workspace-level mixmaxApi feature to be enabled by\
  \ an admin.\n  - No OAuth 2.0 / OpenID Connect flow is documented for the public REST API; message-integration surfaces use their own SDK context.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mixmax/refs/heads/main/authentication/mixmax-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Saas
- Sales Engagement
- Email
- Sales
- CRM
- Productivity
- Meetings
- Sequences
---
