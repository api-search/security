---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: 51offer-horizon-site-openapi.yml
  format: yaml
  label: 51offer Horizon Site API
  slug: 51offer-horizon-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/51offer/refs/heads/main/openapi/51offer-horizon-site-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 51Offer Authentication
name_suffix: Authentication
oauth_flows: []
overview: 51offer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 51offer
provider_slug: 51offer
scheme_count: 1
schemes:
- description: 'Session token header. Observed on live responses from https://www.51offer.com: Access-Control-Allow-Headers includes "token" and Access-Control-Expose-Headers is "token". Unauthenticated calls to public endpoints (e.g. GET /ngGpaCalc/constants) return 200; authenticated user endpoints return the envelope with a non-200 code field. 51offer publishes no developer auth documentation.'
  in: header
  name: tokenHeader
  parameter: token
  sources:
  - openapi/51offer-horizon-site-openapi.yml
  type: apiKey
slug: 51offer-authentication
source_filename: 51offer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/51offer-horizon-site-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenHeader\n  type: apiKey\n  in: header\n  parameter: token\n  description: 'Session token header. Observed on live responses from https://www.51offer.com:\n    Access-Control-Allow-Headers includes \"token\" and Access-Control-Expose-Headers is \"token\".\n    Unauthenticated calls to public endpoints (e.g. GET /ngGpaCalc/constants) return 200; authenticated\n    user endpoints return the envelope with a non-200 code field. 51offer publishes no developer\n    auth documentation.'\n  sources:\n  - openapi/51offer-horizon-site-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/51offer/refs/heads/main/authentication/51offer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Education
- Study Abroad
- Higher Education
- University Applications
- Students
- Language Training
- E-Commerce
- China
- Consulting
---
