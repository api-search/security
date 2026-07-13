---
api_key_in:
- header
api_specs:
- filename: bugsnag-data-access-openapi.yml
  format: yaml
  label: Bugsnag Data Access API
  slug: data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-data-access-openapi.yml
- filename: bugsnag-error-reporting-openapi.yml
  format: yaml
  label: Bugsnag Error Reporting API
  slug: error-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-error-reporting-openapi.yml
- filename: bugsnag-session-tracking-openapi.yml
  format: yaml
  label: Bugsnag Session Tracking API
  slug: session-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-session-tracking-openapi.yml
- filename: bugsnag-build-openapi.yml
  format: yaml
  label: Bugsnag Build API
  slug: build-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-build-openapi.yml
- filename: bugsnag-trace-openapi.yml
  format: yaml
  label: Bugsnag Trace API
  slug: trace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/openapi/bugsnag-trace-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Bugsnag Authentication
name_suffix: Authentication
oauth_flows: []
overview: bugsnag secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: bugsnag
provider_slug: bugsnag
scheme_count: 1
schemes:
- description: Personal auth token sent as "token YOUR-AUTH-TOKEN". The token can be found in the Bugsnag account settings under the API section.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/bugsnag-data-access-openapi.yml
  type: apiKey
slug: bugsnag-authentication
source_filename: bugsnag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bugsnag-data-access-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Personal auth token sent as \"token YOUR-AUTH-TOKEN\". The token can be found in\n    the Bugsnag account settings under the API section.\n  sources:\n  - openapi/bugsnag-data-access-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bugsnag/refs/heads/main/authentication/bugsnag-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
