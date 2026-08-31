---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Kakao Entertainment Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kakao Entertainment declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kakao Entertainment
provider_slug: kakao-entertainment
scheme_count: 1
schemes:
- applies_to:
  - https://mcp.melon.com/mcp
  authorization_endpoint: https://cola.melon.com/auth/v3/oauth/authorize
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  introspection_endpoint: https://cola.melon.com/auth/v3/oauth/introspect
  name: melon_oauth2
  pkce:
    code_challenge_methods_supported:
    - S256
    required_by_metadata: true
  registration_endpoint: https://cola.melon.com/auth/v3/oauth/register
  response_types_supported:
  - code
  revocation_endpoint: https://cola.melon.com/auth/v3/oauth/revoke
  scopes: scopes/kakao-entertainment-scopes.yml
  token_endpoint: https://cola.melon.com/auth/v3/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: kakao-entertainment-authentication
source_filename: kakao-entertainment-authentication.yml
source_heading: Authentication Profile
source_url: https://cola.melon.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://cola.melon.com/auth/v3/oauth/docs\nsources:\n- https://cola.melon.com/.well-known/oauth-authorization-server\n- https://cola.melon.com/auth/v3/oauth/docs\n- https://cola.melon.com/auth/v3/oauth/docs/dynamic-client-registration\n- https://tech.kakaoent.com/ai/using-melon-mcp-server-en/\nnote: >-\n  Kakao Entertainment publishes no OpenAPI, so this profile is not derived from securitySchemes. It is\n  read from the provider's own RFC 8414 authorization server metadata document and from the Melon\n  Alliance Auth v3 documentation pages, both fetched anonymously on 2026-08-23. Melon Alliance Auth v3\n  describes itself as \"a standards-compliant authorization platform that implements OAuth 2.0 and\n  OAuth 2.1 (draft)\".\nplatform:\n  name: Melon Alliance Auth v3\n  issuer: https://cola.melon.com\n  documentation: https://cola.melon.com/auth/v3/oauth/docs\nschemes:\n- name: melon_oauth2\n  type: oauth2\n  flow: authorization_code\n\
  \  pkce:\n    required_by_metadata: true\n    code_challenge_methods_supported:\n    - S256\n  authorization_endpoint: https://cola.melon.com/auth/v3/oauth/authorize\n  token_endpoint: https://cola.melon.com/auth/v3/oauth/token\n  introspection_endpoint: https://cola.melon.com/auth/v3/oauth/introspect\n  revocation_endpoint: https://cola.melon.com/auth/v3/oauth/revoke\n  registration_endpoint: https://cola.melon.com/auth/v3/oauth/register\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  scopes: scopes/kakao-entertainment-scopes.yml\n  applies_to:\n  - https://mcp.melon.com/mcp\ndynamic_client_registration:\n  supported: true\n  spec: RFC 7591\n  endpoint: https://cola.melon.com/auth/v3/oauth/register\n  auth_methods_supported:\n  - none\n  documentation: https://cola.melon.com/auth/v3/oauth/docs/dynamic-client-registration\n  request_fields:\n\
  \  - name: client_name\n    type: string\n    required: true\n    constraint: max 50 characters\n  - name: redirect_uris\n    type: string[]\n    required: true\n    constraint: max 5 URIs, each 300 characters or fewer\n  response_fields:\n  - client_id\n  - client_secret\n  - client_id_issued_at\n  - client_secret_expires_at\n  - client_name\n  - redirect_uris\n  - grant_types\n  - response_types\n  - token_endpoint_auth_method\n  defaults:\n    grant_types:\n    - authorization_code\n    - refresh_token\n    response_types:\n    - code\n    token_endpoint_auth_method: client_secret_basic\n    client_secret_expires_at: 0\n  constraint: >-\n    Registration is not open self-service. The provider states only redirect URIs allowlisted per\n    partner are accepted and that malformed or disallowed redirect URIs are rejected; the MCP\n    integration guide directs partners to melon_info@kakaoent.com to have their information registered\n    before use.\nsecurity_considerations_published:\n\
  - client_secret must be kept confidential and never exposed to browser or frontend clients.\n- Only per-partner allowlisted redirect URIs are accepted.\n- All transport is HTTPS; the provider states authentication tokens are not stored on the MCP server.\n- Provider recommends explicit user confirmation for critical actions and input sanitisation against\n  prompt injection when building agent workflows.\nui_locales_supported:\n- ko\nx-evidence:\n  fetched: '2026-08-23'\n  metadata_url: https://cola.melon.com/.well-known/oauth-authorization-server\n  metadata_status: 200\n  docs_url: https://cola.melon.com/auth/v3/oauth/docs\n  docs_status: 200\n  dcr_docs_url: https://cola.melon.com/auth/v3/oauth/docs/dynamic-client-registration\n  dcr_docs_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kakao-entertainment/refs/heads/main/authentication/kakao-entertainment-authentication.yml
summary_line: 1 scheme
tags:
- Entertainment
- Music
- Streaming
- Webtoons
- Publishing
- Media
- MCP
- Agents
- South Korea
- Company
---
