---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Motion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Motion declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Motion
provider_slug: motion
scheme_count: 0
schemes: []
slug: motion-authentication
source_filename: motion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://help.motionapp.com/en/articles/14315735-motion-mcp\nprobe_source: https://projects.motionapp.com/.well-known/oauth-authorization-server\ndocs: https://help.motionapp.com/en/articles/14315735-motion-mcp\nname: Motion — authentication profile\nnote: >-\n  Motion publishes no OpenAPI, so this profile is not derived from a spec. It is read from Motion's\n  own RFC 8414 authorization-server metadata (fetched live, HTTP 200) plus the Motion MCP help-centre\n  article. Motion ships exactly one machine-callable surface — the Motion MCP server at\n  https://projects.motionapp.com/mcp — and it is OAuth 2.0 only. There is no API key, no personal\n  access token, and no basic-auth path published anywhere on Motion's public surface.\nsurfaces:\n- surface: Motion MCP\n  url: https://projects.motionapp.com/mcp\n  scheme: oauth2\n  gated: true\n  observed_challenge:\n    http_status: 401\n    www_authenticate: Bearer resource_metadata=\"\
  https://projects.motionapp.com/mcp/.well-known/oauth-protected-resource\"\n    body: '{\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Missing or invalid Authorization header\"},\"id\":null}'\nsecurity_schemes:\n- name: motion_oauth2\n  type: oauth2\n  bearer_methods_supported:\n  - header\n  issuer: https://projects.motionapp.com/api/auth\n  flows:\n  - flow: authorizationCode\n    authorization_url: https://projects.motionapp.com/api/auth/oauth2/authorize\n    token_url: https://projects.motionapp.com/api/auth/oauth2/token\n    refresh_url: https://projects.motionapp.com/api/auth/oauth2/token\n    pkce_required_methods:\n    - S256\n  - flow: clientCredentials\n    token_url: https://projects.motionapp.com/api/auth/oauth2/token\n  - flow: refreshToken\n    token_url: https://projects.motionapp.com/api/auth/oauth2/token\nendpoints:\n  authorization: https://projects.motionapp.com/api/auth/oauth2/authorize\n  token: https://projects.motionapp.com/api/auth/oauth2/token\n  registration:\
  \ https://projects.motionapp.com/api/auth/oauth2/register\n  introspection: https://projects.motionapp.com/api/auth/oauth2/introspect\n  revocation: https://projects.motionapp.com/api/auth/oauth2/revoke\n  userinfo: https://projects.motionapp.com/api/auth/oauth2/userinfo\n  end_session: https://projects.motionapp.com/api/auth/oauth2/end-session\n  jwks: https://projects.motionapp.com/api/auth/jwks\n  discovery:\n  - https://projects.motionapp.com/.well-known/oauth-authorization-server\n  - https://projects.motionapp.com/api/auth/.well-known/openid-configuration\n  protected_resource_metadata: https://projects.motionapp.com/mcp/.well-known/oauth-protected-resource\ncapabilities:\n  dynamic_client_registration: true\n  dynamic_client_registration_note: >-\n    RFC 7591 registration_endpoint is advertised and token_endpoint_auth_methods_supported includes\n    \"none\", which is what lets an MCP client register itself and run a public-client PKCE flow with\n    no pre-provisioned credentials.\
  \ This is why Claude/ChatGPT/Cursor can connect with nothing but\n    the server URL.\n  pkce: true\n  pkce_methods:\n  - S256\n  response_types_supported:\n  - code\n  response_modes_supported:\n  - query\n  grant_types_supported:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  introspection_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  revocation_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - EdDSA\n  subject_types_supported:\n  - public\n  authorization_response_iss_parameter_supported: true\n  acr_values_supported:\n  - urn:mace:incommon:iap:bronze\n  prompt_values_supported:\n  - login\n  - consent\n  - create\n  - select_account\n  - none\n  claims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - sid\n  - scope\n  - azp\n  - email\n\
  \  - email_verified\n  - name\n  - picture\n  - family_name\n  - given_name\nauthorization_model:\n  per_user: true\n  note: >-\n    Authorization is the user's own Motion account authorization — the token carries exactly the\n    workspaces and organizations that user can already see in the app. There is no separate\n    machine/service identity documented for the MCP surface even though client_credentials is\n    advertised by the authorization server.\n  roles_permitted:\n  - Owner\n  - Admin\n  - Collaborator\n  roles_denied:\n  - Guest access\n  - Partner share access\n  credential_handling: >-\n    Provider states the AI client never receives or stores Motion credentials, and that access can be\n    revoked at any time by disconnecting the MCP from the client's settings.\nnot_published:\n- API keys or personal access tokens\n- HTTP basic authentication\n- mutual TLS\n- an OpenAPI securitySchemes block (Motion publishes no OpenAPI)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motion/refs/heads/main/authentication/motion-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Creative Analytics
- Advertising
- Marketing Analytics
- Performance Marketing
- Ad Reporting
- Creative Strategy
- Software-as-a-Service
- MCP
- Agent Surface
---
