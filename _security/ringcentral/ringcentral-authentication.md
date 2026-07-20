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
method: searched
name: Ringcentral Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- jwt
overview: RingCentral secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and jwt flow(s).
provider_name: RingCentral
provider_slug: ringcentral
scheme_count: 1
schemes:
- docs: https://developers.ringcentral.com/guide/authentication/auth-code-flow
  flows:
  - authorizationUrl: https://platform.ringcentral.com/restapi/oauth/authorize
    flow: authorizationCode
    pkce: true
    scopes: 37
    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token
  - flow: jwt
    grant: urn:ietf:params:oauth:grant-type:jwt-bearer
    notes: JWT auth credential flow for server-only apps.
    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token
  - flow: clientCredentials
    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token
  name: OAuth2
  sources:
  - openapi/ringcentral-platform-openapi.yml
  type: oauth2
slug: ringcentral-authentication
source_filename: ringcentral-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/ringcentral-platform-openapi.yml\ndocs: https://developers.ringcentral.com/guide/authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - jwt\n  notes: >-\n    RingCentral standardized on OAuth 2.0 (all password/ROPC flows retired). Access\n    tokens are bearer tokens with a ~1 hour TTL; refresh tokens rotate. Documented\n    grant types: Authorization Code (with PKCE) for user apps, JWT assertion (RFC\n    7523) for server-only/no-UI apps, and Client Credentials for app-context calls.\n    The public OpenAPI only encodes the authorizationCode scheme.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://platform.ringcentral.com/restapi/oauth/authorize\n    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token\n    scopes: 37\n    pkce: true\n  - flow: jwt\n    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token\n\
  \    grant: urn:ietf:params:oauth:grant-type:jwt-bearer\n    notes: JWT auth credential flow for server-only apps.\n  - flow: clientCredentials\n    tokenUrl: https://platform.ringcentral.com/restapi/oauth/token\n  sources:\n  - openapi/ringcentral-platform-openapi.yml\n  docs: https://developers.ringcentral.com/guide/authentication/auth-code-flow\ntoken:\n  type: bearer\n  ttl_seconds: 3600\n  refresh: true\n  revocation_endpoint: https://platform.ringcentral.com/restapi/oauth/revoke\n"
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
