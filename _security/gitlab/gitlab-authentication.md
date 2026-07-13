---
api_key_in:
- header
api_specs:
- filename: gitlab-api-v4-groups-openapi-original.yml
  format: yaml
  label: GitLab Groups API
  slug: apiv4groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-groups-openapi-original.yml
- filename: gitlab-api-v4-projects-openapi-original.yml
  format: yaml
  label: GitLab Projects API
  slug: apiv4projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-projects-openapi-original.yml
- filename: gitlab-api-v4-admin-openapi-original.yml
  format: yaml
  label: GitLab Admin API
  slug: apiv4admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-admin-openapi-original.yml
- filename: gitlab-api-v4-applications-openapi-original.yml
  format: yaml
  label: GitLab Applications API
  slug: apiv4applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-applications-openapi-original.yml
- filename: gitlab-api-v4-avatar-openapi-original.yml
  format: yaml
  label: GitLab Avatar API
  slug: apiv4avatar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-avatar-openapi-original.yml
- filename: gitlab-api-v4-broadcast-messages-openapi-original.yml
  format: yaml
  label: GitLab Broadcast Messages API
  slug: apiv4broadcast-messages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-broadcast-messages-openapi-original.yml
- filename: gitlab-api-v4-bulk-imports-openapi-original.yml
  format: yaml
  label: GitLab Bulk Imports API
  slug: apiv4bulk-imports
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-bulk-imports-openapi-original.yml
- filename: gitlab-api-v4-application-openapi-original.yml
  format: yaml
  label: GitLab Application Settings API
  slug: apiv4application
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-application-openapi-original.yml
- filename: gitlab-api-v4-metadata-openapi-original.yml
  format: yaml
  label: GitLab Metadata API
  slug: apiv4metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-metadata-openapi-original.yml
- filename: gitlab-api-v4-version-openapi-original.yml
  format: yaml
  label: GitLab Version API
  slug: apiv4version
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-api-v4-version-openapi-original.yml
- filename: gitlab-openapi-original.yml
  format: yaml
  label: GitLab REST API
  slug: gitlab-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-openapi-original.yml
- filename: gitlab-oauth2-openapi.yml
  format: yaml
  label: GitLab OAuth 2.0 API
  slug: gitlab-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-oauth2-openapi.yml
- filename: gitlab-webhooks-openapi.yml
  format: yaml
  label: GitLab Webhooks
  slug: gitlab-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhooks-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitLab secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GitLab
provider_slug: gitlab
scheme_count: 3
schemes:
- description: OAuth 2.0 access token obtained via the authorization flow.
  name: oauthToken
  scheme: bearer
  sources:
  - openapi/gitlab-oauth2-openapi.yml
  - openapi/gitlab-webhooks-openapi.yml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: Private-Token
  sources:
  - openapi/gitlab-openapi-original.yml
  type: apiKey
- description: GitLab personal access token or project access token.
  in: header
  name: privateToken
  parameter: PRIVATE-TOKEN
  sources:
  - openapi/gitlab-webhooks-openapi.yml
  type: apiKey
slug: gitlab-authentication
source_filename: gitlab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitlab-oauth2-openapi.yml, openapi/gitlab-openapi-original.yml, openapi/gitlab-webhooks-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: oauthToken\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token obtained via the authorization flow.\n  sources:\n  - openapi/gitlab-oauth2-openapi.yml\n  - openapi/gitlab-webhooks-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Private-Token\n  sources:\n  - openapi/gitlab-openapi-original.yml\n- name: privateToken\n  type: apiKey\n  in: header\n  parameter: PRIVATE-TOKEN\n  description: GitLab personal access token or project access token.\n  sources:\n  - openapi/gitlab-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/authentication/gitlab-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Code
- Platform
- Software Development
- Source Control
---
