---
api_key_in: []
api_specs:
- filename: gotowebinar-attendees-api-openapi.yml
  format: yaml
  label: GoToWebinar Attendees API
  slug: gotowebinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-attendees-api-openapi.yml
- filename: gotowebinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoToWebinar Co-Organizers API
  slug: gotowebinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-co-organizers-api-openapi.yml
- filename: gotowebinar-panelists-api-openapi.yml
  format: yaml
  label: GoToWebinar Panelists API
  slug: gotowebinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-panelists-api-openapi.yml
- filename: gotowebinar-polls-api-openapi.yml
  format: yaml
  label: GoToWebinar Polls API
  slug: gotowebinar-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-polls-api-openapi.yml
- filename: gotowebinar-questions-api-openapi.yml
  format: yaml
  label: GoToWebinar Questions API
  slug: gotowebinar-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-questions-api-openapi.yml
- filename: gotowebinar-recordings-api-openapi.yml
  format: yaml
  label: GoToWebinar Recordings API
  slug: gotowebinar-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-recordings-api-openapi.yml
- filename: gotowebinar-registrants-api-openapi.yml
  format: yaml
  label: GoToWebinar Registrants API
  slug: gotowebinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-registrants-api-openapi.yml
- filename: gotowebinar-sessions-api-openapi.yml
  format: yaml
  label: GoToWebinar Sessions API
  slug: gotowebinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-sessions-api-openapi.yml
- filename: gotowebinar-surveys-api-openapi.yml
  format: yaml
  label: GoToWebinar Surveys API
  slug: gotowebinar-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-surveys-api-openapi.yml
- filename: gotowebinar-user-subscriptions-api-openapi.yml
  format: yaml
  label: GoToWebinar User Subscriptions API
  slug: gotowebinar-user-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-user-subscriptions-api-openapi.yml
- filename: gotowebinar-webhooks-api-openapi.yml
  format: yaml
  label: GoToWebinar Webhooks API
  slug: gotowebinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webhooks-api-openapi.yml
- filename: gotowebinar-webinars-api-openapi.yml
  format: yaml
  label: GoToWebinar Webinars API
  slug: gotowebinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/openapi/gotowebinar-webinars-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gotowebinar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GoToWebinar secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GoToWebinar
provider_slug: gotowebinar
scheme_count: 1
schemes:
- description: OAuth 2.0 via the GoTo authentication service.
  flows:
  - authorizationUrl: https://authentication.logmeininc.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://authentication.logmeininc.com/oauth/token
  name: oauth2
  sources:
  - openapi/gotowebinar-rest-openapi.yml
  - openapi/gotowebinar-webhooks-openapi.yml
  type: oauth2
slug: gotowebinar-authentication
source_filename: gotowebinar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gotowebinar-rest-openapi.yml, openapi/gotowebinar-webhooks-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authentication.logmeininc.com/oauth/authorize\n    tokenUrl: https://authentication.logmeininc.com/oauth/token\n    scopes: 2\n  description: OAuth 2.0 via the GoTo authentication service.\n  sources:\n  - openapi/gotowebinar-rest-openapi.yml\n  - openapi/gotowebinar-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gotowebinar/refs/heads/main/authentication/gotowebinar-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Attendees
- Collaboration
- Communications
- Event
- Meetings
- Registrants
- Sessions
- Surveys
- Video Conferencing
- Virtual Events
- Webhook
- Webinars
---
