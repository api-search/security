---
api_key_in: []
api_specs:
- filename: openapi.yml
  format: yaml
  label: Xoxoday Plum Rewards API
  slug: plum-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoxoday/refs/heads/main/openapi/openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Xoxoday Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Xoxoday secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Xoxoday
provider_slug: xoxoday
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://accounts.xoxoday.com/chef/v1/oauth/token
  name: oauth2ClientCredentials
  sources:
  - openapi/openapi.yml
  type: oauth2
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: xoxoday-authentication
source_filename: xoxoday-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts.xoxoday.com/chef/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xoxoday/refs/heads/main/authentication/xoxoday-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Rewards
- Employee Engagement
- Gift Cards
- Incentives
- Loyalty
- Recognition
- Digital Rewards
- Points Programs
- Redemption
- Fintech
---
