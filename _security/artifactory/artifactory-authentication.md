---
api_key_in:
- header
api_specs:
- filename: artifactory-aql-search-api-openapi.yml
  format: yaml
  label: JFrog Artifactory AQL Search API
  slug: artifactory-aql-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-aql-search-api-openapi.yml
- filename: artifactory-artifactory-extensions-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Artifactory Extensions API
  slug: artifactory-artifactory-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-artifactory-extensions-api-openapi.yml
- filename: artifactory-artifacts-storage-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Artifacts & Storage API
  slug: artifactory-artifacts-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-artifacts-storage-api-openapi.yml
- filename: artifactory-base-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Base API
  slug: artifactory-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-base-api-openapi.yml
- filename: artifactory-blobs-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Blobs API
  slug: artifactory-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-blobs-api-openapi.yml
- filename: artifactory-build-diff-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Diff API
  slug: artifactory-build-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-diff-api-openapi.yml
- filename: artifactory-build-info-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Info API
  slug: artifactory-build-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-info-api-openapi.yml
- filename: artifactory-build-management-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Management API
  slug: artifactory-build-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-management-api-openapi.yml
- filename: artifactory-build-promotion-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Build Promotion API
  slug: artifactory-build-promotion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-promotion-api-openapi.yml
- filename: artifactory-catalog-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Catalog API
  slug: artifactory-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-catalog-api-openapi.yml
- filename: artifactory-manifests-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Manifests API
  slug: artifactory-manifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-manifests-api-openapi.yml
- filename: artifactory-replication-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Replication API
  slug: artifactory-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-replication-api-openapi.yml
- filename: artifactory-repositories-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Repositories API
  slug: artifactory-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-repositories-api-openapi.yml
- filename: artifactory-search-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Search API
  slug: artifactory-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-search-api-openapi.yml
- filename: artifactory-security-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Security API
  slug: artifactory-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-security-api-openapi.yml
- filename: artifactory-system-configuration-api-openapi.yml
  format: yaml
  label: JFrog Artifactory System & Configuration API
  slug: artifactory-system-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-system-configuration-api-openapi.yml
- filename: artifactory-tags-api-openapi.yml
  format: yaml
  label: JFrog Artifactory Tags API
  slug: artifactory-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-tags-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Artifactory Authentication
name_suffix: Authentication
oauth_flows: []
overview: JFrog Artifactory secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JFrog Artifactory
provider_slug: artifactory
scheme_count: 3
schemes:
- description: Access token authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/artifactory-aql-api-openapi.yml
  - openapi/artifactory-build-integration-api-openapi.yml
  - openapi/artifactory-docker-registry-api-openapi.yml
  - openapi/artifactory-rest-api-openapi.yml
  type: http
- description: API key authentication via header
  in: header
  name: ApiKeyAuth
  parameter: X-JFrog-Art-Api
  sources:
  - openapi/artifactory-aql-api-openapi.yml
  - openapi/artifactory-build-integration-api-openapi.yml
  - openapi/artifactory-rest-api-openapi.yml
  type: apiKey
- description: HTTP Basic authentication
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/artifactory-aql-api-openapi.yml
  - openapi/artifactory-build-integration-api-openapi.yml
  - openapi/artifactory-docker-registry-api-openapi.yml
  - openapi/artifactory-rest-api-openapi.yml
  type: http
slug: artifactory-authentication
source_filename: artifactory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/artifactory-aql-api-openapi.yml, openapi/artifactory-build-integration-api-openapi.yml,\n  openapi/artifactory-docker-registry-api-openapi.yml, openapi/artifactory-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Access token authentication\n  sources:\n  - openapi/artifactory-aql-api-openapi.yml\n  - openapi/artifactory-build-integration-api-openapi.yml\n  - openapi/artifactory-docker-registry-api-openapi.yml\n  - openapi/artifactory-rest-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-JFrog-Art-Api\n  description: API key authentication via header\n  sources:\n  - openapi/artifactory-aql-api-openapi.yml\n  - openapi/artifactory-build-integration-api-openapi.yml\n  - openapi/artifactory-rest-api-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description:\
  \ HTTP Basic authentication\n  sources:\n  - openapi/artifactory-aql-api-openapi.yml\n  - openapi/artifactory-build-integration-api-openapi.yml\n  - openapi/artifactory-docker-registry-api-openapi.yml\n  - openapi/artifactory-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/authentication/artifactory-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Artifacts
- DevOps
- CI/CD
- docker-registry
- Maven
- Package Management
- Repository
---
