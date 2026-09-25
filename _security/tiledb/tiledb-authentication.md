---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: tiledb-array-api-openapi.yml
  format: yaml
  label: TileDB Array API
  slug: tiledb-array-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-array-api-openapi.yml
- filename: tiledb-array-tasks-api-openapi.yml
  format: yaml
  label: TileDB Array Tasks API
  slug: tiledb-array-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-array-tasks-api-openapi.yml
- filename: tiledb-assets-api-openapi.yml
  format: yaml
  label: TileDB Assets API
  slug: tiledb-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-assets-api-openapi.yml
- filename: tiledb-favorites-api-openapi.yml
  format: yaml
  label: TileDB Favorites API
  slug: tiledb-favorites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-favorites-api-openapi.yml
- filename: tiledb-files-api-openapi.yml
  format: yaml
  label: TileDB Files API
  slug: tiledb-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-files-api-openapi.yml
- filename: tiledb-groups-api-openapi.yml
  format: yaml
  label: TileDB Groups API
  slug: tiledb-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-groups-api-openapi.yml
- filename: tiledb-invitation-api-openapi.yml
  format: yaml
  label: TileDB Invitation API
  slug: tiledb-invitation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-invitation-api-openapi.yml
- filename: tiledb-notebook-api-openapi.yml
  format: yaml
  label: TileDB Notebook API
  slug: tiledb-notebook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-notebook-api-openapi.yml
- filename: tiledb-notebooks-api-openapi.yml
  format: yaml
  label: TileDB Notebooks API
  slug: tiledb-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-notebooks-api-openapi.yml
- filename: tiledb-organization-api-openapi.yml
  format: yaml
  label: TileDB Organization API
  slug: tiledb-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-organization-api-openapi.yml
- filename: tiledb-query-api-openapi.yml
  format: yaml
  label: TileDB Query API
  slug: tiledb-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-query-api-openapi.yml
- filename: tiledb-registered-task-graphs-api-openapi.yml
  format: yaml
  label: TileDB Registered Task Graphs API
  slug: tiledb-registered-task-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-registered-task-graphs-api-openapi.yml
- filename: tiledb-sql-api-openapi.yml
  format: yaml
  label: TileDB Sql API
  slug: tiledb-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-sql-api-openapi.yml
- filename: tiledb-stats-api-openapi.yml
  format: yaml
  label: TileDB Stats API
  slug: tiledb-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-stats-api-openapi.yml
- filename: tiledb-task-graph-logs-api-openapi.yml
  format: yaml
  label: TileDB Task Graph Logs API
  slug: tiledb-task-graph-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-task-graph-logs-api-openapi.yml
- filename: tiledb-task-graphs-api-openapi.yml
  format: yaml
  label: TileDB Task Graphs API
  slug: tiledb-task-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-task-graphs-api-openapi.yml
- filename: tiledb-tasks-api-openapi.yml
  format: yaml
  label: TileDB Tasks API
  slug: tiledb-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-tasks-api-openapi.yml
- filename: tiledb-udf-api-openapi.yml
  format: yaml
  label: TileDB Udf API
  slug: tiledb-udf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-udf-api-openapi.yml
- filename: tiledb-user-api-openapi.yml
  format: yaml
  label: TileDB User API
  slug: tiledb-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiledb/refs/heads/main/openapi/tiledb-user-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
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
- Machine Learning
---
