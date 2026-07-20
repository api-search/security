---
api_key_in:
- header
api_specs:
- filename: apptimize-rest-api-openapi.yml
  format: yaml
  label: Apptimize REST API
  slug: apptimize-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apptimize/refs/heads/main/openapi/apptimize-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Apptimize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apptimize secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Apptimize
provider_slug: apptimize
scheme_count: 1
schemes:
- description: Apptimize API Token from the dashboard Install page. Distinct from the App Key used with the SDKs.
  in: header
  name: ApptimizeApiToken
  parameter: ApptimizeApiToken
  sources:
  - openapi/apptimize-rest-api-openapi.yml
  type: apiKey
slug: apptimize-authentication
source_filename: apptimize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/apptimize-rest-api-openapi.yml\ndocs: https://apptimize.com/docs/apis/rest-api.html\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  notes: >-\n    The REST API authenticates with an Apptimize API Token supplied in the\n    ApptimizeApiToken request header, obtained from the dashboard Install page.\n    This is distinct from the App Key used to initialize the client/server SDKs.\n    No OAuth or OpenID Connect surface is documented.\nschemes:\n- name: ApptimizeApiToken\n  type: apiKey\n  in: header\n  parameter: ApptimizeApiToken\n  description: Apptimize API Token from the dashboard Install page. Distinct from the App Key\n    used with the SDKs.\n  sources:\n  - openapi/apptimize-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apptimize/refs/heads/main/authentication/apptimize-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- A/B Testing
- Feature Flags
- Feature Management
- Experimentation
- Mobile
- SDK
- Optimization
---
