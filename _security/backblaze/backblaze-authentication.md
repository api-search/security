---
api_key_in: []
api_specs:
- filename: backblaze-application-keys-api-openapi.yml
  format: yaml
  label: Backblaze Application Keys API
  slug: backblaze-application-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-application-keys-api-openapi.yml
- filename: backblaze-authorization-api-openapi.yml
  format: yaml
  label: Backblaze Authorization API
  slug: backblaze-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-authorization-api-openapi.yml
- filename: backblaze-buckets-api-openapi.yml
  format: yaml
  label: Backblaze Buckets API
  slug: backblaze-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-buckets-api-openapi.yml
- filename: backblaze-files-api-openapi.yml
  format: yaml
  label: Backblaze Files API
  slug: backblaze-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-files-api-openapi.yml
- filename: backblaze-large-files-api-openapi.yml
  format: yaml
  label: Backblaze Large Files API
  slug: backblaze-large-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-large-files-api-openapi.yml
- filename: backblaze-notifications-api-openapi.yml
  format: yaml
  label: Backblaze Notifications API
  slug: backblaze-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-notifications-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Backblaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Backblaze secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Backblaze
provider_slug: backblaze
scheme_count: 2
schemes:
- description: Authorization token obtained from b2_authorize_account
  name: ApplicationKeyAuth
  scheme: bearer
  sources:
  - openapi/backblaze-b2-native-api.yaml
  type: http
- description: HTTP Basic auth using applicationKeyId as username and applicationKey as password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/backblaze-b2-native-api.yaml
  type: http
slug: backblaze-authentication
source_filename: backblaze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/backblaze-b2-native-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApplicationKeyAuth\n  type: http\n  scheme: bearer\n  description: Authorization token obtained from b2_authorize_account\n  sources:\n  - openapi/backblaze-b2-native-api.yaml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using applicationKeyId as username and applicationKey as password\n  sources:\n  - openapi/backblaze-b2-native-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/authentication/backblaze-authentication.yml
summary_line: http · 2 schemes
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
---
