---
api_key_in: []
api_specs:
- filename: collate-openmetadata-openapi.yml
  format: yaml
  label: OpenMetadata REST API
  slug: collate-openmetadata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collate/refs/heads/main/openapi/collate-openmetadata-openapi.yml
auth_types:
- http
description: 'OpenMetadata authenticates every REST API request with a JWT Bearer token passed in the Authorization header (`Authorization: Bearer <jwt>`). Tokens are either Bot tokens (Settings > Bots > Generate Token) or Personal Access Tokens (profile > Access Tokens, expiry required, shown once). The server validates the JWT signature and enforces role-based access control before processing the request; expired or invalid tokens return 401. The same JWT works across the Python, Java, and curl/bash clients. The hosted MCP server uses OAuth 2.1 / OIDC (authorization_code + PKCE) — see mcp/collate-mcp.yml.'
kind: authentication
layout: security
method: searched
name: Collate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Collate
provider_slug: collate
scheme_count: 1
schemes:
- bearer_format: JWT
  description: JWT Bearer token in the Authorization header. Issued as a Bot token or a Personal Access Token from the OpenMetadata UI.
  header: 'Authorization: Bearer <jwt-token>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/collate-openmetadata-openapi.yml
  type: http
slug: collate-authentication
source_filename: collate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/collate-openmetadata-openapi.yml\ndocs: https://docs.open-metadata.org/latest/api-reference/authentication\ndescription: >-\n  OpenMetadata authenticates every REST API request with a JWT Bearer token\n  passed in the Authorization header (`Authorization: Bearer <jwt>`). Tokens are\n  either Bot tokens (Settings > Bots > Generate Token) or Personal Access Tokens\n  (profile > Access Tokens, expiry required, shown once). The server validates\n  the JWT signature and enforces role-based access control before processing the\n  request; expired or invalid tokens return 401. The same JWT works across the\n  Python, Java, and curl/bash clients. The hosted MCP server uses OAuth 2.1 /\n  OIDC (authorization_code + PKCE) — see mcp/collate-mcp.yml.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  bearer_format: JWT\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description:\
  \ >-\n    JWT Bearer token in the Authorization header. Issued as a Bot token or a\n    Personal Access Token from the OpenMetadata UI.\n  header: 'Authorization: Bearer <jwt-token>'\n  sources:\n  - openapi/collate-openmetadata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collate/refs/heads/main/authentication/collate-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data
- Metadata
- Data Catalog
- Data Governance
- Data Discovery
- Data Quality
- Data Lineage
- Open Source
- API
---
