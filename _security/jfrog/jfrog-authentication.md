---
api_key_in:
- header
api_specs:
- filename: jfrog-artifactory-openapi.yml
  format: yaml
  label: JFrog Artifactory REST API
  slug: jfrog-artifactory-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-artifactory-openapi.yml
- filename: jfrog-artifactory-openapi.yml
  format: yaml
  label: JFrog Artifactory REST API V2
  slug: jfrog-artifactory-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-artifactory-openapi.yml
- filename: jfrog-xray-openapi.yml
  format: yaml
  label: JFrog Xray REST API
  slug: jfrog-xray-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-xray-openapi.yml
- filename: jfrog-distribution-openapi.yml
  format: yaml
  label: JFrog Distribution REST API
  slug: jfrog-distribution-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-distribution-openapi.yml
- filename: jfrog-pipelines-openapi.yml
  format: yaml
  label: JFrog Pipelines REST API
  slug: jfrog-pipelines-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-pipelines-openapi.yml
- filename: jfrog-platform-openapi.yml
  format: yaml
  label: JFrog Platform REST API
  slug: jfrog-platform-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-platform-openapi.yml
- filename: jfrog-access-openapi.yml
  format: yaml
  label: JFrog Access REST API
  slug: jfrog-access-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-access-openapi.yml
- filename: jfrog-curation-openapi.yml
  format: yaml
  label: JFrog Curation REST API
  slug: jfrog-curation-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-curation-openapi.yml
- filename: jfrog-mission-control-openapi.yml
  format: yaml
  label: JFrog Mission Control REST API
  slug: jfrog-mission-control-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-mission-control-openapi.yml
- filename: jfrog-release-lifecycle-openapi.yml
  format: yaml
  label: JFrog Release Lifecycle Management REST API
  slug: jfrog-release-lifecycle-management-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-release-lifecycle-openapi.yml
- filename: jfrog-workers-openapi.yml
  format: yaml
  label: JFrog Workers REST API
  slug: jfrog-workers-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-workers-openapi.yml
- filename: jfrog-ml-openapi.yml
  format: yaml
  label: JFrog ML REST API
  slug: jfrog-ml-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-ml-openapi.yml
- filename: jfrog-connect-openapi.yml
  format: yaml
  label: JFrog Connect REST API
  slug: jfrog-connect-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-connect-openapi.yml
- filename: jfrog-catalog-openapi.yml
  format: yaml
  label: JFrog Catalog REST API
  slug: jfrog-catalog-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-catalog-openapi.yml
- filename: jfrog-evidence-openapi.yml
  format: yaml
  label: JFrog Evidence REST API
  slug: jfrog-evidence-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/openapi/jfrog-evidence-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jfrog Authentication
name_suffix: Authentication
oauth_flows: []
overview: JFrog secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: JFrog
provider_slug: jfrog
scheme_count: 4
schemes:
- description: Access token authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jfrog-access-openapi.yml
  - openapi/jfrog-artifactory-openapi.yml
  - openapi/jfrog-catalog-openapi.yml
  - openapi/jfrog-curation-openapi.yml
  - openapi/jfrog-distribution-openapi.yml
  - openapi/jfrog-evidence-openapi.yml
  - openapi/jfrog-mission-control-openapi.yml
  - openapi/jfrog-ml-openapi.yml
  - openapi/jfrog-pipelines-openapi.yml
  - openapi/jfrog-platform-openapi.yml
  - openapi/jfrog-release-lifecycle-openapi.yml
  - openapi/jfrog-workers-openapi.yml
  - openapi/jfrog-xray-openapi.yml
  type: http
- description: Basic username/password authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/jfrog-access-openapi.yml
  - openapi/jfrog-artifactory-openapi.yml
  - openapi/jfrog-catalog-openapi.yml
  - openapi/jfrog-curation-openapi.yml
  - openapi/jfrog-distribution-openapi.yml
  - openapi/jfrog-mission-control-openapi.yml
  - openapi/jfrog-ml-openapi.yml
  - openapi/jfrog-pipelines-openapi.yml
  - openapi/jfrog-platform-openapi.yml
  - openapi/jfrog-release-lifecycle-openapi.yml
  - openapi/jfrog-workers-openapi.yml
  - openapi/jfrog-xray-openapi.yml
  type: http
- description: API key authentication
  in: header
  name: apiKeyAuth
  parameter: X-JFrog-Art-Api
  sources:
  - openapi/jfrog-artifactory-openapi.yml
  type: apiKey
- description: API key authentication using Bearer token format
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/jfrog-connect-openapi.yml
  type: apiKey
slug: jfrog-authentication
source_filename: jfrog-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jfrog-access-openapi.yml, openapi/jfrog-artifactory-openapi.yml, openapi/jfrog-catalog-openapi.yml,\n  openapi/jfrog-connect-openapi.yml, openapi/jfrog-curation-openapi.yml, openapi/jfrog-distribution-openapi.yml,\n  openapi/jfrog-evidence-openapi.yml, openapi/jfrog-mission-control-openapi.yml, openapi/jfrog-ml-openapi.yml,\n  openapi/jfrog-pipelines-openapi.yml, openapi/jfrog-platform-openapi.yml, openapi/jfrog-release-lifecycle-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token authentication\n  sources:\n  - openapi/jfrog-access-openapi.yml\n  - openapi/jfrog-artifactory-openapi.yml\n  - openapi/jfrog-catalog-openapi.yml\n  - openapi/jfrog-curation-openapi.yml\n  - openapi/jfrog-distribution-openapi.yml\n  - openapi/jfrog-evidence-openapi.yml\n  - openapi/jfrog-mission-control-openapi.yml\n\
  \  - openapi/jfrog-ml-openapi.yml\n  - openapi/jfrog-pipelines-openapi.yml\n  - openapi/jfrog-platform-openapi.yml\n  - openapi/jfrog-release-lifecycle-openapi.yml\n  - openapi/jfrog-workers-openapi.yml\n  - openapi/jfrog-xray-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic username/password authentication\n  sources:\n  - openapi/jfrog-access-openapi.yml\n  - openapi/jfrog-artifactory-openapi.yml\n  - openapi/jfrog-catalog-openapi.yml\n  - openapi/jfrog-curation-openapi.yml\n  - openapi/jfrog-distribution-openapi.yml\n  - openapi/jfrog-mission-control-openapi.yml\n  - openapi/jfrog-ml-openapi.yml\n  - openapi/jfrog-pipelines-openapi.yml\n  - openapi/jfrog-platform-openapi.yml\n  - openapi/jfrog-release-lifecycle-openapi.yml\n  - openapi/jfrog-workers-openapi.yml\n  - openapi/jfrog-xray-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-JFrog-Art-Api\n  description: API key authentication\n  sources:\n  - openapi/jfrog-artifactory-openapi.yml\n\
  - name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication using Bearer token format\n  sources:\n  - openapi/jfrog-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/authentication/jfrog-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
---
