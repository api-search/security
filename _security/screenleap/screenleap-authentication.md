---
api_key_in:
- header
api_specs:
- filename: screenleap-openapi.yml
  format: yaml
  label: Screenleap API
  slug: screenleap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/screenleap/refs/heads/main/openapi/screenleap-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Screenleap Authentication
name_suffix: Authentication
oauth_flows: []
overview: Screenleap secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Screenleap
provider_slug: screenleap
scheme_count: 2
schemes:
- description: Your Screenleap account identifier.
  in: header
  name: accountId
  parameter: accountid
  sources:
  - openapi/screenleap-openapi.yml
  type: apiKey
- description: Your Screenleap authentication token. SSL required when sending it.
  in: header
  name: authToken
  parameter: authtoken
  sources:
  - openapi/screenleap-openapi.yml
  type: apiKey
slug: screenleap-authentication
source_filename: screenleap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/screenleap-openapi.yml\ndocs: https://www.screenleap.com/api/native/doc\nnotes: >-\n  Screenleap authenticates every request with two apiKey headers — accountid\n  (your account identifier, may also be a query parameter) and authtoken (your\n  auth token). SSL is required for any request carrying the auth token. There is\n  no OAuth surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: accountId\n  type: apiKey\n  in: header\n  parameter: accountid\n  description: Your Screenleap account identifier.\n  sources:\n  - openapi/screenleap-openapi.yml\n- name: authToken\n  type: apiKey\n  in: header\n  parameter: authtoken\n  description: Your Screenleap authentication token. SSL required when sending it.\n  sources:\n  - openapi/screenleap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenleap/refs/heads/main/authentication/screenleap-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Screen Sharing
- Video Conferencing
- Screen Recording
- Collaboration
- Real-Time Communication
- WebRTC
- Embeddable
- Developer API
---
