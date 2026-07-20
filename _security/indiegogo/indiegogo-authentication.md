---
api_key_in: []
api_specs:
- filename: indiegogo-public-openapi.yml
  format: yaml
  label: Indiegogo Public API
  slug: indiegogo-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indiegogo/refs/heads/main/openapi/indiegogo-public-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Indiegogo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indiegogo secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Indiegogo
provider_slug: indiegogo
scheme_count: 1
schemes:
- description: Public endpoints are unauthenticated. No API key, token, or OAuth flow is required to call the creators or projects public endpoints.
  name: public
  sources:
  - openapi/indiegogo-public-openapi.yml
  type: none
slug: indiegogo-authentication
source_filename: indiegogo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.indiegogo.com/article/616-indiegogo-public-api\ndocs: https://help.indiegogo.com/category/617-developer-resources\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The current Indiegogo Public API (https://www.indiegogo.com/api/public/*) is\n    read-only and requires NO authentication; all endpoints are open and results\n    are cached for a short duration. A separate, legacy Partner/Campaign API\n    (api.indiegogo.com/:version/) historically used an application api_token plus\n    an optional per-user access_token; that host now returns 403 / redirects and\n    is treated as deprecated.\nschemes:\n  - name: public\n    type: none\n    description: >-\n      Public endpoints are unauthenticated. No API key, token, or OAuth flow is\n      required to call the creators or projects public endpoints.\n    sources: [openapi/indiegogo-public-openapi.yml]\nlegacy:\n  - name: api_token\n\
  \    type: apiKey\n    in: query\n    parameter: api_token\n    status: deprecated\n    description: >-\n      Application-level token on the legacy Partner API (api.indiegogo.com), e.g.\n      /1/campaigns/{id}.json?api_token={token}. Host now 403/redirects.\n  - name: access_token\n    type: apiKey\n    in: query\n    parameter: access_token\n    status: deprecated\n    description: >-\n      Optional per-user (campaign creator / team member) token on the legacy\n      Partner API that unlocked privileged campaign data. Never expose in HTML.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indiegogo/refs/heads/main/authentication/indiegogo-authentication.yml
summary_line: none · 1 scheme
tags:
- Company
- Consumer
- Crowdfunding
- Fundraising
- Campaigns
- Payments
- Marketplace
- Creators
---
