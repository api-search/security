---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: antfly-ai-api-openapi.yml
  format: yaml
  label: Antfly AI API
  slug: antfly-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-ai-api-openapi.yml
- filename: antfly-cluster-management-api-openapi.yml
  format: yaml
  label: Antfly Cluster Management API
  slug: antfly-cluster-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-cluster-management-api-openapi.yml
- filename: antfly-data-operations-api-openapi.yml
  format: yaml
  label: Antfly Data Operations API
  slug: antfly-data-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-data-operations-api-openapi.yml
- filename: antfly-documents-api-openapi.yml
  format: yaml
  label: Antfly Documents API
  slug: antfly-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-documents-api-openapi.yml
- filename: antfly-index-management-api-openapi.yml
  format: yaml
  label: Antfly Index Management API
  slug: antfly-index-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-index-management-api-openapi.yml
- filename: antfly-inference-api-openapi.yml
  format: yaml
  label: Antfly Inference API
  slug: antfly-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-inference-api-openapi.yml
- filename: antfly-installed-api-openapi.yml
  format: yaml
  label: Antfly Installed API
  slug: antfly-installed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-installed-api-openapi.yml
- filename: antfly-memory-api-openapi.yml
  format: yaml
  label: Antfly Memory API
  slug: antfly-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-memory-api-openapi.yml
- filename: antfly-ml-api-openapi.yml
  format: yaml
  label: Antfly Ml API
  slug: antfly-ml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-ml-api-openapi.yml
- filename: antfly-models-api-openapi.yml
  format: yaml
  label: Antfly Models API
  slug: antfly-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-models-api-openapi.yml
- filename: antfly-packages-api-openapi.yml
  format: yaml
  label: Antfly Packages API
  slug: antfly-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-packages-api-openapi.yml
- filename: antfly-permission-api-openapi.yml
  format: yaml
  label: Antfly Permission API
  slug: antfly-permission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-permission-api-openapi.yml
- filename: antfly-personal-connections-api-openapi.yml
  format: yaml
  label: Antfly Personal Connections API
  slug: antfly-personal-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-personal-connections-api-openapi.yml
- filename: antfly-query-operations-api-openapi.yml
  format: yaml
  label: Antfly Query Operations API
  slug: antfly-query-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-query-operations-api-openapi.yml
- filename: antfly-resolver-curation-api-openapi.yml
  format: yaml
  label: Antfly Resolver Curation API
  slug: antfly-resolver-curation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-resolver-curation-api-openapi.yml
- filename: antfly-role-api-openapi.yml
  format: yaml
  label: Antfly Role API
  slug: antfly-role-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-role-api-openapi.yml
- filename: antfly-rowfilter-api-openapi.yml
  format: yaml
  label: Antfly Row Filter API
  slug: antfly-rowfilter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-rowfilter-api-openapi.yml
- filename: antfly-table-management-api-openapi.yml
  format: yaml
  label: Antfly Table Management API
  slug: antfly-table-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-table-management-api-openapi.yml
- filename: antfly-user-api-openapi.yml
  format: yaml
  label: Antfly User API
  slug: antfly-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-user-api-openapi.yml
- filename: antfly-api-key-api-openapi.yml
  format: yaml
  label: Antfly API Key API
  slug: antfly-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antfly/openapi/antfly-api-key-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Antfly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Antfly secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Antfly
provider_slug: antfly
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/antfly-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/antfly-openapi.yaml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/antfly-openapi.yaml
  type: http
slug: antfly-authentication
source_filename: antfly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/antfly-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/antfly-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/antfly-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/antfly-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/antfly/authentication/antfly-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- AI
- Search
- Retrieval
- Vector
- Hybrid
---
