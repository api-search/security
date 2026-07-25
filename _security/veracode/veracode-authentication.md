---
api_key_in: []
api_specs:
- filename: veracode-api-credentials-api-openapi.yml
  format: yaml
  label: Veracode API Credentials API
  slug: veracode-api-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-api-credentials-api-openapi.yml
- filename: veracode-applications-api-openapi.yml
  format: yaml
  label: Veracode Applications API
  slug: veracode-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-applications-api-openapi.yml
- filename: veracode-business-units-api-openapi.yml
  format: yaml
  label: Veracode Business Units API
  slug: veracode-business-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-business-units-api-openapi.yml
- filename: veracode-findings-api-openapi.yml
  format: yaml
  label: Veracode Findings API
  slug: veracode-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-findings-api-openapi.yml
- filename: veracode-manual-penetration-testing-api-openapi.yml
  format: yaml
  label: Veracode Manual Penetration Testing API
  slug: veracode-manual-penetration-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-manual-penetration-testing-api-openapi.yml
- filename: veracode-policy-evaluations-api-openapi.yml
  format: yaml
  label: Veracode Policy Evaluations API
  slug: veracode-policy-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-policy-evaluations-api-openapi.yml
- filename: veracode-reports-api-openapi.yml
  format: yaml
  label: Veracode Reports API
  slug: veracode-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-reports-api-openapi.yml
- filename: veracode-roles-api-openapi.yml
  format: yaml
  label: Veracode Roles API
  slug: veracode-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-roles-api-openapi.yml
- filename: veracode-sandboxes-api-openapi.yml
  format: yaml
  label: Veracode Sandboxes API
  slug: veracode-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-sandboxes-api-openapi.yml
- filename: veracode-teams-api-openapi.yml
  format: yaml
  label: Veracode Teams API
  slug: veracode-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-teams-api-openapi.yml
- filename: veracode-users-api-openapi.yml
  format: yaml
  label: Veracode Users API
  slug: veracode-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veracode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veracode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veracode
provider_slug: veracode
scheme_count: 1
schemes:
- description: HMAC authentication with Veracode API ID and key credentials
  name: HmacAuth
  scheme: veracode_hmac
  sources:
  - openapi/veracode-applications-openapi.yml
  - openapi/veracode-findings-openapi.yml
  - openapi/veracode-identity-openapi.yml
  - openapi/veracode-reporting-openapi.yml
  type: http
slug: veracode-authentication
source_filename: veracode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veracode-applications-openapi.yml, openapi/veracode-findings-openapi.yml, openapi/veracode-identity-openapi.yml,\n  openapi/veracode-reporting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HmacAuth\n  type: http\n  scheme: veracode_hmac\n  description: HMAC authentication with Veracode API ID and key credentials\n  sources:\n  - openapi/veracode-applications-openapi.yml\n  - openapi/veracode-findings-openapi.yml\n  - openapi/veracode-identity-openapi.yml\n  - openapi/veracode-reporting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/authentication/veracode-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Security
- SAST
- DAST
- SCA
- Security Testing
- DevSecOps
---
