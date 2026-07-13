---
api_key_in:
- cookie
- query
api_specs:
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Tracking / Collect API
  slug: counter-dev-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Stats / Dashboard Data API
  slug: counter-dev-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
- filename: counter-dev-openapi.yml
  format: yaml
  label: Counter Account API
  slug: counter-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/openapi/counter-dev-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Counter Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Counter secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Counter
provider_slug: counter-dev
scheme_count: 2
schemes:
- description: Session cookie set on login/register, used by the dashboard UI.
  in: cookie
  name: sessionCookie
  parameter: session
  sources:
  - openapi/counter-dev-openapi.yml
  type: apiKey
- description: Read-only account token, paired with the user query parameter, for sessionless access to /query and /dump.
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/counter-dev-openapi.yml
  type: apiKey
slug: counter-dev-authentication
source_filename: counter-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/counter-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - query\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session\n  description: Session cookie set on login/register, used by the dashboard UI.\n  sources:\n  - openapi/counter-dev-openapi.yml\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Read-only account token, paired with the user query parameter, for sessionless\n    access to /query and /dump.\n  sources:\n  - openapi/counter-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/counter-dev/refs/heads/main/authentication/counter-dev-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Web Analytics
- Privacy
- Open Source
- Tracking
- Self-Hosted
---
