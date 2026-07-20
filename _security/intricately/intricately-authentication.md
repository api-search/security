---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Intricately Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intricately secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intricately
provider_slug: intricately
scheme_count: 1
schemes:
- description: Every API request must be authenticated using the X-API-KEY HTTP header. A missing or invalid key returns response code 4000. API keys are issued to Enterprise-plan customers on request; there is no self-serve OAuth or token flow.
  in: header
  name: X-API-KEY
  parameter_name: X-API-KEY
  sources:
  - https://help.intricately.com/hc/en-us/articles/3278449675-authentication
  type: apiKey
slug: intricately-authentication
source_filename: intricately-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.intricately.com/hc/en-us/articles/3278449675-authentication\ndocs: https://help.intricately.com/hc/en-us/articles/3278449675-authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter_name: X-API-KEY\n  description: >-\n    Every API request must be authenticated using the X-API-KEY HTTP header. A missing\n    or invalid key returns response code 4000. API keys are issued to Enterprise-plan\n    customers on request; there is no self-serve OAuth or token flow.\n  sources:\n  - https://help.intricately.com/hc/en-us/articles/3278449675-authentication\naccess:\n  availability: enterprise-only\n  request_key: https://help.intricately.com/hc/en-us/articles/4416133622285-Request-an-API-Key\nnotes: >-\n  Product rebranded to the Cloud Dynamics API after HG Insights acquired Intricately\n  in 2022; the api.intricately.com\
  \ host and X-API-KEY scheme remain in use.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intricately/refs/heads/main/authentication/intricately-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- API
- Sales Intelligence
- Cloud Intelligence
- Technographics
- Data Enrichment
- Cloud Spend
- Market Intelligence
---
