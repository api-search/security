---
api_key_in: []
api_specs:
- filename: cvent-platform-openapi.yml
  format: yaml
  label: Cvent Platform REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-platform/refs/heads/main/openapi/cvent-platform-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cvent Platform Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cvent Platform secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cvent Platform
provider_slug: cvent-platform
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/cvent-platform-openapi.yml
  type: oauth2
- description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cvent-platform-openapi.yml
  type: http
slug: cvent-platform-authentication
source_filename: cvent-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-platform-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/cvent-platform-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.\n  sources:\n  - openapi/cvent-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-platform/refs/heads/main/authentication/cvent-platform-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Attendee Hub
- Conferences
- Event Management
- Event Marketing
- Events
- Hospitality
- Hospitality Cloud
- Hybrid Events
- Meetings
- OAuth 2.0
- Passkey
- Registration
- REST API
- Supplier Network
- Surveys
- Venue Management
- Virtual Events
---
