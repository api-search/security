---
api_key_in:
- header
api_specs:
- filename: gitlab-admin-api-openapi.yml
  format: yaml
  label: GitLab Admin API
  slug: gitlab-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-admin-api-openapi.yml
- filename: gitlab-application-api-openapi.yml
  format: yaml
  label: GitLab Application API
  slug: gitlab-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-application-api-openapi.yml
- filename: gitlab-applications-api-openapi.yml
  format: yaml
  label: GitLab Applications API
  slug: gitlab-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-applications-api-openapi.yml
- filename: gitlab-authorization-api-openapi.yml
  format: yaml
  label: GitLab Authorization API
  slug: gitlab-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-authorization-api-openapi.yml
- filename: gitlab-avatar-api-openapi.yml
  format: yaml
  label: GitLab Avatar API
  slug: gitlab-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-avatar-api-openapi.yml
- filename: gitlab-broadcast-messages-api-openapi.yml
  format: yaml
  label: GitLab Broadcast Messages API
  slug: gitlab-broadcast-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-broadcast-messages-api-openapi.yml
- filename: gitlab-bulk-imports-api-openapi.yml
  format: yaml
  label: GitLab Bulk Imports API
  slug: gitlab-bulk-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-bulk-imports-api-openapi.yml
- filename: gitlab-groups-api-openapi.yml
  format: yaml
  label: GitLab Groups API
  slug: gitlab-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-groups-api-openapi.yml
- filename: gitlab-metadata-api-openapi.yml
  format: yaml
  label: GitLab Metadata API
  slug: gitlab-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-metadata-api-openapi.yml
- filename: gitlab-project-webhooks-api-openapi.yml
  format: yaml
  label: GitLab Project Webhooks API
  slug: gitlab-project-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-project-webhooks-api-openapi.yml
- filename: gitlab-projects-api-openapi.yml
  format: yaml
  label: GitLab Projects API
  slug: gitlab-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-projects-api-openapi.yml
- filename: gitlab-tokens-api-openapi.yml
  format: yaml
  label: GitLab Tokens API
  slug: gitlab-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-tokens-api-openapi.yml
- filename: gitlab-user-info-api-openapi.yml
  format: yaml
  label: GitLab User Info API
  slug: gitlab-user-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-user-info-api-openapi.yml
- filename: gitlab-version-api-openapi.yml
  format: yaml
  label: GitLab Version API
  slug: gitlab-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-version-api-openapi.yml
- filename: gitlab-webhook-configuration-api-openapi.yml
  format: yaml
  label: GitLab Webhook Configuration API
  slug: gitlab-webhook-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhook-configuration-api-openapi.yml
- filename: gitlab-webhook-events-api-openapi.yml
  format: yaml
  label: GitLab Webhook Events API
  slug: gitlab-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/openapi/gitlab-webhook-events-api-openapi.yml
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
