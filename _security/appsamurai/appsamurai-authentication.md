---
api_key_in:
- path
api_specs:
- filename: appsamurai-campaign-spend-openapi.yml
  format: yaml
  label: AppSamurai Campaign Spend API
  slug: appsamurai-campaign-spend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/openapi/appsamurai-campaign-spend-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Appsamurai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appsamurai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appsamurai
provider_slug: appsamurai
scheme_count: 1
schemes:
- docs: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api
  in: path
  issuance: manual (provided by AppSamurai account manager)
  name: PathApiKey
  parameter: api_key
  sources:
  - openapi/appsamurai-campaign-spend-openapi.yml
  type: apiKey
slug: appsamurai-authentication
source_filename: appsamurai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api\ndocs: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api\nsummary:\n  types: [apiKey]\n  api_key_in: [path]\n  oauth2_flows: []\n  notes: >-\n    The Campaign Spend API authenticates with a single account-scoped API key,\n    provided by an AppSamurai account manager and passed as a path segment in\n    the request URL (/api/customer-pull/spent/{api_key}). No OAuth, no\n    self-service key issuance documented.\nschemes:\n  - name: PathApiKey\n    type: apiKey\n    in: path\n    parameter: api_key\n    issuance: manual (provided by AppSamurai account manager)\n    sources: [openapi/appsamurai-campaign-spend-openapi.yml]\n    docs: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsamurai/refs/heads/main/authentication/appsamurai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mobile
- Advertising
- User Acquisition
- Marketing
- App Growth
- Attribution
- Analytics
- Mobile Marketing
- SDK
---
