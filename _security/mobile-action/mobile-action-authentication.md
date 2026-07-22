---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Mobile Action Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mobile Action secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mobile Action
provider_slug: mobile-action
scheme_count: 1
schemes:
- description: Account API key supplied as the `token` query parameter on each request against https://api.mobileaction.co. Retrieve and rotate keys from the MobileAction dashboard.
  in: query
  name: apiKeyToken
  parameter: token
  sources:
  - https://docs.mobileaction.co/guide/introduction
  type: apiKey
slug: mobile-action-authentication
source_filename: mobile-action-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mobileaction.co/guide/introduction\ndocs: https://docs.mobileaction.co/guide/introduction\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  notes: >-\n    The MobileAction API uses a single API key (\"token\") passed as a query\n    parameter on every request. Keys are issued per account and metered against\n    a credit balance; the remaining balance can be checked via the /api-key\n    endpoint or the X-Credit-Remaining response header. No OAuth surface is\n    documented.\nschemes:\n- name: apiKeyToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    Account API key supplied as the `token` query parameter on each request\n    against https://api.mobileaction.co. Retrieve and rotate keys from the\n    MobileAction dashboard.\n  sources:\n  - https://docs.mobileaction.co/guide/introduction\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mobile-action/refs/heads/main/authentication/mobile-action-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- App Store Optimization
- ASO
- Mobile Marketing
- Apple Search Ads
- App Intelligence
- Ad Intelligence
- Market Intelligence
- Analytics
---
