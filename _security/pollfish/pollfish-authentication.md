---
api_key_in: []
api_specs:
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Apps API
  slug: pollfish-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Performance API
  slug: pollfish-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Revenue API
  slug: pollfish-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Respondent Demographics API
  slug: pollfish-respondent-demographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish User Logs API
  slug: pollfish-user-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Survey Distribution and Offerwall API
  slug: pollfish-survey-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Server-to-Server Callbacks
  slug: pollfish-s2s-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
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
