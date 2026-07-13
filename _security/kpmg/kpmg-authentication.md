---
api_key_in:
- header
api_specs:
- filename: kpmg-openapi.yml
  format: yaml
  label: KPMG Origins (IWTS)
  slug: kpmg-origins-iwts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpmg/refs/heads/main/openapi/kpmg-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Kpmg Authentication
name_suffix: Authentication
oauth_flows: []
overview: KPMG secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KPMG
provider_slug: kpmg
scheme_count: 1
schemes:
- description: 'Operator-generated API access key from KPMG Origins account

    settings. The integration guide describes the key as required

    for all calls to the client-api surface; see

    https://help.kpmgorigins.com/en/articles/1850-integrating-with-origins'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/kpmg-openapi.yml
  type: apiKey
slug: kpmg-authentication
source_filename: kpmg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kpmg-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Operator-generated API access key from KPMG Origins account\n    settings. The integration guide describes the key as required\n    for all calls to the client-api surface; see\n    https://help.kpmgorigins.com/en/articles/1850-integrating-with-origins\n  sources:\n  - openapi/kpmg-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kpmg/refs/heads/main/authentication/kpmg-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Consulting
- Audit
- Tax
- Legal
- Professional Services
- Big Four
- Advisory
- AI
- Trusted AI
- ESG
- Sustainability
- Risk
- Regulation
- Cybersecurity
- Strategy
- Technology
- Workforce
- Research
- Insights
- Industry Analysis
- Transformation
- Pillar Two
- Waste Tracking
---
