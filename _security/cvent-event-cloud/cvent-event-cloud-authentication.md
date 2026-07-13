---
api_key_in: []
api_specs:
- filename: cvent-event-cloud-openapi.yml
  format: yaml
  label: Cvent Platform REST API (Event Cloud)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-event-cloud/refs/heads/main/openapi/cvent-event-cloud-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cvent Event Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cvent Event Cloud secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cvent Event Cloud
provider_slug: cvent-event-cloud
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 9
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/cvent-event-cloud-openapi.yml
  type: oauth2
- description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cvent-event-cloud-openapi.yml
  type: http
slug: cvent-event-cloud-authentication
source_filename: cvent-event-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cvent-event-cloud-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 9\n  sources:\n  - openapi/cvent-event-cloud-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Client ID / client secret Basic auth used only for the /ea/oauth2/token call.\n  sources:\n  - openapi/cvent-event-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-event-cloud/refs/heads/main/authentication/cvent-event-cloud-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Attendee Hub
- Attendees
- Event Cloud
- Event Management
- Event Marketing
- Events
- Hybrid Events
- OAuth 2.0
- Onsite
- Registration
- REST
- Sessions
- Speakers
- Surveys
- Virtual Events
- Webhooks
---
