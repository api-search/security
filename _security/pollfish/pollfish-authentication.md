---
api_key_in: []
api_specs:
- filename: pollfish-apps-api-openapi.yml
  format: yaml
  label: Pollfish Apps API
  slug: pollfish-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-apps-api-openapi.yml
- filename: pollfish-demographics-api-openapi.yml
  format: yaml
  label: Pollfish Demographics API
  slug: pollfish-demographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-demographics-api-openapi.yml
- filename: pollfish-logs-api-openapi.yml
  format: yaml
  label: Pollfish Logs API
  slug: pollfish-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-logs-api-openapi.yml
- filename: pollfish-performance-api-openapi.yml
  format: yaml
  label: Pollfish Performance API
  slug: pollfish-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-performance-api-openapi.yml
- filename: pollfish-revenue-api-openapi.yml
  format: yaml
  label: Pollfish Revenue API
  slug: pollfish-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-revenue-api-openapi.yml
- filename: pollfish-survey-distribution-api-openapi.yml
  format: yaml
  label: Pollfish Survey Distribution API
  slug: pollfish-survey-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-survey-distribution-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pollfish Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pollfish secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pollfish
provider_slug: pollfish
scheme_count: 1
schemes:
- description: HTTP Basic Auth for the Dashboard API. Username is your Pollfish account email, password is your account secret key (from Account Information in the publisher dashboard).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/pollfish-openapi.yml
  type: http
slug: pollfish-authentication
source_filename: pollfish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pollfish-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth for the Dashboard API. Username is your Pollfish account email,\n    password is your account secret key (from Account Information in the publisher dashboard).\n  sources:\n  - openapi/pollfish-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/authentication/pollfish-authentication.yml
summary_line: http · 1 scheme
tags:
- Surveys
- Market Research
- Mobile
- Monetization
- Offerwall
- Rewarded Ads
- Prodege
---
