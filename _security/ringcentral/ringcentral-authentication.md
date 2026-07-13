---
api_key_in: []
api_specs:
- filename: ringcentral-platform-openapi.yml
  format: yaml
  label: RingCentral Voice API
  slug: ringcentral-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/openapi/ringcentral-platform-openapi.yml
- filename: ringcentral-subscriptions-asyncapi.yaml
  format: yaml
  label: RingCentral Webhooks and Subscriptions API
  slug: ringcentral-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/asyncapi/ringcentral-subscriptions-asyncapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ringcentral Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RingCentral secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RingCentral
provider_slug: ringcentral
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://platform.ringcentral.com/restapi/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token
  name: OAuth2
  sources:
  - openapi/ringcentral-platform-openapi.yml
  type: oauth2
slug: ringcentral-authentication
source_filename: ringcentral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ringcentral-platform-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.ringcentral.com/restapi/oauth/authorize\n    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token\n    scopes: 0\n  sources:\n  - openapi/ringcentral-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ringcentral/refs/heads/main/authentication/ringcentral-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Communications
- UCaaS
- Voice
- Video
- Contact Center
- SMS
- Messaging
- Fax
---
