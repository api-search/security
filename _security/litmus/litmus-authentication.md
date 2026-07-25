---
api_key_in: []
api_specs:
- filename: litmus-analytics-api-openapi.yml
  format: yaml
  label: Litmus Analytics API
  slug: litmus-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-analytics-api-openapi.yml
- filename: litmus-campaigns-api-openapi.yml
  format: yaml
  label: Litmus Campaigns API
  slug: litmus-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-campaigns-api-openapi.yml
- filename: litmus-clients-api-openapi.yml
  format: yaml
  label: Litmus Clients API
  slug: litmus-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-clients-api-openapi.yml
- filename: litmus-previews-api-openapi.yml
  format: yaml
  label: Litmus Previews API
  slug: litmus-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-previews-api-openapi.yml
- filename: litmus-results-api-openapi.yml
  format: yaml
  label: Litmus Results API
  slug: litmus-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-results-api-openapi.yml
- filename: litmus-tests-api-openapi.yml
  format: yaml
  label: Litmus Tests API
  slug: litmus-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litmus/refs/heads/main/openapi/litmus-tests-api-openapi.yml
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
