---
api_key_in: []
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Uteach Inc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uteach, Inc. secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Uteach, Inc.
provider_slug: uteach-inc
scheme_count: 2
schemes:
- description: API key generated in the Uteach dashboard under Settings > Integrations, used together with the school domain to connect Zapier, Make, and Pabbly Connect. The Zapier connection prompts for "API key and domain".
  docs: https://uteach.io/support/integrations/connect-uteach-to-zapier
  name: integrationApiKey
  type: apiKey
- description: The single sign-on integration provisions users by sending a POST request to the school's "Create user API URL" authenticated with a "Create user API bearer token", both issued from the Uteach dashboard.
  docs: https://uteach.io/support/integrations/single-sign-on-for-seamless-authentication
  name: ssoCreateUserBearer
  scheme: bearer
  type: http
slug: uteach-inc-authentication
source_filename: uteach-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://uteach.io/support/integrations/connect-uteach-to-zapier\ndocs: https://uteach.io/support/integrations\nsummary:\n  types: [apiKey, http-bearer]\n  notes: Uteach publishes no public developer portal or OpenAPI. Its programmatic\n    surface is authenticated two ways, both documented in the support center -\n    an integration API key (plus school domain) for automation platforms, and a\n    bearer token for the single sign-on user-provisioning endpoint.\nschemes:\n  - name: integrationApiKey\n    type: apiKey\n    description: API key generated in the Uteach dashboard under Settings > Integrations,\n      used together with the school domain to connect Zapier, Make, and Pabbly\n      Connect. The Zapier connection prompts for \"API key and domain\".\n    docs: https://uteach.io/support/integrations/connect-uteach-to-zapier\n  - name: ssoCreateUserBearer\n    type: http\n    scheme: bearer\n    description: The single\
  \ sign-on integration provisions users by sending a POST\n      request to the school's \"Create user API URL\" authenticated with a \"Create\n      user API bearer token\", both issued from the Uteach dashboard.\n    docs: https://uteach.io/support/integrations/single-sign-on-for-seamless-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uteach-inc/refs/heads/main/authentication/uteach-inc-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Company
- Education
- eLearning
- LMS
- Online Courses
- Employee Training
- Coaching
- EdTech
---
