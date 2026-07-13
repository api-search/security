---
api_key_in:
- header
api_specs:
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Users API
  slug: learnworlds-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Courses API
  slug: learnworlds-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Enrollments API
  slug: learnworlds-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Payments API
  slug: learnworlds-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Progress API
  slug: learnworlds-progress-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Tags API
  slug: learnworlds-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
- filename: learnworlds-openapi.yml
  format: yaml
  label: LearnWorlds Webhooks API
  slug: learnworlds-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/openapi/learnworlds-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Learnworlds Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LearnWorlds secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LearnWorlds
provider_slug: learnworlds
scheme_count: 2
schemes:
- description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for a bearer access token at the school token endpoint, then pass it as Authorization: Bearer ACCESS_TOKEN.'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token
  name: oauth2ClientCredentials
  sources:
  - openapi/learnworlds-openapi.yml
  type: oauth2
- description: Client identifier header sent on every request alongside the bearer token. Its value is your API client_id.
  in: header
  name: lwClient
  parameter: Lw-Client
  sources:
  - openapi/learnworlds-openapi.yml
  type: apiKey
slug: learnworlds-authentication
source_filename: learnworlds-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/learnworlds-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://yourschool.learnworlds.com/admin/api/oauth2/access_token\n    scopes: 0\n  description: 'OAuth2 client credentials flow. Exchange your client_id and client_secret for\n    a bearer access token at the school token endpoint, then pass it as Authorization: Bearer\n    ACCESS_TOKEN.'\n  sources:\n  - openapi/learnworlds-openapi.yml\n- name: lwClient\n  type: apiKey\n  in: header\n  parameter: Lw-Client\n  description: Client identifier header sent on every request alongside the bearer token. Its\n    value is your API client_id.\n  sources:\n  - openapi/learnworlds-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnworlds/refs/heads/main/authentication/learnworlds-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Online Courses
- LMS
- eLearning
- Education
- Course Platform
- Creator Economy
---
