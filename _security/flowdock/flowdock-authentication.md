---
api_key_in: []
api_specs:
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
- filename: flowdock-authentication-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Authentication API
  slug: flowdock-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-authentication-api-openapi.yml
- filename: flowdock-chat-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Chat API
  slug: flowdock-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-chat-api-openapi.yml
- filename: flowdock-files-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Files API
  slug: flowdock-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-files-api-openapi.yml
- filename: flowdock-flows-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Flows API
  slug: flowdock-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-flows-api-openapi.yml
- filename: flowdock-invitations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Invitations API
  slug: flowdock-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-invitations-api-openapi.yml
- filename: flowdock-messages-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Messages API
  slug: flowdock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-messages-api-openapi.yml
- filename: flowdock-organizations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Organizations API
  slug: flowdock-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-organizations-api-openapi.yml
- filename: flowdock-private-conversations-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Private Conversations API
  slug: flowdock-private-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-private-conversations-api-openapi.yml
- filename: flowdock-private-messages-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Private Messages API
  slug: flowdock-private-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-private-messages-api-openapi.yml
- filename: flowdock-sources-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Sources API
  slug: flowdock-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-sources-api-openapi.yml
- filename: flowdock-team-inbox-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Team Inbox API
  slug: flowdock-team-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-team-inbox-api-openapi.yml
- filename: flowdock-threads-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Threads API
  slug: flowdock-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-threads-api-openapi.yml
- filename: flowdock-users-api-openapi.yml
  format: yaml
  label: Flowdock (Discontinued) Users API
  slug: flowdock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowdock/refs/heads/main/openapi/flowdock-users-api-openapi.yml
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
- Integration
- Discontinued
---
