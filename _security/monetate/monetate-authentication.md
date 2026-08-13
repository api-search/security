---
api_key_in:
- header
api_specs:
- filename: monetate-engine-api-openapi.yml
  format: yaml
  label: Monetate Engine API
  slug: monetate-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-engine-api-openapi.yml
- filename: monetate-data-api-openapi.yml
  format: yaml
  label: Monetate Data API
  slug: monetate-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-data-api-openapi.yml
- filename: monetate-metadata-api-openapi.yml
  format: yaml
  label: Monetate Metadata API
  slug: monetate-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-metadata-api-openapi.yml
- filename: monetate-auth-api-openapi.yml
  format: yaml
  label: Monetate Auth API
  slug: monetate-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/openapi/monetate-auth-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Monetate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monetate secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Monetate
provider_slug: monetate
scheme_count: 3
schemes:
- algorithms:
  - RS256
  - RS384
  - RS512
  api: Monetate Auth API
  credential_provisioning: Self-service inside the Monetate platform UI — generate an API key/username on the API Keys tab of the Sites page under Settings, and upload the matching RSA public key. Requires an existing Monetate account; there is no public signup.
  description: A signed JSON Web Token proves possession of a private key whose public half was uploaded in the Monetate platform (Settings > Sites > API Keys tab). The JWT payload must carry an `iat` claim (Unix timestamp of the request; 60 seconds of clock skew allowed) and a `username` claim matching the API username generated on that API Keys tab.
  in: header
  name: JWTAuthentication
  parameter: Authorization
  revocation: Deactivate the public key in the UI; every token issued against it stops working (403).
  source: openapi/monetate-auth-api-openapi.yml
  type: apiKey
  value_format: JWT <signed_jwt>
- api: Monetate Metadata API
  description: Opaque bearer token obtained from GET /api/auth/v0/refresh/. Sent on every Metadata API request.
  in: header
  name: TokenAuthentication
  parameter: Authorization
  source: openapi/monetate-metadata-api-openapi.yml
  type: apiKey
  value_format: Token <token_string>
- api: Monetate Data API
  description: Same opaque bearer token as the Metadata API. Note the securityScheme key in the Data API spec contains a space ("Token Authentication") while the Metadata API spec uses "TokenAuthentication" — the same mechanism named two ways across two published specs.
  in: header
  name: Token Authentication
  parameter: Authorization
  source: openapi/monetate-data-api-openapi.yml
  type: apiKey
  value_format: Token <token_string>
slug: monetate-authentication
source_filename: monetate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developer.monetate.com/auth-api\ndocs:\n- https://developer.monetate.com/auth-api\n- https://developer.monetate.com/auth-api/token\n- https://developer.monetate.com/auth-api/refresh-token\n- https://developer.monetate.com/metadata-api/get-interpretable-values-with-the-metadata-api\n- openapi/monetate-auth-api-openapi.yml\n- openapi/monetate-data-api-openapi.yml\n- openapi/monetate-metadata-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  note: >-\n    Two different Authorization header schemes are in play and the specs do not make that obvious. A\n    caller first signs a JWT with an RSA private key and sends `Authorization: JWT <jwt>` to the Auth API;\n    the Auth API returns an opaque bearer token, which is then sent as `Authorization: Token <token>` to\n    the Data API and Metadata API. The Engine API is\
  \ different again — it is unauthenticated at the\n    transport level and identifies the caller by the retailer shortname in the path plus the account\n    fields in the request body.\nschemes:\n- name: JWTAuthentication\n  api: Monetate Auth API\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: JWT <signed_jwt>\n  description: >-\n    A signed JSON Web Token proves possession of a private key whose public half was uploaded in the\n    Monetate platform (Settings > Sites > API Keys tab). The JWT payload must carry an `iat` claim (Unix\n    timestamp of the request; 60 seconds of clock skew allowed) and a `username` claim matching the API\n    username generated on that API Keys tab.\n  algorithms:\n  - RS256\n  - RS384\n  - RS512\n  credential_provisioning: >-\n    Self-service inside the Monetate platform UI — generate an API key/username on the API Keys tab of the\n    Sites page under Settings, and upload the matching RSA public key. Requires an existing Monetate\n\
  \    account; there is no public signup.\n  revocation: Deactivate the public key in the UI; every token issued against it stops working (403).\n  source: openapi/monetate-auth-api-openapi.yml\n- name: TokenAuthentication\n  api: Monetate Metadata API\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: Token <token_string>\n  description: >-\n    Opaque bearer token obtained from GET /api/auth/v0/refresh/. Sent on every Metadata API request.\n  source: openapi/monetate-metadata-api-openapi.yml\n- name: Token Authentication\n  api: Monetate Data API\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: Token <token_string>\n  description: >-\n    Same opaque bearer token as the Metadata API. Note the securityScheme key in the Data API spec\n    contains a space (\"Token Authentication\") while the Metadata API spec uses \"TokenAuthentication\" —\n    the same mechanism named two ways across two published specs.\n  source: openapi/monetate-data-api-openapi.yml\n\
  token_flow:\n  step_1:\n    request: GET https://api.monetate.net/api/auth/v0/refresh/?ttl=3600\n    headers:\n      Authorization: JWT <signed_jwt>\n    query:\n      ttl:\n        description: Requested token lifetime in seconds.\n        default: 3600\n        minimum: 600\n        maximum: 43200\n  step_2:\n    response_body_path: data.token\n    also_returns:\n    - data.expires_in\n    - data.expires_at\n    note: >-\n      `expires_in` always equals the requested `ttl`; `expires_at` is seconds since epoch, so a client can\n      pre-emptively refresh rather than waiting for a 401.\n  step_3:\n    request: Any Data API or Metadata API call\n    headers:\n      Authorization: Token <token_string>\nunauthenticated_surfaces:\n- api: Monetate Engine API\n  endpoint: POST https://engine.monetate.net/api/engine/v1/decide/{retailerShortname}\n  note: >-\n    The published Swagger 2.0 document declares no securityDefinitions and no security requirement. The\n    caller is identified by the\
  \ retailer shortname path parameter and the channel/instance/domain values\n    in the request body. This is deliberate — the endpoint is designed to be called from a browser or a\n    mobile app where no secret can be held — but it means the Engine API's access model is not described\n    in machine-readable form anywhere.\ngaps:\n- >-\n  The Auth API spec declares JWTAuthentication as `type: apiKey` rather than `type: http, scheme: bearer,\n  bearerFormat: JWT`, so tooling cannot tell it is a JWT from the spec alone.\n- No `security` block is applied per-operation in the Engine API spec.\n- No OAuth 2.0, no OpenID Connect, no scopes anywhere in the product APIs. (The only OAuth surface Monetate\n  publishes is on the WordPress marketing site's MCP server — see mcp/monetate-mcp.yml.)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetate/refs/heads/main/authentication/monetate-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Personalization
- Experience Optimization
- A/B Testing
- Ecommerce
- Product Recommendations
- Personalized Search
- Marketing
- Customer Data
- Retail
- Decision Engine
---
