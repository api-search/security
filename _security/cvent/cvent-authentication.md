---
api_key_in: []
api_specs:
- filename: cvent-openapi.yml
  format: yaml
  label: Cvent REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent/refs/heads/main/openapi/cvent-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cvent Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cvent secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cvent
provider_slug: cvent
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/cvent-openapi.yml
  type: oauth2
- description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cvent-openapi.yml
  type: http
slug: cvent-authentication
source_filename: cvent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/cvent-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.\n  sources:\n  - openapi/cvent-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent/refs/heads/main/authentication/cvent-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Attendee Hub
- Attendee Management
- Conferences
- Diagramming
- Event Management
- Event Marketing
- Events
- Exhibitors
- Hospitality
- Hospitality Cloud
- Hybrid Events
- Meetings
- OAuth 2.0
- Passkey
- Registration
- REST API
- SOAP API
- SSO
- Supplier Network
- Surveys
- Venue Management
- Venue Sourcing
- Virtual Events
- Webhooks
- White Label
---
