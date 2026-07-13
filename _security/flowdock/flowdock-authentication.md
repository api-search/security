---
api_key_in: []
api_specs:
- filename: flowdock-rest-api-openapi.yml
  format: yaml
  label: Flowdock REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-rest-api-openapi.yml
- filename: flowdock-push-api-openapi.yml
  format: yaml
  label: Flowdock Push API (Deprecated)
  slug: push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-push-api-openapi.yml
- filename: flowdock-streaming-api-asyncapi.yml
  format: yaml
  label: Flowdock Streaming API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/asyncapi/flowdock-streaming-api-asyncapi.yml
- filename: flowdock-scim-api-openapi.yml
  format: yaml
  label: Flowdock SCIM Provisioning API
  slug: scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-scim-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Flowdock Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Flowdock (Discontinued) secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Flowdock (Discontinued)
provider_slug: flowdock
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://api.flowdock.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://api.flowdock.com/oauth/token
  name: oauth2
  sources:
  - openapi/flowdock-rest-api-openapi.yml
  type: oauth2
- description: Email + password, or personal API token as the username.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/flowdock-rest-api-openapi.yml
  type: http
- description: SCIM bearer token issued during SSO setup.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flowdock-scim-api-openapi.yml
  type: http
slug: flowdock-authentication
source_filename: flowdock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flowdock-rest-api-openapi.yml, openapi/flowdock-scim-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.flowdock.com/oauth/authorize\n    tokenUrl: https://api.flowdock.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/flowdock-rest-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Email + password, or personal API token as the username.\n  sources:\n  - openapi/flowdock-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: SCIM bearer token issued during SSO setup.\n  sources:\n  - openapi/flowdock-scim-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/authentication/flowdock-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Team Chat
- Team Inbox
- Collaboration
- Real-Time Messaging
- Integrations
- Discontinued
---
