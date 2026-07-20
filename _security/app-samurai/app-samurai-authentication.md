---
api_key_in:
- path
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: App Samurai Authentication
name_suffix: Authentication
oauth_flows: []
overview: App Samurai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: App Samurai
provider_slug: app-samurai
scheme_count: 1
schemes:
- description: Unique per-customer API key provided by the App Samurai account manager, passed as the final path segment of the Campaign Spend endpoint.
  in: path
  name: apiKeyPath
  parameter: api_key
  sources:
  - https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api
  type: apiKey
slug: app-samurai-authentication
source_filename: app-samurai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api\ndocs: https://help.appsamurai.com/en/collections/12520260-campaign-spend-api-documentation\nsummary:\n  types: [apiKey]\n  api_key_in: [path]\n  oauth2_flows: []\n  notes: >-\n    The App Samurai Campaign Spend API authenticates with a static per-customer\n    API key that is embedded directly in the request path segment\n    (/api/customer-pull/spent/{api_key}). The key is issued by the customer's\n    account manager; there is no OAuth, no self-service key rotation portal, and\n    no documented scope model. Mobile SDKs (Ads / Storyly / attribution) use\n    per-app tokens configured at SDK init, out of band from this REST API.\nschemes:\n  - name: apiKeyPath\n    type: apiKey\n    in: path\n    parameter: api_key\n    description: >-\n      Unique per-customer API key provided by the App Samurai account manager,\n      passed as the final path\
  \ segment of the Campaign Spend endpoint.\n    sources: [https://help.appsamurai.com/en/articles/11105087-appsamurai-campaign-spend-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/app-samurai/refs/heads/main/authentication/app-samurai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Mobile
- Advertising
- User Acquisition
- App Marketing
- Attribution
- Monetization
- Mobile SDK
- Programmatic
---
