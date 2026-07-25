---
api_key_in: []
api_specs:
- filename: dagshub-branches-api-openapi.yml
  format: yaml
  label: DagsHub Branches API
  slug: dagshub-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-branches-api-openapi.yml
- filename: dagshub-issues-api-openapi.yml
  format: yaml
  label: DagsHub Issues API
  slug: dagshub-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-issues-api-openapi.yml
- filename: dagshub-orgs-api-openapi.yml
  format: yaml
  label: DagsHub Orgs API
  slug: dagshub-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-orgs-api-openapi.yml
- filename: dagshub-pullrequests-api-openapi.yml
  format: yaml
  label: DagsHub PullRequests API
  slug: dagshub-pullrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-pullrequests-api-openapi.yml
- filename: dagshub-repos-api-openapi.yml
  format: yaml
  label: DagsHub Repos API
  slug: dagshub-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-repos-api-openapi.yml
- filename: dagshub-storage-api-openapi.yml
  format: yaml
  label: DagsHub Storage API
  slug: dagshub-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-storage-api-openapi.yml
- filename: dagshub-user-api-openapi.yml
  format: yaml
  label: DagsHub User API
  slug: dagshub-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-user-api-openapi.yml
- filename: dagshub-users-api-openapi.yml
  format: yaml
  label: DagsHub Users API
  slug: dagshub-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/openapi/dagshub-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dagshub Authentication
name_suffix: Authentication
oauth_flows: []
overview: DagsHub secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DagsHub
provider_slug: dagshub
scheme_count: 2
schemes:
- description: DagsHub access token sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/dagshub-openapi.yml
  type: http
- description: Username and DagsHub access token via HTTP Basic auth.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/dagshub-openapi.yml
  type: http
slug: dagshub-authentication
source_filename: dagshub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dagshub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: DagsHub access token sent as a Bearer token.\n  sources:\n  - openapi/dagshub-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Username and DagsHub access token via HTTP Basic auth.\n  sources:\n  - openapi/dagshub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagshub/refs/heads/main/authentication/dagshub-authentication.yml
summary_line: http · 2 schemes
tags:
- ML
- MLOps
- Data Versioning
- Git
- MLflow
---
