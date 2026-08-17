---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Peopleix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peopleix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Peopleix
provider_slug: peopleix
scheme_count: 1
schemes:
- applies_to:
  - https://app.peopleix.com/mcp
  authorization_endpoint: https://app.peopleix.com/oauth/authorize
  claims_supported:
  - sub
  - iss
  - aud
  - exp
  - iat
  - email
  - name
  - org_id
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.1-style authorization code flow with mandatory PKCE, used to obtain a bearer access token for the peopleIX MCP resource. Dynamic client registration (RFC 7591) is supported, which is what lets an MCP client such as Claude or ChatGPT connect without a pre-provisioned client_id.
  flow: authorizationCode
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oauth2_authorization_code
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://app.peopleix.com
  jwks_note: The jwks_uri is advertised but returns 307 to the app shell for an anonymous client.
  jwks_uri: https://app.peopleix.com/.well-known/jwks.json
  registration_endpoint: https://app.peopleix.com/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://clerk.peopleix.com/oauth/token/revoke
  scopes_supported:
  - openid
  - offline_access
  subject_types_supported:
  - public
  token_endpoint: https://app.peopleix.com/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: peopleix-authentication
source_filename: peopleix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://app.peopleix.com/.well-known/oauth-authorization-server and https://app.peopleix.com/.well-known/oauth-protected-resource/mcp\nnote: >-\n  peopleIX publishes no OpenAPI and no human-readable authentication documentation,\n  so this profile is derived entirely from the machine-readable OAuth metadata the\n  application host serves anonymously. It describes how a client authenticates to the\n  peopleIX MCP resource at https://app.peopleix.com/mcp. The identity layer is Clerk\n  (revocation endpoint on clerk.peopleix.com, service_documentation on clerk.com).\nschemes:\n- id: oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    OAuth 2.1-style authorization code flow with mandatory PKCE, used to obtain a\n    bearer access token for the peopleIX MCP resource. Dynamic client registration\n    (RFC 7591) is supported, which is what lets an MCP client such as Claude or\n    ChatGPT connect\
  \ without a pre-provisioned client_id.\n  issuer: https://app.peopleix.com\n  authorization_endpoint: https://app.peopleix.com/oauth/authorize\n  token_endpoint: https://app.peopleix.com/oauth/token\n  registration_endpoint: https://app.peopleix.com/oauth/register\n  revocation_endpoint: https://clerk.peopleix.com/oauth/token/revoke\n  jwks_uri: https://app.peopleix.com/.well-known/jwks.json\n  jwks_note: The jwks_uri is advertised but returns 307 to the app shell for an anonymous client.\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  code_challenge_methods_supported:\n  - S256\n  scopes_supported:\n  - openid\n  - offline_access\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  claims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - email\n  - name\n  - org_id\n  applies_to:\n\
  \  - https://app.peopleix.com/mcp\nprotected_resources:\n- resource: https://app.peopleix.com/mcp\n  resource_name: peopleIX MCP\n  authorization_servers:\n  - https://app.peopleix.com\n  token_types_supported:\n  - urn:ietf:params:oauth:token-type:access_token\n  token_introspection_endpoint: https://app.peopleix.com/oauth/token\n  authorization_data_locations_supported:\n  - header\n  - body\n  scopes_supported: []\nchallenge:\n  status: 401\n  header: >-\n    WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"No authorization\n    provided\", resource_metadata=\"https://app.peopleix.com/.well-known/oauth-protected-resource/mcp\"\n  spec: RFC 9728\n  note: >-\n    The 401 carries a machine-readable pointer to its own resource metadata, which is\n    the discovery path an MCP client is expected to follow. This is the strongest\n    agent-facing auth signal peopleIX publishes.\nhuman_auth:\n  sign_in: https://app.peopleix.com/en/auth/sign-in\n  note: End-user sign-in\
  \ to the peopleIX application; distinct from the OAuth client flow above.\ngaps:\n- No published authentication documentation page for developers.\n- No API keys, no service-account credential, and no documented machine-to-machine grant (client_credentials is not in grant_types_supported).\n- The MCP resource advertises an empty scopes_supported array, so no least-privilege scoping is exposed to a connecting agent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleix/refs/heads/main/authentication/peopleix-authentication.yml
summary_line: 1 scheme
tags:
- Company
- HR
- People Analytics
- People Intelligence
- Conversation Intelligence
- Human Resources
- Workforce Analytics
- AI
- MCP
- Germany
---
