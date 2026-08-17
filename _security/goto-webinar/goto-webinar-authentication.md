---
api_key_in: []
api_specs:
- filename: goto-webinar-openapi.yml
  format: yaml
  label: GoTo Webinar REST API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/_original/goto-webinar-openapi.yml
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
- filename: goto-webinar-co-organizers-api-openapi.yml
  format: yaml
  label: GoTo Webinar Co Organizers API
  slug: goto-webinar-co-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-co-organizers-api-openapi.yml
- filename: goto-webinar-recordingassets-api-openapi.yml
  format: yaml
  label: GoTo Webinar Recording Assets API
  slug: goto-webinar-recordingassets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-recordingassets-api-openapi.yml
- filename: goto-webinar-webhooks-api-openapi.yml
  format: yaml
  label: GoTo Webinar Webhooks API
  slug: goto-webinar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/openapi/goto-webinar-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Goto Webinar Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: GoTo Webinar secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: GoTo Webinar
provider_slug: goto-webinar
scheme_count: 1
schemes:
- description: To use this API you must provide an OAuth token requested from GoTo's authorization server. The spec's own description still points at the legacy LogMeIn documentation URL; the current guides live under developer.goto.com/guides/Authentication/.
  flows:
  - authorizationUrl: https://identity.goto.com/oauth/authorize
    flow: authorizationCode
    note: The recommended flow. The OpenAPI names authentication.logmeininc.com; the RFC 8414 metadata served at that exact host reports issuer https://identity.goto.com and lists identity.goto.com endpoints, so both hostnames front one authorization server mid-rename. GoTo publishes a migration guide for the transition.
    pkce: S256
    refreshUrl: https://identity.goto.com/oauth/token
    scopes: 0
    spec_declares:
      authorizationUrl: https://authentication.logmeininc.com/oauth/authorize
      tokenUrl: https://authentication.logmeininc.com/oauth/token
    tokenUrl: https://identity.goto.com/oauth/token
  - deprecated: true
    flow: password
    note: '"Direct Login". GoTo''s SDK guides state "This authentication API is now deprecated. All new clients will not be able to use this API. If you have a client for which the direct login works, that will continue to work for now." It is still declared in the live contract — the spec advertises a grant the docs bar new clients from using. GoTo publishes a Direct Login migration guide at /guides/References/05_Direct-Login_migration/.'
    refreshUrl: https://identity.goto.com/oauth/token
    scopes: 0
    tokenUrl: https://identity.goto.com/oauth/token
  header: Authorization
  in: header
  name: OAuth2
  scheme: Bearer
  sources:
  - openapi/_original/goto-webinar-openapi.yml
  - openapi/goto-webinar-webinars-api-openapi.yml
  - openapi/goto-webinar-sessions-api-openapi.yml
  - openapi/goto-webinar-registrants-api-openapi.yml
  - openapi/goto-webinar-attendees-api-openapi.yml
  - openapi/goto-webinar-panelists-api-openapi.yml
  - openapi/goto-webinar-co-organizers-api-openapi.yml
  - openapi/goto-webinar-recordingassets-api-openapi.yml
  - openapi/goto-webinar-webhooks-api-openapi.yml
  type: oauth2
slug: goto-webinar-authentication
source_filename: goto-webinar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/goto-webinar-openapi.yml\ndocs:\n- https://developer.goto.com/guides/Authentication/03_HOW_accessToken/\n- https://developer.goto.com/guides/Authentication/03.1_HOW_accessTokenPAT/\n- https://developer.goto.com/guides/Authentication/05_HOW_refreshToken/\n- https://developer.goto.com/guides/Authentication/New_Token_Retrieval_Migration_Guide/\n- https://developer.goto.com/guides/Get%20Started/02_HOW_createClient/\nmetadata_document:\n  url: https://identity.goto.com/.well-known/oauth-authorization-server\n  status: 200\n  spec: RFC 8414\n  file: well-known/goto-webinar-oauth-authorization-server.json\n  alias_host: https://authentication.logmeininc.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, password]\n  api_key_in: []\n  bearer: true\n  issuer: https://identity.goto.com\n  pkce: [S256]\n  scope: 'collab:'\nschemes:\n- name: OAuth2\n  type: oauth2\n\
  \  in: header\n  header: Authorization\n  scheme: Bearer\n  description: >-\n    To use this API you must provide an OAuth token requested from GoTo's\n    authorization server. The spec's own description still points at the legacy\n    LogMeIn documentation URL; the current guides live under\n    developer.goto.com/guides/Authentication/.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://identity.goto.com/oauth/authorize\n    tokenUrl: https://identity.goto.com/oauth/token\n    refreshUrl: https://identity.goto.com/oauth/token\n    spec_declares:\n      authorizationUrl: https://authentication.logmeininc.com/oauth/authorize\n      tokenUrl: https://authentication.logmeininc.com/oauth/token\n    pkce: S256\n    scopes: 0\n    note: >-\n      The recommended flow. The OpenAPI names authentication.logmeininc.com;\n      the RFC 8414 metadata served at that exact host reports issuer\n      https://identity.goto.com and lists identity.goto.com endpoints, so both\n     \
  \ hostnames front one authorization server mid-rename. GoTo publishes a\n      migration guide for the transition.\n  - flow: password\n    tokenUrl: https://identity.goto.com/oauth/token\n    refreshUrl: https://identity.goto.com/oauth/token\n    scopes: 0\n    deprecated: true\n    note: >-\n      \"Direct Login\". GoTo's SDK guides state \"This authentication API is now\n      deprecated. All new clients will not be able to use this API. If you have\n      a client for which the direct login works, that will continue to work for\n      now.\" It is still declared in the live contract — the spec advertises a\n      grant the docs bar new clients from using. GoTo publishes a Direct Login\n      migration guide at /guides/References/05_Direct-Login_migration/.\n  sources:\n  - openapi/_original/goto-webinar-openapi.yml\n  - openapi/goto-webinar-webinars-api-openapi.yml\n  - openapi/goto-webinar-sessions-api-openapi.yml\n  - openapi/goto-webinar-registrants-api-openapi.yml\n  - openapi/goto-webinar-attendees-api-openapi.yml\n\
  \  - openapi/goto-webinar-panelists-api-openapi.yml\n  - openapi/goto-webinar-co-organizers-api-openapi.yml\n  - openapi/goto-webinar-recordingassets-api-openapi.yml\n  - openapi/goto-webinar-webhooks-api-openapi.yml\nendpoints:\n  authorization: https://identity.goto.com/oauth/authorize\n  token: https://identity.goto.com/oauth/token\n  introspection: https://identity.goto.com/oauth/introspect\n  revocation: https://identity.goto.com/oauth/revoke\n  jwks: https://identity.goto.com/oauth/jwks.json\n  client_management: https://developer.logmeininc.com/clients\nsupported:\n  response_types: [code]\n  grant_types: [authorization_code, refresh_token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  code_challenge_methods: [S256]\n  client_id_metadata_document: true\n  source: https://identity.goto.com/.well-known/oauth-authorization-server\npersonal_access_tokens:\n  supported: true\n  docs: https://developer.goto.com/guides/Authentication/03.1_HOW_accessTokenPAT/\n\
  \  note: >-\n    GoTo publishes a guide for obtaining an OAuth access token using a Personal\n    Access Token — the low-friction path for scripts and back-office\n    integrations that do not need a user-consent redirect.\nrefresh_tokens:\n  supported: true\n  docs: https://developer.goto.com/guides/Authentication/05_HOW_refreshToken/\n  note: The token response includes a refresh token; refresh_token is a declared grant type.\nruntime_behaviour:\n  auth_failure_status: 403\n  note: >-\n    No operation in the contract declares 401. Authentication and authorization\n    failures both surface as 403, so token-refresh logic keyed on 401 will never\n    fire against this API.\ngaps:\n- No OpenID Connect discovery document (/.well-known/openid-configuration 404s on every GoTo host) — this is plain OAuth 2.0, no id_token.\n- No RFC 9728 OAuth Protected Resource metadata at the API host (api.getgo.com 404s).\n- No per-operation scopes. The whole API is guarded by one product-level scope, so\
  \ an agent token cannot be least-privileged. See scopes/goto-webinar-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-webinar/refs/heads/main/authentication/goto-webinar-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Webinars
- Virtual Events
- Video Conferencing
- Marketing
- Lead Capture
- Registration
- Webhooks
- Event Management
- Collaboration
- Analytics
---
