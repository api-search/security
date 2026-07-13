---
api_key_in: []
api_specs:
- filename: litmus-instant-openapi.yml
  format: yaml
  label: Litmus Instant API
  slug: litmus-instant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-instant-openapi.yml
- filename: litmus-legacy-previews-openapi.yml
  format: yaml
  label: Litmus Legacy Previews API
  slug: litmus-legacy-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-legacy-previews-openapi.yml
- filename: litmus-email-analytics-openapi.yml
  format: yaml
  label: Litmus Email Analytics API
  slug: litmus-email-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-email-analytics-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Litmus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Litmus secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Litmus
provider_slug: litmus
scheme_count: 2
schemes:
- description: HTTP Basic Auth using Litmus account username and password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/litmus-email-analytics-openapi.yml
  - openapi/litmus-legacy-previews-openapi.yml
  type: http
- description: OAuth 2.0 access token obtained via the Litmus OAuth flow
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/litmus-instant-openapi.yml
  type: http
slug: litmus-authentication
source_filename: litmus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/litmus-email-analytics-openapi.yml, openapi/litmus-instant-openapi.yml, openapi/litmus-legacy-previews-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using Litmus account username and password\n  sources:\n  - openapi/litmus-email-analytics-openapi.yml\n  - openapi/litmus-legacy-previews-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained via the Litmus OAuth flow\n  sources:\n  - openapi/litmus-instant-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/authentication/litmus-authentication.yml
summary_line: http · 2 schemes
tags:
- Developer Tools
- Email Testing
- Marketing Tools
- Quality Assurance
---
