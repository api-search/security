---
api_key_in: []
api_specs:
- filename: graphql-api
  format: yaml
  label: The Brief Public GraphQL API
  slug: the-brief-public-graphql-api
  spec_type: Postman
  url: https://www.postman.com/thebrieftechnical/the-brief-api/collection/1lfct1g/graphql-api
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Thebrief Authentication
name_suffix: Authentication
oauth_flows: []
overview: TheBrief declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: TheBrief
provider_slug: thebrief
scheme_count: 3
schemes:
- applies_to: https://api.thebrief.ai/v1
  bearerFormat: JWT
  header: Authorization
  id: rest_bearer_jwt
  note: 'POST the clientId/clientSecret pair to /v1/auth/token and the API returns {"token": "<jwt>"} to send as Authorization: Bearer on every subsequent request.'
  scheme: bearer
  token_endpoint: https://api.thebrief.ai/v1/auth/token
  token_endpoint_method: POST
  token_request_body:
  - name: clientId
    required: true
    type: string
  - name: clientSecret
    required: true
    type: string
  token_response_field: token
  type: http
  value_format: Bearer <jwt>
- applies_to: https://graphql.thebrief.ai/public
  bearerFormat: JWT
  header: Authorization
  id: graphql_bearer_jwt
  note: The GraphQL endpoint accepts the same bearer token. Anonymous __schema introspection IS permitted (verified 2026-08-12, HTTP 200) but executing queries/mutations is not.
  scheme: bearer
  type: http
- claims:
  - description: The public clientId from API credentials.
    name: clientId
    required: true
  - description: Issued-at timestamp.
    name: iat
    required: false
  - description: App Integration only — the team user to impersonate for the session.
    name: userId
    required: false
  - create_blank_design: null
    description: App Integration only — the session action (create_design_from_template
    edit_design: null
    get_share_link).: null
    name: action
    required: false
  - description: App Integration only — UI configuration for the session.
    name: sessionConfig
    required: false
  id: self_signed_jwt
  note: Clients may sign their own JWT with the secret rather than calling /v1/auth/token. The App Integration (embedded editor) flow REQUIRES this form — the signed token is handed to https://app.thebrief.ai/tokenAuth?token=<jwt> (or app-proxy.thebrief.ai in an iframe) to open an impersonated editor session.
  signing: HS256 (jsonwebtoken sign with the clientSecret)
  source: https://docs.thebrief.ai/app-integration
  type: jwt
slug: thebrief-authentication
source_filename: thebrief-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://docs.thebrief.ai/public-api/authentication\ndocs:\n  - https://docs.thebrief.ai/public-api/authentication\n  - https://docs.thebrief.ai/public-api/rest-api/auth\n  - https://docs.thebrief.ai/public-api\n  - https://docs.thebrief.ai/app-integration\nsummary: >-\n  The Brief Public API (REST at https://api.thebrief.ai/v1 and GraphQL at\n  https://graphql.thebrief.ai/public) authenticates with a JWT bearer token minted from a\n  clientId / clientSecret pair the team creates in the app under Manage account >\n  API credentials. There is no OAuth 2.0 authorization server, no OpenID Connect\n  discovery document and no mTLS surface; token scopes are carried in the token, not\n  negotiated. The same clientId/secret pair also signs the session JWT used by the\n  App Integration (embedded editor) flow.\n\ncredential_issuance:\n  console_url: https://app.thebrief.ai/go-to/settings/api-credentials\n  path_in_app: Profile > Manage\
  \ account > API credentials\n  credential_pair:\n    - {name: clientId, type: uuid, role: public identifier}\n    - {name: clientSecret, type: uuid, role: signing secret, note: Kept private; never shared client-side.}\n  revocation:\n    supported: true\n    note: >-\n      The docs warn that deleting an API key blocks every already-configured integration\n      from accessing The Brief — deletion is the documented revocation mechanism.\n    source: https://docs.thebrief.ai/zapier-integration\n\nschemes:\n  - id: rest_bearer_jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    header: Authorization\n    value_format: 'Bearer <jwt>'\n    applies_to: https://api.thebrief.ai/v1\n    token_endpoint: https://api.thebrief.ai/v1/auth/token\n    token_endpoint_method: POST\n    token_request_body:\n      - {name: clientId, required: true, type: string}\n      - {name: clientSecret, required: true, type: string}\n    token_response_field: token\n    note: >-\n      POST the clientId/clientSecret\
  \ pair to /v1/auth/token and the API returns\n      {\"token\": \"<jwt>\"} to send as Authorization: Bearer on every subsequent request.\n\n  - id: graphql_bearer_jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    header: Authorization\n    applies_to: https://graphql.thebrief.ai/public\n    note: >-\n      The GraphQL endpoint accepts the same bearer token. Anonymous __schema introspection\n      IS permitted (verified 2026-08-12, HTTP 200) but executing queries/mutations is not.\n\n  - id: self_signed_jwt\n    type: jwt\n    signing: HS256 (jsonwebtoken sign with the clientSecret)\n    claims:\n      - {name: clientId, required: true, description: The public clientId from API credentials.}\n      - {name: iat, required: false, description: Issued-at timestamp.}\n      - {name: userId, required: false, description: App Integration only — the team user to impersonate for the session.}\n      - {name: action, required: false, description: App Integration only — the session\
  \ action (create_design_from_template, create_blank_design, edit_design, get_share_link).}\n      - {name: sessionConfig, required: false, description: App Integration only — UI configuration for the session.}\n    note: >-\n      Clients may sign their own JWT with the secret rather than calling /v1/auth/token.\n      The App Integration (embedded editor) flow REQUIRES this form — the signed token is\n      handed to https://app.thebrief.ai/tokenAuth?token=<jwt> (or app-proxy.thebrief.ai in\n      an iframe) to open an impersonated editor session.\n    source: https://docs.thebrief.ai/app-integration\n\ntoken_scopes:\n  model: api-token-scope\n  note: >-\n    Not OAuth 2.0 scopes. The public GraphQL schema publishes an ApiTokenScope enum naming\n    the surfaces an API token may be issued against; this is the only scope vocabulary The\n    Brief exposes, and it is captured verbatim from the live introspection response.\n  source: graphql/thebrief-public.graphql (enum ApiTokenScope)\n\
  \  scopes:\n    - {name: CREATOPY_API, description: Access to Creatopy API}\n    - {name: FIGMA, description: Access to Figma plugin}\n    - {name: ZAPIER, description: Access to Zapier integration}\n\nauthorization:\n  model: team-scoped\n  admin_gated_operations:\n    note: >-\n      The GraphQL schema marks a set of team-administration fields as requiring admin access\n      in their own descriptions (teamUsers, createTeamUser, deleteTeamUser, updateTeamUserRole).\n      The InputAuthorization input type carries needAdmin and requiredScopes, confirming the\n      server evaluates both an admin flag and a scope list per request.\n    fields: [teamUsers, createTeamUser, deleteTeamUser, updateTeamUserRole]\n  impersonation:\n    supported: true\n    note: >-\n      A clientId/secret pair generated by a team owner or admin may impersonate any user on\n      that team by putting their userId in the App Integration session JWT.\n\nnot_present:\n  oauth2: {documented: false, note: No OAuth\
  \ 2.0 authorization-code/client-credentials flow is documented.}\n  openid_connect: {documented: false, probe: 'https://www.thebrief.ai/.well-known/openid-configuration -> 404 (also 404 on api., docs.)'}\n  oauth_authorization_server_metadata: {documented: false, probe: 'https://api.thebrief.ai/.well-known/oauth-authorization-server -> 404'}\n  mutual_tls: {documented: false}\n  api_key_header: {documented: false, note: The \"API key\" named in the UI is the clientId/clientSecret pair, exchanged for a JWT — not a raw key header.}\n\ncross_links:\n  conventions: conventions/thebrief-conventions.yml\n  errors: errors/thebrief-error-codes.yml\n  rate_limits: rate-limits/thebrief-rate-limits.yml\n  graphql: graphql/thebrief-public.graphql\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thebrief/refs/heads/main/authentication/thebrief-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Advertising
- Creative
- Design
- Artificial Intelligence
- Marketing
- Ad Serving
- Software-as-a-Service
- GraphQL
- Creative Automation
- Digital Asset Management
- Webhook
---
