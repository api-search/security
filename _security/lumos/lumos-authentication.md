---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lumos-tasks-api-openapi.yml
  format: yaml
  label: Lumos Tasks API
  slug: lumos-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-tasks-api-openapi.yml
- filename: lumos-access-reviews-api-openapi.yml
  format: yaml
  label: Lumos Access Reviews API
  slug: lumos-access-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-access-reviews-api-openapi.yml
- filename: lumos-core-api-openapi.yml
  format: yaml
  label: Lumos Core API
  slug: lumos-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-core-api-openapi.yml
- filename: lumos-integration-webhooks-api-openapi.yml
  format: yaml
  label: Lumos Integration Webhooks API
  slug: lumos-integration-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-integration-webhooks-api-openapi.yml
- filename: lumos-knowledge-api-openapi.yml
  format: yaml
  label: Lumos Knowledge API
  slug: lumos-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-knowledge-api-openapi.yml
- filename: lumos-lifecycle-management-api-openapi.yml
  format: yaml
  label: Lumos Lifecycle Management API
  slug: lumos-lifecycle-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-lifecycle-management-api-openapi.yml
- filename: lumos-meta-api-openapi.yml
  format: yaml
  label: Lumos Meta API
  slug: lumos-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-meta-api-openapi.yml
- filename: lumos-vendor-management-api-openapi.yml
  format: yaml
  label: Lumos Vendor Management API
  slug: lumos-vendor-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-vendor-management-api-openapi.yml
- filename: lumos-app-store-api-openapi.yml
  format: yaml
  label: Lumos App Store API
  slug: lumos-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-app-store-api-openapi.yml
auth_types:
- http
- oauth2
description: Lumos runs TWO independent credential systems on one host. The REST API takes a static bearer API key prefixed `lsk_`. The two hosted MCP servers take an OAuth 2.1 access token from b.app.lumosidentity.com and explicitly refuse API keys. An agent that has a working REST key still cannot call the MCP servers, and vice versa.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lumos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumos secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lumos
provider_slug: lumos
scheme_count: 2
schemes:
- applies_to: REST API (https://api.lumos.com)
  bearerFormat: Lumos API key (lsk_ prefix)
  expiry: not documented
  in: Authorization header
  key_prefix: lsk_
  name: HTTPBearer
  rotation: not documented
  scheme: bearer
  sources:
  - openapi/lumos-openapi.json
  - https://developers.lumos.com/docs/rest-api
  type: http
- applies_to:
  - https://api.lumos.com/mcp/user
  - https://api.lumos.com/mcp/admin
  discovery:
  - https://api.lumos.com/.well-known/oauth-authorization-server
  - https://api.lumos.com/.well-known/oauth-protected-resource/mcp/user
  - https://api.lumos.com/.well-known/oauth-protected-resource/mcp/admin
  dynamic_client_registration: https://b.app.lumosidentity.com/b/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://b.app.lumosidentity.com/b/oauth/authorize
      pkce: S256
      refreshUrl: https://b.app.lumosidentity.com/b/oauth/token
      tokenUrl: https://b.app.lumosidentity.com/b/oauth/token
  issuer: https://b.app.lumosidentity.com
  name: LumosOAuth
  note: Public-client friendly — `none` is an accepted token endpoint auth method and RFC 7591 dynamic registration is open, which is what lets an arbitrary MCP client onboard without a pre-provisioned client_id.
  scopes: scopes/lumos-scopes.yml
  sources:
  - well-known/lumos-oauth-authorization-server.json
  - https://developers.lumos.com/docs/mcp
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: lumos-authentication
source_filename: lumos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://developers.lumos.com/docs/rest-api, https://api.lumos.com/openapi.json,\n  https://api.lumos.com/.well-known/oauth-authorization-server, and the RFC 9728 protected-resource\n  documents for both MCP endpoints\ndocs: https://developers.lumos.com/docs/rest-api\ndescription: >-\n  Lumos runs TWO independent credential systems on one host. The REST API takes a static bearer API\n  key prefixed `lsk_`. The two hosted MCP servers take an OAuth 2.1 access token from\n  b.app.lumosidentity.com and explicitly refuse API keys. An agent that has a working REST key still\n  cannot call the MCP servers, and vice versa.\nsummary:\n  types:\n  - http\n  - oauth2\n  systems: 2\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: Lumos API key (lsk_ prefix)\n  applies_to: REST API (https://api.lumos.com)\n  in: Authorization header\n  key_prefix: lsk_\n  rotation: not documented\n  expiry: not documented\n\
  \  sources:\n  - openapi/lumos-openapi.json\n  - https://developers.lumos.com/docs/rest-api\n- name: LumosOAuth\n  type: oauth2\n  applies_to:\n  - https://api.lumos.com/mcp/user\n  - https://api.lumos.com/mcp/admin\n  flows:\n    authorizationCode:\n      authorizationUrl: https://b.app.lumosidentity.com/b/oauth/authorize\n      tokenUrl: https://b.app.lumosidentity.com/b/oauth/token\n      refreshUrl: https://b.app.lumosidentity.com/b/oauth/token\n      pkce: S256\n  issuer: https://b.app.lumosidentity.com\n  dynamic_client_registration: https://b.app.lumosidentity.com/b/oauth/register\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  scopes: scopes/lumos-scopes.yml\n  discovery:\n  - https://api.lumos.com/.well-known/oauth-authorization-server\n  - https://api.lumos.com/.well-known/oauth-protected-resource/mcp/user\n  - https://api.lumos.com/.well-known/oauth-protected-resource/mcp/admin\n  sources:\n  - well-known/lumos-oauth-authorization-server.json\n\
  \  - https://developers.lumos.com/docs/mcp\n  note: >-\n    Public-client friendly — `none` is an accepted token endpoint auth method and RFC 7591 dynamic\n    registration is open, which is what lets an arbitrary MCP client onboard without a pre-provisioned\n    client_id.\nchallenge_observed:\n  url: https://api.lumos.com/mcp/user\n  http_status: 401\n  www_authenticate: Bearer resource_metadata=\"https://api.lumos.com/.well-known/oauth-protected-resource/mcp/user\"\n  probed: '2026-08-29'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/authentication/lumos-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
---
