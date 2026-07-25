---
api_key_in: []
api_specs:
- filename: checkmarx-applications-api-openapi.yml
  format: yaml
  label: Checkmarx Applications API
  slug: checkmarx-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-applications-api-openapi.yml
- filename: checkmarx-authentication-api-openapi.yml
  format: yaml
  label: Checkmarx Authentication API
  slug: checkmarx-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-authentication-api-openapi.yml
- filename: checkmarx-configuration-api-openapi.yml
  format: yaml
  label: Checkmarx Configuration API
  slug: checkmarx-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-configuration-api-openapi.yml
- filename: checkmarx-engines-api-openapi.yml
  format: yaml
  label: Checkmarx Engines API
  slug: checkmarx-engines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-engines-api-openapi.yml
- filename: checkmarx-groups-api-openapi.yml
  format: yaml
  label: Checkmarx Groups API
  slug: checkmarx-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-groups-api-openapi.yml
- filename: checkmarx-packages-api-openapi.yml
  format: yaml
  label: Checkmarx Packages API
  slug: checkmarx-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-packages-api-openapi.yml
- filename: checkmarx-presets-api-openapi.yml
  format: yaml
  label: Checkmarx Presets API
  slug: checkmarx-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-presets-api-openapi.yml
- filename: checkmarx-projects-api-openapi.yml
  format: yaml
  label: Checkmarx Projects API
  slug: checkmarx-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-projects-api-openapi.yml
- filename: checkmarx-queries-api-openapi.yml
  format: yaml
  label: Checkmarx Queries API
  slug: checkmarx-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-queries-api-openapi.yml
- filename: checkmarx-reports-api-openapi.yml
  format: yaml
  label: Checkmarx Reports API
  slug: checkmarx-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-reports-api-openapi.yml
- filename: checkmarx-results-api-openapi.yml
  format: yaml
  label: Checkmarx Results API
  slug: checkmarx-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-results-api-openapi.yml
- filename: checkmarx-risk-reports-api-openapi.yml
  format: yaml
  label: Checkmarx Risk Reports API
  slug: checkmarx-risk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-risk-reports-api-openapi.yml
- filename: checkmarx-scans-api-openapi.yml
  format: yaml
  label: Checkmarx Scans API
  slug: checkmarx-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-scans-api-openapi.yml
- filename: checkmarx-settings-api-openapi.yml
  format: yaml
  label: Checkmarx Settings API
  slug: checkmarx-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-settings-api-openapi.yml
- filename: checkmarx-teams-api-openapi.yml
  format: yaml
  label: Checkmarx Teams API
  slug: checkmarx-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/openapi/checkmarx-teams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Checkmarx Authentication
name_suffix: Authentication
oauth_flows: []
overview: Checkmarx secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Checkmarx
provider_slug: checkmarx
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 bearer token obtained via client credentials from the Checkmarx One IAM service
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/checkmarx-one-openapi.yml
  - openapi/checkmarx-sast-openapi.yml
  - openapi/checkmarx-sca-openapi.yml
  type: http
slug: checkmarx-authentication
source_filename: checkmarx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/checkmarx-one-openapi.yml, openapi/checkmarx-sast-openapi.yml, openapi/checkmarx-sca-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 bearer token obtained via client credentials from the Checkmarx One\n    IAM service\n  sources:\n  - openapi/checkmarx-one-openapi.yml\n  - openapi/checkmarx-sast-openapi.yml\n  - openapi/checkmarx-sca-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmarx/refs/heads/main/authentication/checkmarx-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Security
- Code Analysis
- DevSecOps
- SAST
- Security Testing
- Vulnerability Scanning
---
