---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: RingCentral Events API
  slug: ringcentral-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/openapi/openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hopin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: RingCentral Events secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: RingCentral Events
provider_slug: hopin
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.events.ringcentral.com/v1/auth/token
  name: oauth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: hopin-authentication
source_filename: hopin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.events.ringcentral.com/v1/auth/token\n    scopes: 2\n  description: OAuth 2.0 Client Credentials flow\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopin/refs/heads/main/authentication/hopin-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Events
- Virtual Events
- Hybrid Events
- Webinars
- Event Management
- Registration
- Sessions
- Networking
---
