---
api_key_in:
- query
api_specs:
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Tracking Events API
  slug: freshpaint-tracking-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Identify API
  slug: freshpaint-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
- filename: freshpaint-openapi.yml
  format: yaml
  label: Freshpaint Page and Screen API
  slug: freshpaint-page-screen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/openapi/freshpaint-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Freshpaint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freshpaint secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freshpaint
provider_slug: freshpaint
scheme_count: 1
schemes:
- description: Freshpaint authenticates server-side events with your environment ID (token). The token is supplied inside the event payload as properties.token rather than as a header or query string; this scheme documents the token-based, in-body authentication used by the HTTP API. Obtain the token from the Server Side API section of the Sources page in the Freshpaint app.
  in: query
  name: EnvironmentToken
  parameter: token
  sources:
  - openapi/freshpaint-openapi.yml
  type: apiKey
slug: freshpaint-authentication
source_filename: freshpaint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freshpaint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: EnvironmentToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Freshpaint authenticates server-side events with your environment ID (token).\n    The token is supplied inside the event payload as properties.token rather than as a header\n    or query string; this scheme documents the token-based, in-body authentication used by the\n    HTTP API. Obtain the token from the Server Side API section of the Sources page in the Freshpaint\n    app.\n  sources:\n  - openapi/freshpaint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshpaint/refs/heads/main/authentication/freshpaint-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Customer Data Platform
- Event Tracking
- Healthcare
- HIPAA
- Privacy
- Analytics
---
