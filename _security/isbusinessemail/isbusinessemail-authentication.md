---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: isbusinessemail-check-api-openapi.yml
  format: yaml
  label: isBusinessEmail Check API
  slug: isbusinessemail-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-check-api-openapi.yml
- filename: isbusinessemail-feedback-api-openapi.yml
  format: yaml
  label: isBusinessEmail Feedback API
  slug: isbusinessemail-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-feedback-api-openapi.yml
- filename: isbusinessemail-health-api-openapi.yml
  format: yaml
  label: isBusinessEmail Health API
  slug: isbusinessemail-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-health-api-openapi.yml
- filename: isbusinessemail-usage-api-openapi.yml
  format: yaml
  label: isBusinessEmail Usage API
  slug: isbusinessemail-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/openapi/isbusinessemail-usage-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Isbusinessemail Authentication
name_suffix: Authentication
oauth_flows: []
overview: isBusinessEmail secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: isBusinessEmail
provider_slug: isbusinessemail
scheme_count: 2
schemes:
- description: 'Authorization: Bearer ibe_live_...'
  name: bearer
  scheme: bearer
  sources:
  - openapi/isbusinessemail-openapi.json
  type: http
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/isbusinessemail-openapi.json
  type: apiKey
slug: isbusinessemail-authentication
source_filename: isbusinessemail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: derived\nsource: openapi/isbusinessemail-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer ibe_live_...'\n  sources:\n  - openapi/isbusinessemail-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/isbusinessemail-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isbusinessemail/refs/heads/main/authentication/isbusinessemail-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- EmailVerification
- BusinessTools
- API
- EUHosted
---
