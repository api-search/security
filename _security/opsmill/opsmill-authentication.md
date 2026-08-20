---
api_key_in:
- header
api_specs:
- filename: opsmill-artifact-api-openapi.yml
  format: yaml
  label: OpsMill Artifact API
  slug: opsmill-artifact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-artifact-api-openapi.yml
- filename: opsmill-auth-api-openapi.yml
  format: yaml
  label: OpsMill Auth API
  slug: opsmill-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-auth-api-openapi.yml
- filename: opsmill-config-api-openapi.yml
  format: yaml
  label: OpsMill Config API
  slug: opsmill-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-config-api-openapi.yml
- filename: opsmill-diff-api-openapi.yml
  format: yaml
  label: OpsMill Diff API
  slug: opsmill-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-diff-api-openapi.yml
- filename: opsmill-file-api-openapi.yml
  format: yaml
  label: OpsMill File API
  slug: opsmill-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-file-api-openapi.yml
- filename: opsmill-info-api-openapi.yml
  format: yaml
  label: OpsMill Info API
  slug: opsmill-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-info-api-openapi.yml
- filename: opsmill-menu-api-openapi.yml
  format: yaml
  label: OpsMill Menu API
  slug: opsmill-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-menu-api-openapi.yml
- filename: opsmill-oauth2-api-openapi.yml
  format: yaml
  label: OpsMill Oauth2 API
  slug: opsmill-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-oauth2-api-openapi.yml
- filename: opsmill-oidc-api-openapi.yml
  format: yaml
  label: OpsMill Oidc API
  slug: opsmill-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-oidc-api-openapi.yml
- filename: opsmill-query-api-openapi.yml
  format: yaml
  label: OpsMill Query API
  slug: opsmill-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-query-api-openapi.yml
- filename: opsmill-schema-api-openapi.yml
  format: yaml
  label: OpsMill Schema API
  slug: opsmill-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-schema-api-openapi.yml
- filename: opsmill-schema-graphql-api-openapi.yml
  format: yaml
  label: OpsMill Schema.graphql API
  slug: opsmill-schema-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-schema-graphql-api-openapi.yml
- filename: opsmill-storage-api-openapi.yml
  format: yaml
  label: OpsMill Storage API
  slug: opsmill-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-storage-api-openapi.yml
- filename: opsmill-telemetry-api-openapi.yml
  format: yaml
  label: OpsMill Telemetry API
  slug: opsmill-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-telemetry-api-openapi.yml
- filename: opsmill-transform-api-openapi.yml
  format: yaml
  label: OpsMill Transform API
  slug: opsmill-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/openapi/opsmill-transform-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Opsmill Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpsMill secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OpsMill
provider_slug: opsmill
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/opsmill-infrahub-openapi-original.json
  type: http
- in: header
  name: APIKeyHeader
  parameter: X-INFRAHUB-KEY
  sources:
  - openapi/opsmill-infrahub-openapi-original.json
  type: apiKey
slug: opsmill-authentication
source_filename: opsmill-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/opsmill-infrahub-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/opsmill-infrahub-openapi-original.json\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-INFRAHUB-KEY\n  sources:\n  - openapi/opsmill-infrahub-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsmill/refs/heads/main/authentication/opsmill-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Infrastructure Saas
- Network Automation
- Source of Truth
- Data Management
- GraphQL
- DevOps
- Configuration Management
- AIOps
- Open-Source
---
