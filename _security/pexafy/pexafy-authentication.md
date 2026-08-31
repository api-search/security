---
api_key_in:
- header
api_specs:
- filename: pexafy-collections-api-openapi.yml
  format: yaml
  label: Pexafy Collections API
  slug: pexafy-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-collections-api-openapi.yml
- filename: pexafy-facets-api-openapi.yml
  format: yaml
  label: Pexafy Facets API
  slug: pexafy-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-facets-api-openapi.yml
- filename: pexafy-photos-api-openapi.yml
  format: yaml
  label: Pexafy Photos API
  slug: pexafy-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-photos-api-openapi.yml
- filename: pexafy-search-api-openapi.yml
  format: yaml
  label: Pexafy Search API
  slug: pexafy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-search-api-openapi.yml
- filename: pexafy-usage-api-openapi.yml
  format: yaml
  label: Pexafy Usage API
  slug: pexafy-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/openapi/pexafy-usage-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pexafy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pexafy secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pexafy
provider_slug: pexafy
scheme_count: 3
schemes:
- description: 'Pass your Pexafy API key in this header.


    Get your API key at https://pexafy.com/dashboard/api-keys/create/'
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/pexafy-api-openapi.json
  type: apiKey
- description: Send the key as a bearer token. Keys carry scopes; a read-scoped key gets a 403 on anything under /collections.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/pexafy-api-v1-openapi.json
  type: http
- flows:
  - authorizationUrl: https://pexafy.com/oauth/authorize/
    flow: authorizationCode
    pkce: S256
    scopes:
    - read
    - write
    tokenUrl: https://pexafy.com/oauth/token/
  introspection_endpoint: https://pexafy.com/oauth/introspect/
  issuer: https://pexafy.com/
  name: PexafyOAuth
  note: Not declared in either OpenAPI document — discovered from RFC 8414 metadata. It is the credential model for the MCP server (mcp.pexafy.com), which advertises it via RFC 9728 protected-resource metadata and a WWW-Authenticate challenge on an unauthenticated tools/list.
  registration_endpoint: https://pexafy.com/oauth/register
  revocation_endpoint: https://pexafy.com/oauth/revoke_token/
  sources:
  - https://pexafy.com/.well-known/oauth-authorization-server
  type: oauth2
slug: pexafy-authentication
source_filename: pexafy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/pexafy-api-openapi.json, openapi/pexafy-api-v1-openapi.json\ndocs: https://docs.pexafy.com/quickstart\nadditional_sources:\n- https://pexafy.com/.well-known/api-onboarding\n- https://pexafy.com/.well-known/oauth-authorization-server\n- https://mcp.pexafy.com/.well-known/oauth-protected-resource\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Two surfaces, two credential models. The REST API takes a long-lived API key, sent\n    either as x-api-key or as Authorization: Bearer — the two OpenAPI documents each\n    declare only one of those, but the provider's own api-onboarding descriptor states\n    both work on the same routes, and the live 401 body confirms it\n    (\"Authentication required (Bearer token or X-Api-Key)\"). The hosted MCP server takes\n    OAuth 2.1 with dynamic client registration and PKCE, or the same API key\
  \ as a bearer\n    token for clients that cannot do OAuth.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: |-\n    Pass your Pexafy API key in this header.\n\n    Get your API key at https://pexafy.com/dashboard/api-keys/create/\n  sources:\n  - openapi/pexafy-api-openapi.json\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: >-\n    Send the key as a bearer token. Keys carry scopes; a read-scoped key gets a 403 on\n    anything under /collections.\n  sources:\n  - openapi/pexafy-api-v1-openapi.json\n- name: PexafyOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://pexafy.com/oauth/authorize/\n    tokenUrl: https://pexafy.com/oauth/token/\n    scopes: [read, write]\n    pkce: S256\n  registration_endpoint: https://pexafy.com/oauth/register\n  revocation_endpoint: https://pexafy.com/oauth/revoke_token/\n  introspection_endpoint: https://pexafy.com/oauth/introspect/\n  issuer: https://pexafy.com/\n\
  \  sources:\n  - https://pexafy.com/.well-known/oauth-authorization-server\n  note: >-\n    Not declared in either OpenAPI document — discovered from RFC 8414 metadata. It is the\n    credential model for the MCP server (mcp.pexafy.com), which advertises it via RFC 9728\n    protected-resource metadata and a WWW-Authenticate challenge on an unauthenticated\n    tools/list.\nkey_lifecycle:\n  issuance: >-\n    Console only. Create an account at https://pexafy.com/signup/, then create a key at\n    https://pexafy.com/dashboard/api-keys/create/. Issued immediately — no application\n    form, no review queue.\n  programmatic_issuance: false\n  one_time_display: true\n  rotation: Create a new key and revoke the old one from https://pexafy.com/dashboard/api-keys/\n  env_var: PEXAFY_API_KEY\n  key_prefix: pexafy_api_\n  keys_per_plan: 1 on Free, 3 Starter, 5 Pro, 10 Expert, 25 Team, unlimited on Business and Enterprise\nunauthenticated_surface:\n- endpoint: GET https://api.pexafy.com/health\n\
  \  status: 200\n  note: Public liveness check — the api-onboarding flow uses it as the pre-flight probe before spending a key.\n- endpoint: GET https://mcp.pexafy.com/health\n  note: Public liveness check for the MCP server, per the pexafy-mcp README.\ngaps:\n- The live /openapi.json declares ApiKeyAuth per-operation on all 20 operations but has no root-level `security` and no 401 response anywhere, so a generated client knows a credential is needed and still has no error shape for a missing one.\n- The two published OpenAPI documents disagree on the scheme name and type (ApiKeyAuth/apiKey-header vs apiKey/http-bearer) for the same credential.\n- OAuth 2.1 is not represented in either OpenAPI document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pexafy/refs/heads/main/authentication/pexafy-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Image
- Photos
- Stock Photos
- Image Search
- Semantic Search
- Computer-Vision
- Embeddings
- MCP
- agent-native
- Content Licensing
---
