---
api_key_in: []
api_specs:
- filename: aimlapi-api-key-management-api-openapi.yml
  format: yaml
  label: AIMLAPI API Key Management API
  slug: aimlapi-api-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-api-key-management-api-openapi.yml
- filename: aimlapi-assistants-api-openapi.yml
  format: yaml
  label: AIMLAPI Assistants API
  slug: aimlapi-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-assistants-api-openapi.yml
- filename: aimlapi-chat-api-openapi.yml
  format: yaml
  label: AIMLAPI Chat API
  slug: aimlapi-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-chat-api-openapi.yml
- filename: aimlapi-images-api-openapi.yml
  format: yaml
  label: AIMLAPI Images API
  slug: aimlapi-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-images-api-openapi.yml
- filename: aimlapi-models-api-openapi.yml
  format: yaml
  label: AIMLAPI Models API
  slug: aimlapi-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-models-api-openapi.yml
- filename: aimlapi-threads-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads API
  slug: aimlapi-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-api-openapi.yml
- filename: aimlapi-threads-messages-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads > Messages API
  slug: aimlapi-threads-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-messages-api-openapi.yml
- filename: aimlapi-threads-runs-api-openapi.yml
  format: yaml
  label: AIMLAPI Threads > Runs API
  slug: aimlapi-threads-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-threads-runs-api-openapi.yml
- filename: aimlapi-voice-api-openapi.yml
  format: yaml
  label: AIMLAPI Voice API
  slug: aimlapi-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-voice-api-openapi.yml
- filename: aimlapi-wip-completions-api-openapi.yml
  format: yaml
  label: AIMLAPI [WIP] Completions API
  slug: aimlapi-wip-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-wip-completions-api-openapi.yml
- filename: aimlapi-inference-openapi.yml
  format: yaml
  label: AIMLAPI Inference API
  slug: aimlapi-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/openapi/aimlapi-inference-openapi.yml
auth_types:
- http
- oauth2
description: AIMLAPI runs two distinct authentication systems. The REST API is bearer API keys with two privilege classes (regular keys and management keys) and per-key model scopes and spend caps. The remote MCP server additionally supports full OAuth 2.1 with PKCE and dynamic client registration — the only place OAuth appears in the AIMLAPI surface, and it is not available for the REST API.
kind: authentication
layout: security
method: searched
name: Aimlapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: AIMLAPI secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AIMLAPI
provider_slug: aimlapi
scheme_count: 2
schemes:
- applies_to: REST API (https://api.aimlapi.com)
  header: 'Authorization: Bearer <YOUR_AIMLAPI_KEY>'
  key_classes:
  - controls:
      endpoint_permissions: true
      model_scopes: see scopes/aimlapi-scopes.yml
      spend_limit:
        reset: 00:00 UTC
        retention:
        - no_reset
        - day
        - week
        - month
        threshold: USD
    created_in: dashboard (https://aimlapi.com/app/keys) or POST /v1/keys with a management key
    name: API key
    prefix: The first 8 characters of the key are its `prefix`, visible in the dashboard and used as the path parameter on the key-management endpoints.
    purpose: Calling models and inference endpoints from applications and the Playground.
    shown_once: true
  - created_in: dashboard only — cannot be minted through the API
    name: Management key
    note: 'A deliberate privilege split: the credential that can mint credentials is not itself mintable over the wire. A regular key naming another key''s prefix on the reporting endpoints gets a 403.'
    purpose: Creating, listing, updating and deleting regular API keys via the API.
    shown_once: true
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.aimlapi.com/faq/how-can-i-work-with-my-api-keys
  - openapi/aimlapi-inference-openapi.yml
  type: http
- applies_to: remote MCP server (https://mcp.aimlapi.com/mcp)
  discovery:
  - https://mcp.aimlapi.com/.well-known/oauth-protected-resource
  - https://auth.aimlapi.com/mcp-oauth/.well-known/oauth-authorization-server
  dynamic_client_registration: true
  flows:
    authorizationCode:
      authorizationUrl: https://auth.aimlapi.com/mcp-oauth/auth
      pushedAuthorizationRequestUrl: https://auth.aimlapi.com/mcp-oauth/par
      registrationUrl: https://auth.aimlapi.com/mcp-oauth/register
      scopes:
        email: the account email address
        mcp:invoke: permission to invoke MCP tools, billed to the account
        offline_access: refresh tokens for unattended re-authorization
        openid: OpenID Connect subject identity
      tokenUrl: https://auth.aimlapi.com/mcp-oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - implicit
  id_token_signing_alg:
  - RS256
  name: mcpOAuth
  pkce:
    required_methods:
    - S256
  sources:
  - https://docs.aimlapi.com/quickstart/mcp
  - well-known/aimlapi-mcp-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_jwt
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
slug: aimlapi-authentication
source_filename: aimlapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: AIMLAPI\nproviderId: aimlapi\ngenerated: '2026-08-30'\nmethod: searched\nsource: >-\n  https://docs.aimlapi.com/quickstart/supported-sdks,\n  https://docs.aimlapi.com/faq/how-can-i-work-with-my-api-keys,\n  https://docs.aimlapi.com/api-references/service-endpoints/api-key-management,\n  https://docs.aimlapi.com/quickstart/mcp,\n  https://mcp.aimlapi.com/.well-known/oauth-protected-resource — corroborated by\n  live 401 probes of https://api.aimlapi.com and https://mcp.aimlapi.com\ndescription: >-\n  AIMLAPI runs two distinct authentication systems. The REST API is bearer API\n  keys with two privilege classes (regular keys and management keys) and\n  per-key model scopes and spend caps. The remote MCP server additionally\n  supports full OAuth 2.1 with PKCE and dynamic client registration — the only\n  place OAuth appears in the AIMLAPI surface, and it is not available for the\n  REST API.\nsummary:\n\
  \  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  applies_to: REST API (https://api.aimlapi.com)\n  header: 'Authorization: Bearer <YOUR_AIMLAPI_KEY>'\n  key_classes:\n  - name: API key\n    purpose: Calling models and inference endpoints from applications and the Playground.\n    created_in: dashboard (https://aimlapi.com/app/keys) or POST /v1/keys with a management key\n    shown_once: true\n    prefix: >-\n      The first 8 characters of the key are its `prefix`, visible in the\n      dashboard and used as the path parameter on the key-management endpoints.\n    controls:\n      spend_limit:\n        retention:\n        - no_reset\n        - day\n        - week\n        - month\n        threshold: USD\n        reset: 00:00 UTC\n      endpoint_permissions: true\n      model_scopes: see scopes/aimlapi-scopes.yml\n  - name: Management key\n    purpose: Creating, listing, updating and deleting regular API keys via the API.\n    created_in:\
  \ dashboard only — cannot be minted through the API\n    shown_once: true\n    note: >-\n      A deliberate privilege split: the credential that can mint credentials is\n      not itself mintable over the wire. A regular key naming another key's\n      prefix on the reporting endpoints gets a 403.\n  sources:\n  - https://docs.aimlapi.com/faq/how-can-i-work-with-my-api-keys\n  - openapi/aimlapi-inference-openapi.yml\n- name: mcpOAuth\n  type: oauth2\n  applies_to: remote MCP server (https://mcp.aimlapi.com/mcp)\n  flows:\n    authorizationCode:\n      authorizationUrl: https://auth.aimlapi.com/mcp-oauth/auth\n      tokenUrl: https://auth.aimlapi.com/mcp-oauth/token\n      registrationUrl: https://auth.aimlapi.com/mcp-oauth/register\n      pushedAuthorizationRequestUrl: https://auth.aimlapi.com/mcp-oauth/par\n      scopes:\n        openid: OpenID Connect subject identity\n        email: the account email address\n        offline_access: refresh tokens for unattended re-authorization\n \
  \       mcp:invoke: permission to invoke MCP tools, billed to the account\n  pkce:\n    required_methods:\n    - S256\n  dynamic_client_registration: true\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - implicit\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_jwt\n  - client_secret_post\n  - private_key_jwt\n  - none\n  id_token_signing_alg:\n  - RS256\n  discovery:\n  - https://mcp.aimlapi.com/.well-known/oauth-protected-resource\n  - https://auth.aimlapi.com/mcp-oauth/.well-known/oauth-authorization-server\n  sources:\n  - https://docs.aimlapi.com/quickstart/mcp\n  - well-known/aimlapi-mcp-oauth-authorization-server.json\ngaps:\n- >-\n  The published OpenAPI at https://api.aimlapi.com/docs-yaml declares NO\n  components.securitySchemes and NO security requirement on any of its 19\n  operations, even though every one of them requires a bearer key. An agent\n  reading only the contract would not know the API needs authentication at all.\n  The\
  \ bearerAuth scheme recorded here comes from the older per-tag specs in\n  openapi/ and from the prose documentation.\n- >-\n  The OAuth authorization server advertises the `openid` scope and an `id_token`\n  response type but serves no /.well-known/openid-configuration, so an OIDC\n  client cannot discover it by the standard path.\n- >-\n  No mutualTLS, no signed-request scheme, and no IP allowlisting is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimlapi/refs/heads/main/authentication/aimlapi-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Artificial Intelligence
- Machine-Learning
- AI Models
- LLM
- Image-Generation
- Video Generation
- Speech
- Embeddings
- API Gateway
- Developer Tools
---
