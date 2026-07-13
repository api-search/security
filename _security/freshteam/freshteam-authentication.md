---
api_key_in: []
api_specs:
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Employees API
  slug: freshteam-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Time-off API
  slug: freshteam-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Job Postings API
  slug: freshteam-job-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Applicants API
  slug: freshteam-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
- filename: freshteam-openapi.yml
  format: yaml
  label: Freshteam Onboarding API
  slug: freshteam-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/openapi/freshteam-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freshteam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshteam secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshteam
provider_slug: freshteam
scheme_count: 1
schemes:
- description: 'Freshteam uses a per-account API token passed as a Bearer credential. An admin generates it in the Freshteam UI under profile icon > API Settings > Your API Key, then sends it on every request as `Authorization: Bearer YOUR_API_TOKEN`. Although Freshworks documents the flow under an OAuth 2.0 heading, in practice the token is a long-lived static account key rather than a short-lived per-user-authorized token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freshteam-openapi.yml
  - https://developers.freshteam.com/api/
  type: http
slug: freshteam-authentication
source_filename: freshteam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshteam-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Freshteam uses a per-account API token passed as a Bearer credential.\n    An admin generates it in the Freshteam UI under profile icon > API Settings >\n    Your API Key, then sends it on every request as `Authorization: Bearer YOUR_API_TOKEN`.\n    Although Freshworks documents the flow under an OAuth 2.0 heading, in practice\n    the token is a long-lived static account key rather than a short-lived\n    per-user-authorized token.'\n  sources:\n  - openapi/freshteam-openapi.yml\n  - https://developers.freshteam.com/api/\nnotes: >-\n  Requests target the account-specific base https://{domain}.freshteam.com/api,\n  where {domain} is the customer subdomain. As Freshworks sunsets Freshteam,\n  new subscriptions and renewals are halted from March 7, 2026; API tokens\n  remain valid only for\
  \ existing accounts during their remaining term.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshteam/refs/heads/main/authentication/freshteam-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- HRIS
- Applicant Tracking
- ATS
- Recruiting
- Employee Management
- Onboarding
- Time Off
- HR Software
- End of Life
---
