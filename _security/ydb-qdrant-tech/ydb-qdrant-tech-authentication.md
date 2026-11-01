---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ydb-qdrant-tech-agent-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Agent API
  slug: ydb-qdrant-tech-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-agent-api-openapi.yml
- filename: ydb-qdrant-tech-collections-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Collections API
  slug: ydb-qdrant-tech-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-collections-api-openapi.yml
- filename: ydb-qdrant-tech-discovery-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Discovery API
  slug: ydb-qdrant-tech-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-discovery-api-openapi.yml
- filename: ydb-qdrant-tech-feedback-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Feedback API
  slug: ydb-qdrant-tech-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-feedback-api-openapi.yml
- filename: ydb-qdrant-tech-mcp-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech MCP API
  slug: ydb-qdrant-tech-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-mcp-api-openapi.yml
- filename: ydb-qdrant-tech-pets-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Pets API
  slug: ydb-qdrant-tech-pets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-pets-api-openapi.yml
- filename: ydb-qdrant-tech-points-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Points API
  slug: ydb-qdrant-tech-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-points-api-openapi.yml
- filename: ydb-qdrant-tech-requests-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Requests API
  slug: ydb-qdrant-tech-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-requests-api-openapi.yml
- filename: ydb-qdrant-tech-service-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Service API
  slug: ydb-qdrant-tech-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-service-api-openapi.yml
- filename: ydb-qdrant-tech-submissions-api-openapi.yml
  format: yaml
  label: ydb-qdrant-tech Submissions API
  slug: ydb-qdrant-tech-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb-qdrant-tech/openapi/ydb-qdrant-tech-submissions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Ydb Qdrant Tech Authentication
name_suffix: Authentication
oauth_flows: []
overview: ydb-qdrant-tech declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ydb-qdrant-tech
provider_slug: ydb-qdrant-tech
scheme_count: 3
schemes:
- description: Namespace-oriented REST API key used for vector data operations.
  in: header
  name: api-key
  type: apiKey
- bearerFormat: JWT
  description: Bearer token for hosted Code Indexer MCP repository memory.
  scheme: bearer
  type: http
- description: Optional tenant identifier for multi-tenant namespace separation.
  in: header
  name: X-Tenant-Id
  type: apiKey
slug: ydb-qdrant-tech-authentication
source_filename: ydb-qdrant-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://ydb-qdrant.tech/docs/auth/\nschemes:\n  - type: apiKey\n    name: api-key\n    in: header\n    description: Namespace-oriented REST API key used for vector data operations.\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: Bearer token for hosted Code Indexer MCP repository memory.\n  - type: apiKey\n    name: X-Tenant-Id\n    in: header\n    description: Optional tenant identifier for multi-tenant namespace separation.\n"
source_yaml_url: https://artifacts.apis.io/ydb-qdrant-tech/authentication/ydb-qdrant-tech-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Vector Search
- Database
- API
- YDB
- Qdrant
---
