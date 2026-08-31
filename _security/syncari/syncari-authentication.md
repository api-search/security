---
api_key_in: []
auth_types: []
description: Syncari runs two independent OAuth 2.0 surfaces. The Syncari Embed REST API uses the client-credentials grant against a token endpoint on the API host itself; the hosted MCP server uses the authorization-code grant with PKCE and RFC 7591 dynamic client registration against an authorization server on app.syncari.com. Both issue Bearer tokens carried in the Authorization header. Derived from Syncari's own documentation plus a live probe of the MCP OAuth metadata - no OpenAPI securitySchemes exist because Syncari publishes no machine-readable contract.
kind: authentication
layout: security
method: searched
name: Syncari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Syncari declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Syncari
provider_slug: syncari
scheme_count: 2
schemes:
- api: Syncari Embed API
  authorization_model:
    additional: Attribute Based Access Control (ABAC) is documented as a platform feature for row/field-level access inside an instance.
    custom_roles: A Role API (GET/POST/PATCH/DELETE /api/v1/roles, plus /api/v1/users/{userId}/roles/{roleId}) was added in the June 2026 release for programmatic management of custom roles and role assignments.
    roles:
    - grants: Manage all instances in the subscription, create new instances and new users.
      name: Org Admin
    - grants: Manage a single Syncari instance. One API user per instance is the documented pattern.
      name: Instance Admin
    style: role and instance scoped, enforced by the API user's assignment
  bearer_format: JWT
  content_type: application/x-www-form-urlencoded
  credential_provisioning:
    docs: https://support.syncari.com/hc/en-us/articles/4417399957908-Set-Up-an-API-User
    notes:
    - An API user cannot log in to the Syncari web app and receives no invitation email.
    - An existing interactive user cannot be converted into an API user.
    - Client ID and client secret are shown once at creation and cannot be retrieved afterwards.
    - Rotation is delete-and-recreate the API user; there is no documented key-rotation endpoint.
    where: Syncari app, Settings > Users > Invite User, with the "API Access" checkbox ticked
  credential_transport: query parameters (grant_type, client_id, client_secret)
  flow: clientCredentials
  id: syncari_embed_oauth2_client_credentials
  refresh:
    endpoint: https://api.syncari.com/api/v1/oauth/token
    grant_type: refresh_token
    note: The client-credentials response also returns a refresh_token, which is unusual for that grant. Syncari documents exchanging it at the same endpoint with grant_type=refresh_token plus client_id and client_secret.
    supported: true
  request_header: 'Authorization: Bearer <access_token>'
  response_fields:
  - access_token
  - refresh_token
  - token_type
  - expires_in
  scopes_documented: false
  token_endpoint: https://api.syncari.com/api/v1/oauth/token
  token_endpoint_method: POST
  token_lifetime_note: Tokens remain active for three hours; after three hours the token must be refreshed.
  token_lifetime_seconds: 10800
  token_type: Bearer
  type: oauth2
- api: Syncari MCP Server
  authorization_endpoint: https://app.syncari.com/arcade/api/v1/oauth2/authorize
  bearer_methods_supported:
  - header
  challenge: 'An unauthenticated POST to https://mcp.syncari.com/mcp returns 401 with WWW-Authenticate: Bearer error="invalid_token", resource_metadata="https://mcp.syncari.com/.well-known/oauth-protected-resource" - a correct RFC 9728 implementation.'
  consent: Syncari's Claude setup documentation shows a "Syncari MCP Authorization Request" screen listing the permissions being requested, so a consent surface exists even though no scope names are published.
  dynamic_client_registration: true
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id: syncari_mcp_oauth2_authorization_code
  issuer: https://mcp.syncari.com
  method: probed
  pkce_methods:
  - plain
  - S256
  registration_endpoint: https://app.syncari.com/arcade/api/v1/oauth2/register
  response_modes:
  - query
  response_types:
  - code
  scopes_supported: []
  source: https://mcp.syncari.com/.well-known/oauth-authorization-server
  token_endpoint: https://app.syncari.com/arcade/api/v1/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: syncari-authentication
source_filename: syncari-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://support.syncari.com/hc/en-us/articles/18707594686100-Authenticating-with-Syncari-Embed-APIs\nname: Syncari authentication profile\ndescription: >-\n  Syncari runs two independent OAuth 2.0 surfaces. The Syncari Embed REST API uses the client-credentials grant\n  against a token endpoint on the API host itself; the hosted MCP server uses the authorization-code grant with\n  PKCE and RFC 7591 dynamic client registration against an authorization server on app.syncari.com. Both issue\n  Bearer tokens carried in the Authorization header. Derived from Syncari's own documentation plus a live probe of\n  the MCP OAuth metadata - no OpenAPI securitySchemes exist because Syncari publishes no machine-readable contract.\ndocs:\n- https://support.syncari.com/hc/en-us/articles/18707594686100-Authenticating-with-Syncari-Embed-APIs\n- https://support.syncari.com/hc/en-us/articles/4417399957908-Set-Up-an-API-User\n- https://support.syncari.com/hc/en-us/articles/18707238885780-Using-the-Syncari-Embed-APIs\n\
  schemes:\n- id: syncari_embed_oauth2_client_credentials\n  api: Syncari Embed API\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://api.syncari.com/api/v1/oauth/token\n  token_endpoint_method: POST\n  content_type: application/x-www-form-urlencoded\n  credential_transport: query parameters (grant_type, client_id, client_secret)\n  bearer_format: JWT\n  token_type: Bearer\n  token_lifetime_seconds: 10800\n  token_lifetime_note: Tokens remain active for three hours; after three hours the token must be refreshed.\n  refresh:\n    supported: true\n    grant_type: refresh_token\n    endpoint: https://api.syncari.com/api/v1/oauth/token\n    note: >-\n      The client-credentials response also returns a refresh_token, which is unusual for that grant. Syncari\n      documents exchanging it at the same endpoint with grant_type=refresh_token plus client_id and client_secret.\n  response_fields: [access_token, refresh_token, token_type, expires_in]\n  request_header: 'Authorization:\
  \ Bearer <access_token>'\n  scopes_documented: false\n  credential_provisioning:\n    where: Syncari app, Settings > Users > Invite User, with the \"API Access\" checkbox ticked\n    docs: https://support.syncari.com/hc/en-us/articles/4417399957908-Set-Up-an-API-User\n    notes:\n    - An API user cannot log in to the Syncari web app and receives no invitation email.\n    - An existing interactive user cannot be converted into an API user.\n    - Client ID and client secret are shown once at creation and cannot be retrieved afterwards.\n    - Rotation is delete-and-recreate the API user; there is no documented key-rotation endpoint.\n  authorization_model:\n    style: role and instance scoped, enforced by the API user's assignment\n    roles:\n    - name: Org Admin\n      grants: Manage all instances in the subscription, create new instances and new users.\n    - name: Instance Admin\n      grants: Manage a single Syncari instance. One API user per instance is the documented pattern.\n\
  \    custom_roles: >-\n      A Role API (GET/POST/PATCH/DELETE /api/v1/roles, plus /api/v1/users/{userId}/roles/{roleId}) was added in the\n      June 2026 release for programmatic management of custom roles and role assignments.\n    additional: >-\n      Attribute Based Access Control (ABAC) is documented as a platform feature for row/field-level access inside\n      an instance.\n- id: syncari_mcp_oauth2_authorization_code\n  api: Syncari MCP Server\n  type: oauth2\n  flow: authorizationCode\n  method: probed\n  source: https://mcp.syncari.com/.well-known/oauth-authorization-server\n  issuer: https://mcp.syncari.com\n  authorization_endpoint: https://app.syncari.com/arcade/api/v1/oauth2/authorize\n  token_endpoint: https://app.syncari.com/arcade/api/v1/oauth2/token\n  registration_endpoint: https://app.syncari.com/arcade/api/v1/oauth2/register\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  response_modes: [query]\n  token_endpoint_auth_methods: [client_secret_basic,\
  \ client_secret_post, none]\n  pkce_methods: [plain, S256]\n  dynamic_client_registration: true\n  bearer_methods_supported: [header]\n  scopes_supported: []\n  challenge: >-\n    An unauthenticated POST to https://mcp.syncari.com/mcp returns 401 with\n    WWW-Authenticate: Bearer error=\"invalid_token\", resource_metadata=\"https://mcp.syncari.com/.well-known/oauth-protected-resource\"\n    - a correct RFC 9728 implementation.\n  consent: >-\n    Syncari's Claude setup documentation shows a \"Syncari MCP Authorization Request\" screen listing the permissions\n    being requested, so a consent surface exists even though no scope names are published.\nplatform_connector_auth:\n  note: >-\n    Separate from calling Syncari, the platform authenticates OUT to source systems. The Synapse SDK enumerates the\n    supported outbound auth types, which is the auth vocabulary a custom connector must implement.\n  source: https://support.syncari.com/hc/en-us/articles/25947440030356-Models-Reference-Page\n\
  \  types:\n  - id: UserPasswordToken\n    label: Basic authentication (user, password, security token)\n  - id: UserPassword\n    label: Username and password\n  - id: ApiKey\n    label: API key or single access token\n  - id: Oauth\n    label: OAuth 2.0 with iFrame authorization flow\n  - id: SimpleOAuth\n    label: OAuth 2.0 client credentials, or any scheme whose credentials expire and must be re-requested\n  sso:\n    supported: true\n    docs: https://support.syncari.com/hc/en-us/sections/50437274435732-Single-Sign-On-SSO\n    note: Syncari documents Single Sign-On for interactive users; it is not a path for API access.\ngaps:\n- No published OAuth scope vocabulary for either surface.\n- No mTLS, no OpenID Connect discovery document (mcp.syncari.com/.well-known/openid-configuration returns 404).\n- No documented programmatic credential rotation; secrets are shown once and rotation means recreating the API user.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncari/refs/heads/main/authentication/syncari-authentication.yml
summary_line: 2 schemes
tags:
- company
- master-data-management
- data-unification
- data-integration
- ipaas
- data-quality
- data-governance
- embedded-integration
- MCP
- agent-native
- revops
- data-synchronization
---
