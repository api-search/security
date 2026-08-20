---
api_key_in:
- header
api_specs:
- filename: asknicely-contacts-api-openapi.yml
  format: yaml
  label: AskNicely Contacts API
  slug: asknicely-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-contacts-api-openapi.yml
- filename: asknicely-in-app-surveys-api-openapi.yml
  format: yaml
  label: AskNicely In-App Surveys API
  slug: asknicely-in-app-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-in-app-surveys-api-openapi.yml
- filename: asknicely-responses-api-openapi.yml
  format: yaml
  label: AskNicely Responses API
  slug: asknicely-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-responses-api-openapi.yml
- filename: asknicely-statistics-api-openapi.yml
  format: yaml
  label: AskNicely Statistics API
  slug: asknicely-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-statistics-api-openapi.yml
- filename: asknicely-surveys-api-openapi.yml
  format: yaml
  label: AskNicely Surveys API
  slug: asknicely-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-surveys-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Asknicely Authentication
name_suffix: Authentication
oauth_flows: []
overview: AskNicely secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AskNicely
provider_slug: asknicely
scheme_count: 1
schemes:
- description: The account API key, found in-platform under Settings > API. Every AskNicely user is issued their own key; create a separate user to isolate API traffic. Sending an invalid or missing key returns HTTP 401.
  in: header
  name: apiKeyAuth
  parameter: X-apikey
  sources:
  - openapi/asknicely-openapi.yml
  type: apiKey
slug: asknicely-authentication
source_filename: asknicely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/asknicely-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-apikey\n  description: The account API key, found in-platform under Settings > API. Every AskNicely\n    user is issued their own key; create a separate user to isolate API traffic. Sending an\n    invalid or missing key returns HTTP 401.\n  sources:\n  - openapi/asknicely-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/authentication/asknicely-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Customer Experience
- NPS
- Surveys
- Feedback
- Reputation Management
- Software-as-a-Service
- Customer Success
- Reviews
- SMS
---
