---
api_key_in:
- header
api_specs:
- filename: artifactory-rest-api-openapi.yml
  format: yaml
  label: Artifactory REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-rest-api-openapi.yml
- filename: artifactory-aql-api-openapi.yml
  format: yaml
  label: Artifactory Query Language (AQL) API
  slug: aql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-aql-api-openapi.yml
- filename: artifactory-docker-registry-api-openapi.yml
  format: yaml
  label: Artifactory Docker Registry API
  slug: docker-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-docker-registry-api-openapi.yml
- filename: artifactory-build-integration-api-openapi.yml
  format: yaml
  label: Artifactory Build Integration API
  slug: build-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/openapi/artifactory-build-integration-api-openapi.yml
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
- Docker Registry
- Maven
- Package Management
- Repository
---
