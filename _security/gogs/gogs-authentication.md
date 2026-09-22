---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: gogs-administration-api-openapi.yml
  format: yaml
  label: Gogs Administration API
  slug: gogs-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-administration-api-openapi.yml
- filename: gogs-collaborators-and-deploy-keys-api-openapi.yml
  format: yaml
  label: Gogs Collaborators and Deploy Keys API
  slug: gogs-collaborators-and-deploy-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-collaborators-and-deploy-keys-api-openapi.yml
- filename: gogs-issues-api-openapi.yml
  format: yaml
  label: Gogs Issues API
  slug: gogs-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-issues-api-openapi.yml
- filename: gogs-miscellaneous-api-openapi.yml
  format: yaml
  label: Gogs Miscellaneous API
  slug: gogs-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-miscellaneous-api-openapi.yml
- filename: gogs-organizations-api-openapi.yml
  format: yaml
  label: Gogs Organizations API
  slug: gogs-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-organizations-api-openapi.yml
- filename: gogs-releases-api-openapi.yml
  format: yaml
  label: Gogs Releases API
  slug: gogs-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-releases-api-openapi.yml
- filename: gogs-repositories-api-openapi.yml
  format: yaml
  label: Gogs Repositories API
  slug: gogs-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-repositories-api-openapi.yml
- filename: gogs-users-api-openapi.yml
  format: yaml
  label: Gogs Users API
  slug: gogs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-users-api-openapi.yml
- filename: gogs-webhooks-api-openapi.yml
  format: yaml
  label: Gogs Webhooks API
  slug: gogs-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/openapi/gogs-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Gogs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gogs secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gogs
provider_slug: gogs
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/gogs-openapi.json
  type: http
- description: 'Personal access token. Use format: token {YOUR_ACCESS_TOKEN}'
  in: header
  name: AccessToken
  parameter: Authorization
  sources:
  - openapi/gogs-openapi.json
  type: apiKey
slug: gogs-authentication
source_filename: gogs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: derived\nsource: openapi/gogs-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/gogs-openapi.json\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Personal access token. Use format: token {YOUR_ACCESS_TOKEN}'\n  sources:\n  - openapi/gogs-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gogs/refs/heads/main/authentication/gogs-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Git
- Self-hosted
- Open-source
- Go
---
