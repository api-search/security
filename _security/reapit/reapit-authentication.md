---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: 'Every Foundations surface — REST, GraphQL, webhooks management, notifications and MCP — is fronted by one hosted identity service, Reapit Connect, an Auth0-backed OpenID Connect tenant at connect.reapit.cloud. Two grants are supported: authorization code (user context, PKCE S256) and client credentials (machine-to-machine). The auth model has three quirks worth knowing before writing code: client-credentials callers MUST send a reapit-customer tenant header, the GraphQL proxy requires BOTH the idToken and the accessToken in two different headers (which excludes client-credentials clients entirely), and the MCP server additionally requires the agencyCloud/mcp.access scope on the token.'
kind: authentication
layout: security
method: searched
name: Reapit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Reapit secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Reapit
provider_slug: reapit
scheme_count: 3
schemes:
- audience: user-context web and client-side applications
  authorizationUrl: https://connect.reapit.cloud/authorize
  code_challenge_methods:
  - S256
  - plain
  flow: authorizationCode
  name: ReapitConnectAuthorizationCode
  note: The only grant that works against the GraphQL proxy, because GraphQL needs an idToken as well as an accessToken.
  pkce: true
  sdk: '@reapit/connect-session (browser), @reapit/connect-session-server (Node)'
  tokenUrl: https://connect.reapit.cloud/oauth/token
  type: oauth2
- audience: server-side machine-to-machine applications with no user in context
  client_auth: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'
  content_type: application/x-www-form-urlencoded
  extra_header:
    description: the customer's unique id, or SBOX for the sandbox
    name: reapit-customer
    required: true
  flow: clientCredentials
  name: ReapitConnectClientCredentials
  request_params:
  - client_id
  - grant_type=client_credentials
  tokenUrl: https://connect.reapit.cloud/oauth/token
  type: oauth2
  warning: Reapit explicitly forbids using this grant from client-side-only apps; a server-side component is required to store the secret safely.
- bearerFormat: JWT
  description: 'How the issued access token is presented: Authorization: Bearer <token>'
  name: BearerToken
  scheme: bearer
  type: http
slug: reapit-authentication
source_filename: reapit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://foundations-documentation.reapit.cloud/api/reapit-connect ,\n  https://foundations-documentation.reapit.cloud/api/api-documentation#authentication\n  , and the live discovery document at\n  https://connect.reapit.cloud/.well-known/openid-configuration (HTTP 200,\n  fetched 2026-07-26)\ndocs: https://foundations-documentation.reapit.cloud/api/reapit-connect\ndescription: >-\n  Every Foundations surface — REST, GraphQL, webhooks management, notifications\n  and MCP — is fronted by one hosted identity service, Reapit Connect, an\n  Auth0-backed OpenID Connect tenant at connect.reapit.cloud. Two grants are\n  supported: authorization code (user context, PKCE S256) and client credentials\n  (machine-to-machine). The auth model has three quirks worth knowing before\n  writing code: client-credentials callers MUST send a reapit-customer tenant\n  header, the GraphQL proxy requires BOTH the idToken and the accessToken\
  \ in two\n  different headers (which excludes client-credentials clients entirely), and\n  the MCP server additionally requires the agencyCloud/mcp.access scope on the\n  token.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials]\n  token_type: Bearer (JWT)\n  token_lifetime_seconds: 3600\n  refresh: supported via offline_access / refresh_token grant\n  mtls: false\nissuer:\n  name: Reapit Connect\n  issuer: https://connect.reapit.cloud/\n  backing_provider: Auth0\n  discovery: https://connect.reapit.cloud/.well-known/openid-configuration\n  discovery_file: well-known/reapit-openid-configuration.json\n  oauth_metadata: https://connect.reapit.cloud/.well-known/oauth-authorization-server\n  oauth_metadata_file: well-known/reapit-oauth-authorization-server.json\n  jwks_uri: https://connect.reapit.cloud/.well-known/jwks.json\n  jwks_file: well-known/reapit-connect-jwks.json\nendpoints:\n  authorization: https://connect.reapit.cloud/authorize\n\
  \  token: https://connect.reapit.cloud/oauth/token\n  token_documented_alias: https://connect.reapit.cloud/token\n  userinfo: https://connect.reapit.cloud/userinfo\n  device_authorization: https://connect.reapit.cloud/oauth/device/code\n  backchannel_authentication: https://connect.reapit.cloud/bc-authorize\n  registration: https://connect.reapit.cloud/oidc/register\n  revocation: https://connect.reapit.cloud/oauth/revoke\n  end_session: https://connect.reapit.cloud/oidc/logout\n  mfa_challenge: https://connect.reapit.cloud/mfa/challenge\n  global_token_revocation: https://connect.reapit.cloud/oauth/global-token-revocation/connection/{connectionName}\nschemes:\n- name: ReapitConnectAuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  code_challenge_methods: [S256, plain]\n  authorizationUrl: https://connect.reapit.cloud/authorize\n  tokenUrl: https://connect.reapit.cloud/oauth/token\n  audience: user-context web and client-side applications\n  sdk: \"@reapit/connect-session\
  \ (browser), @reapit/connect-session-server (Node)\"\n  note: >-\n    The only grant that works against the GraphQL proxy, because GraphQL needs\n    an idToken as well as an accessToken.\n- name: ReapitConnectClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://connect.reapit.cloud/oauth/token\n  client_auth: 'HTTP Basic — Authorization: Basic base64(client_id:client_secret)'\n  content_type: application/x-www-form-urlencoded\n  request_params: [client_id, grant_type=client_credentials]\n  audience: server-side machine-to-machine applications with no user in context\n  warning: >-\n    Reapit explicitly forbids using this grant from client-side-only apps; a\n    server-side component is required to store the secret safely.\n  extra_header:\n    name: reapit-customer\n    required: true\n    description: the customer's unique id, or SBOX for the sandbox\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'How the issued\
  \ access token is presented: Authorization: Bearer <token>'\nsupported_grant_types:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\n- http://auth0.com/oauth/grant-type/password-realm\n- http://auth0.com/oauth/grant-type/passwordless/otp\n- http://auth0.com/oauth/grant-type/mfa-oob\n- http://auth0.com/oauth/grant-type/mfa-otp\n- http://auth0.com/oauth/grant-type/mfa-recovery-code\nsupported_grant_types_note: >-\n  This is the raw Auth0 tenant capability from the discovery document. Reapit\n  documents only authorization_code and client_credentials as supported for\n  Foundations applications; do not build against the others.\ntoken_endpoint_auth_methods: [client_secret_basic, client_secret_post, private_key_jwt,\n  none]\nid_token_signing_algs: [HS256, RS256, PS256]\ndpop_signing_algs: [ES256]\ncapabilities:\n\
  \  pkce: true\n  dynamic_client_registration: true\n  device_authorization: true\n  backchannel_authentication: true\n  backchannel_logout: true\n  token_revocation: true\n  mfa: true\n  request_parameter_supported: false\n  request_uri_parameter_supported: false\nper_surface:\n- surface: Foundations REST API\n  base_url: https://platform.reapit.cloud\n  headers:\n    Authorization: Bearer <access token>\n    reapit-customer: required for client-credentials callers (SBOX for sandbox)\n    api-version: '2020-01-31 (required)'\n- surface: Foundations GraphQL proxy\n  base_url: https://graphql.reapit.cloud/graphql\n  headers:\n    authorization: the Reapit Connect idToken\n    reapit-connect-token: the Reapit Connect accessToken\n  constraint: >-\n    Requires BOTH tokens, so only the authorization-code flow works —\n    client-credentials machine-to-machine clients cannot use GraphQL at all.\n  note: >-\n    Schema INTROSPECTION is anonymous (verified 2026-07-26); only execution is\n   \
  \ gated.\n- surface: Foundations MCP server (alpha)\n  base_url: https://foundations-mcp.iaas.reapit.cloud/mcp\n  headers:\n    Authorization: Bearer <Reapit Connect JWT>\n    reapit-customer: machine-to-machine clients only\n    x-timezone: optional, default UTC\n  required_scope: agencyCloud/mcp.access\n  failure: 403 when the scope is absent\n- surface: Foundations Webhooks (inbound to your endpoint)\n  direction: Reapit -> you\n  verification: Ed25519 signature in the X-Signature header (s:keyId:timestamp:signature)\n  public_key: GET https://platform.reapit.cloud/webhooks/signing/{id} (bearer required)\n- surface: Reapit IaaS CLI\n  mechanism: API key created on the pipelines page of the developer portal\n  command: reapit config\nauthorization_model:\n  registration: submit the app to the AppMarket to be issued a client id and secret\n  portal: https://marketplace.reapit.cloud/developer/apps\n  install: >-\n    A customer administrator installs the listed app and grants the permissions\n\
  \    (scopes) it requested; access is revoked on uninstall.\n  scopes: scopes/reapit-scopes.yml\n  identifier_caveat: >-\n    Resource ids are unique only within one customer database — build a\n    composite key of customerId + resource id.\ntroubleshooting:\n- https://foundations-documentation.reapit.cloud/troubleshooting/authentication-issues\n- https://foundations-documentation.reapit.cloud/troubleshooting/reapit-connect\n- https://foundations-documentation.reapit.cloud/troubleshooting/accessing-customer-data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reapit/refs/heads/main/authentication/reapit-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Real Estate
- United Kingdom
- PropTech
- CRM
- Estate Agents
- Property Listings
- Property Management
- Rentals
- Conveyancing
- Australia
---
