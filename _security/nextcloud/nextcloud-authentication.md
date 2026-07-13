---
api_key_in: []
api_specs:
- filename: nextcloud-openapi.yml
  format: yaml
  label: Nextcloud OCS API
  slug: ocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextcloud/refs/heads/main/openapi/nextcloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nextcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nextcloud secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nextcloud
provider_slug: nextcloud
scheme_count: 2
schemes:
- description: Username + password or username + app token
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/nextcloud-openapi.yml
  type: http
- description: OIDC bearer token issued by an external identity provider
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nextcloud-openapi.yml
  type: http
slug: nextcloud-authentication
source_filename: nextcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nextcloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Username + password or username + app token\n  sources:\n  - openapi/nextcloud-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OIDC bearer token issued by an external identity provider\n  sources:\n  - openapi/nextcloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextcloud/refs/heads/main/authentication/nextcloud-authentication.yml
summary_line: http · 2 schemes
tags:
- File Sync
- File Sharing
- Collaboration
- Self-Hosted
- Open Source
- Productivity
- WebDAV
---
