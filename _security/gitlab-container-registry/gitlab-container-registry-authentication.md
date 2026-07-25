---
api_key_in:
- header
api_specs:
- filename: gitlab-container-registry-repositories-api-openapi.yml
  format: yaml
  label: GitLab Container Registry Repositories API
  slug: gitlab-container-registry-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/openapi/gitlab-container-registry-repositories-api-openapi.yml
- filename: gitlab-container-registry-tags-api-openapi.yml
  format: yaml
  label: GitLab Container Registry Tags API
  slug: gitlab-container-registry-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/openapi/gitlab-container-registry-tags-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gitlab Container Registry Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GitLab Container Registry secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GitLab Container Registry
provider_slug: gitlab-container-registry
scheme_count: 2
schemes:
- in: header
  name: PrivateToken
  parameter: PRIVATE-TOKEN
  sources:
  - openapi/gitlab-container-registry-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://gitlab.com/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://gitlab.com/oauth/token
  name: OAuth2
  sources:
  - openapi/gitlab-container-registry-openapi.yml
  type: oauth2
slug: gitlab-container-registry-authentication
source_filename: gitlab-container-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitlab-container-registry-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: PrivateToken\n  type: apiKey\n  in: header\n  parameter: PRIVATE-TOKEN\n  sources:\n  - openapi/gitlab-container-registry-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://gitlab.com/oauth/authorize\n    tokenUrl: https://gitlab.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/gitlab-container-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab-container-registry/refs/heads/main/authentication/gitlab-container-registry-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Container Images
- Containers
- GitLab
- Registry
---
