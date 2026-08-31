---
api_key_in:
- header
api_specs:
- filename: tiledb-cloud-v1-openapi.yaml
  format: yaml
  label: TileDB Storage Platform API (v1)
  slug: tiledb-storage-platform-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-cloud-v1-openapi.yaml
- filename: tiledb-cloud-v2-openapi.yaml
  format: yaml
  label: TileDB Storage Platform API (v2)
  slug: tiledb-storage-platform-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-cloud-v2-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tiledb Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TileDB secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TileDB
provider_slug: tiledb
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/tiledb-cloud-v1-openapi.yaml
  - openapi/tiledb-cloud-v2-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-TILEDB-REST-API-KEY
  sources:
  - openapi/tiledb-cloud-v1-openapi.yaml
  - openapi/tiledb-cloud-v2-openapi.yaml
  type: apiKey
- flows:
  - authorizationUrl: https://oauth2.tiledb.com/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.tiledb.com/oauth2/token
  name: OAuth2
  sources:
  - openapi/tiledb-cloud-v1-openapi.yaml
  - openapi/tiledb-cloud-v2-openapi.yaml
  type: oauth2
slug: tiledb-authentication
source_filename: tiledb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://documentation.cloud.tiledb.com/academy/accounts/individual/profile/api-tokens/ + openapi/tiledb-cloud-v1-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/tiledb-cloud-v1-openapi.yaml\n  - openapi/tiledb-cloud-v2-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-TILEDB-REST-API-KEY\n  sources:\n  - openapi/tiledb-cloud-v1-openapi.yaml\n  - openapi/tiledb-cloud-v2-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth2.tiledb.com/oauth2/authorize\n    tokenUrl: https://oauth2.tiledb.com/oauth2/token\n    scopes: 3\n  sources:\n  - openapi/tiledb-cloud-v1-openapi.yaml\n  - openapi/tiledb-cloud-v2-openapi.yaml\ndocs: https://documentation.cloud.tiledb.com/academy/accounts/individual/profile/api-tokens/\n\
  primary_method: api_key_header\ndetails:\n  api_key_header: X-TILEDB-REST-API-KEY\n  token_type: REST API token, created in the TileDB Cloud console under Profile > API tokens, or via POST /v1/token.\n  token_expiry: User-selected; defaults to 30 minutes when no expiration is set.\n  token_scoping: Optional scope from the TokenScope enum; defaults to all permissions (*). See scopes/tiledb-scopes.yml.\n  environment_variable: TILEDB_REST_TOKEN — TileDB Cloud notebook servers inject a temporary token here at launch.\n  client_config_key: rest.token — the TileDB context config option used by the client libraries instead of username/password.\n  basic_auth: HTTP Basic (username/password) is accepted by the API but the docs steer callers to REST API tokens.\n  oauth2: An authorization-code flow is declared in securityDefinitions against oauth2.tiledb.com, but it is commented\n    out of the global security requirement in the published spec (a note in the spec says it broke the generated\n \
  \   Python client). oauth2.tiledb.com does not resolve in public DNS (NXDOMAIN, probed 2026-08-30).\n  sso: Self-hosted TileDB deployments support OpenID Connect and SCIM 2.0 user provisioning (Okta, Microsoft Entra).\n    See conformance/tiledb-conformance.yml.\nevidence:\n- url: https://api.tiledb.com/v1/user\n  http_status: 401\n  body: '{\"code\":401,\"message\":\"Unauthorized\",\"request_id\":\"...\"}'\n  note: Anonymous probe 2026-08-30 — confirms the live base host and the JSON error envelope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/authentication/tiledb-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Database
- Multimodal Data
- Life Sciences
- Genomics
- Single Cell
- Biomedical Imaging
- Vector Search
- Data Management
- Cloud Storage
- Analytics
- Machine-Learning
---
