---
api_key_in:
- header
api_specs:
- filename: nevercode-app-previews-api-openapi.yml
  format: yaml
  label: Nevercode App Previews API
  slug: nevercode-app-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-app-previews-api-openapi.yml
- filename: nevercode-applications-api-openapi.yml
  format: yaml
  label: Nevercode Applications API
  slug: nevercode-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-applications-api-openapi.yml
- filename: nevercode-billing-api-openapi.yml
  format: yaml
  label: Nevercode Billing API
  slug: nevercode-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-billing-api-openapi.yml
- filename: nevercode-build-dashboards-api-openapi.yml
  format: yaml
  label: Nevercode Build Dashboards API
  slug: nevercode-build-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-build-dashboards-api-openapi.yml
- filename: nevercode-builds-api-openapi.yml
  format: yaml
  label: Nevercode Builds API
  slug: nevercode-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-builds-api-openapi.yml
- filename: nevercode-meta-api-openapi.yml
  format: yaml
  label: Nevercode Meta API
  slug: nevercode-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-meta-api-openapi.yml
- filename: nevercode-over-the-air-updates-api-openapi.yml
  format: yaml
  label: Nevercode Over-the-air Updates API
  slug: nevercode-over-the-air-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-over-the-air-updates-api-openapi.yml
- filename: nevercode-secrets-and-environment-vars-api-openapi.yml
  format: yaml
  label: Nevercode Secrets and Environment Vars API
  slug: nevercode-secrets-and-environment-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-secrets-and-environment-vars-api-openapi.yml
- filename: nevercode-team-invitations-api-openapi.yml
  format: yaml
  label: Nevercode Team Invitations API
  slug: nevercode-team-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-team-invitations-api-openapi.yml
- filename: nevercode-team-members-api-openapi.yml
  format: yaml
  label: Nevercode Team Members API
  slug: nevercode-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-team-members-api-openapi.yml
- filename: nevercode-teams-api-openapi.yml
  format: yaml
  label: Nevercode Teams API
  slug: nevercode-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-teams-api-openapi.yml
- filename: nevercode-tester-groups-api-openapi.yml
  format: yaml
  label: Nevercode Tester Groups API
  slug: nevercode-tester-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-tester-groups-api-openapi.yml
- filename: nevercode-users-api-openapi.yml
  format: yaml
  label: Nevercode Users API
  slug: nevercode-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Nevercode Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nevercode secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nevercode
provider_slug: nevercode
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: x-auth-token
  sources:
  - openapi/nevercode-openapi-original.json
  type: apiKey
slug: nevercode-authentication
source_filename: nevercode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/nevercode-openapi-original.json\ndocs: https://docs.codemagic.io/rest-api/overview/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  note: Personal API token sent in the x-auth-token request header; token is managed in Account settings\n    and can be revoked/regenerated.\nschemes:\n- name: api_key\n  type: apiKey\n  sources:\n  - openapi/nevercode-openapi-original.json\n  in: header\n  parameter: x-auth-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/authentication/nevercode-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Continuous Integration
- Continuous Delivery
- CI/CD
- DevOps
- Mobile
- Flutter
- Builds
- App Distribution
- Code Signing
---
