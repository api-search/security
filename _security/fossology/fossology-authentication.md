---
api_key_in: []
api_specs:
- filename: fossology-admin-api-openapi.yml
  format: yaml
  label: FOSSology Admin API
  slug: fossology-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-admin-api-openapi.yml
- filename: fossology-auth-api-openapi.yml
  format: yaml
  label: FOSSology auth API
  slug: fossology-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-auth-api-openapi.yml
- filename: fossology-copyrights-api-openapi.yml
  format: yaml
  label: FOSSology Copyrights API
  slug: fossology-copyrights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-copyrights-api-openapi.yml
- filename: fossology-folders-api-openapi.yml
  format: yaml
  label: FOSSology Folders API
  slug: fossology-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-folders-api-openapi.yml
- filename: fossology-groups-api-openapi.yml
  format: yaml
  label: FOSSology Groups API
  slug: fossology-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-groups-api-openapi.yml
- filename: fossology-info-api-openapi.yml
  format: yaml
  label: FOSSology info API
  slug: fossology-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-info-api-openapi.yml
- filename: fossology-job-api-openapi.yml
  format: yaml
  label: FOSSology Job API
  slug: fossology-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-job-api-openapi.yml
- filename: fossology-license-api-openapi.yml
  format: yaml
  label: FOSSology License API
  slug: fossology-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-license-api-openapi.yml
- filename: fossology-maintenance-api-openapi.yml
  format: yaml
  label: FOSSology Maintenance API
  slug: fossology-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-maintenance-api-openapi.yml
- filename: fossology-organize-api-openapi.yml
  format: yaml
  label: FOSSology Organize API
  slug: fossology-organize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-organize-api-openapi.yml
- filename: fossology-overview-api-openapi.yml
  format: yaml
  label: FOSSology Overview API
  slug: fossology-overview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-overview-api-openapi.yml
- filename: fossology-report-api-openapi.yml
  format: yaml
  label: FOSSology Report API
  slug: fossology-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-report-api-openapi.yml
- filename: fossology-search-api-openapi.yml
  format: yaml
  label: FOSSology Search API
  slug: fossology-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-search-api-openapi.yml
- filename: fossology-upload-api-openapi.yml
  format: yaml
  label: FOSSology Upload API
  slug: fossology-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-upload-api-openapi.yml
- filename: fossology-user-api-openapi.yml
  format: yaml
  label: FOSSology User API
  slug: fossology-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/openapi/fossology-user-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Fossology Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FOSSology secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FOSSology
provider_slug: fossology
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Token from FOSSology
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fossology-openapi.yml
  type: http
- description: Machine-2-Machine communication from oauth
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.example.com/oauth2/authorize
  name: oauth
  sources:
  - openapi/fossology-openapi.yml
  type: oauth2
slug: fossology-authentication
source_filename: fossology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fossology-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Token from FOSSology\n  sources:\n  - openapi/fossology-openapi.yml\n- name: oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.example.com/oauth2/authorize\n    scopes: 0\n  description: Machine-2-Machine communication from oauth\n  sources:\n  - openapi/fossology-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/authentication/fossology-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Compliance
- Licensing
- Linux Foundation
- Scanning
- SPDX
- Open Source
---
