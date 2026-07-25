---
api_key_in: []
api_specs:
- filename: nowcerts-authentication-api-openapi.yml
  format: yaml
  label: NowCerts Authentication API
  slug: nowcerts-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-authentication-api-openapi.yml
- filename: nowcerts-carriers-api-openapi.yml
  format: yaml
  label: NowCerts Carriers API
  slug: nowcerts-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-carriers-api-openapi.yml
- filename: nowcerts-endorsements-api-openapi.yml
  format: yaml
  label: NowCerts Endorsements API
  slug: nowcerts-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-endorsements-api-openapi.yml
- filename: nowcerts-insureds-api-openapi.yml
  format: yaml
  label: NowCerts Insureds API
  slug: nowcerts-insureds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-insureds-api-openapi.yml
- filename: nowcerts-policies-api-openapi.yml
  format: yaml
  label: NowCerts Policies API
  slug: nowcerts-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-policies-api-openapi.yml
- filename: nowcerts-tasks-api-openapi.yml
  format: yaml
  label: NowCerts Tasks API
  slug: nowcerts-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/openapi/nowcerts-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nowcerts Authentication
name_suffix: Authentication
oauth_flows: []
overview: NowCerts secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NowCerts
provider_slug: nowcerts
scheme_count: 1
schemes:
- description: Bearer token obtained from https://api.nowcerts.com/token via the OAuth2 password grant. The user must have the "API Integration" agent role.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nowcerts-openapi.yml
  type: http
slug: nowcerts-authentication
source_filename: nowcerts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nowcerts-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token obtained from https://api.nowcerts.com/token via the OAuth2 password\n    grant. The user must have the \"API Integration\" agent role.\n  sources:\n  - openapi/nowcerts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nowcerts/refs/heads/main/authentication/nowcerts-authentication.yml
summary_line: http · 1 scheme
tags:
- Insurance
- Insurtech
- Agency Management System
- AMS
- Policies
- Insureds
- Certificates of Insurance
- REST
---
