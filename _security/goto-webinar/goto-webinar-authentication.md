---
api_key_in: []
api_specs:
- filename: goto-webinar-attendees-api-openapi.yml
  format: yaml
  label: GoTo Webinar Attendees API
  slug: goto-webinar-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-attendees-api-openapi.yml
- filename: goto-webinar-panelists-api-openapi.yml
  format: yaml
  label: GoTo Webinar Panelists API
  slug: goto-webinar-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-panelists-api-openapi.yml
- filename: goto-webinar-polls-api-openapi.yml
  format: yaml
  label: GoTo Webinar Polls API
  slug: goto-webinar-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-polls-api-openapi.yml
- filename: goto-webinar-questions-api-openapi.yml
  format: yaml
  label: GoTo Webinar Questions API
  slug: goto-webinar-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-questions-api-openapi.yml
- filename: goto-webinar-registrants-api-openapi.yml
  format: yaml
  label: GoTo Webinar Registrants API
  slug: goto-webinar-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-registrants-api-openapi.yml
- filename: goto-webinar-sessions-api-openapi.yml
  format: yaml
  label: GoTo Webinar Sessions API
  slug: goto-webinar-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-sessions-api-openapi.yml
- filename: goto-webinar-webinars-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webinars API
  slug: goto-webinar-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webinars-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Goto Webinar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GoTo Webinar secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GoTo Webinar
provider_slug: goto-webinar
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://authentication.logmeininc.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://authentication.logmeininc.com/oauth/token
  name: oauth2
  sources:
  - openapi/goto-webinar-openapi.yml
  type: oauth2
slug: goto-webinar-authentication
source_filename: goto-webinar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/goto-webinar-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://authentication.logmeininc.com/oauth/authorize\n    tokenUrl: https://authentication.logmeininc.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/goto-webinar-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/authentication/goto-webinar-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
---
