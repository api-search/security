---
api_key_in:
- header
api_specs:
- filename: border0-audit-actions-api-openapi.yml
  format: yaml
  label: Border0 Audit Actions API
  slug: border0-audit-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-audit-actions-api-openapi.yml
- filename: border0-client-api-openapi.yml
  format: yaml
  label: Border0 Client API
  slug: border0-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-client-api-openapi.yml
- filename: border0-connect-api-openapi.yml
  format: yaml
  label: Border0 Connect API
  slug: border0-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-connect-api-openapi.yml
- filename: border0-login-api-openapi.yml
  format: yaml
  label: Border0 Login API
  slug: border0-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-login-api-openapi.yml
- filename: border0-mtls-ca-api-openapi.yml
  format: yaml
  label: Border0 Mtls-Ca API
  slug: border0-mtls-ca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-mtls-ca-api-openapi.yml
- filename: border0-organization-api-openapi.yml
  format: yaml
  label: Border0 Organization API
  slug: border0-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-organization-api-openapi.yml
- filename: border0-organizations-api-openapi.yml
  format: yaml
  label: Border0 Organizations API
  slug: border0-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-organizations-api-openapi.yml
- filename: border0-policies-api-openapi.yml
  format: yaml
  label: Border0 Policies API
  slug: border0-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-policies-api-openapi.yml
- filename: border0-policy-api-openapi.yml
  format: yaml
  label: Border0 Policy API
  slug: border0-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-policy-api-openapi.yml
- filename: border0-session-api-openapi.yml
  format: yaml
  label: Border0 Session API
  slug: border0-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-session-api-openapi.yml
- filename: border0-sessions-api-openapi.yml
  format: yaml
  label: Border0 Sessions API
  slug: border0-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-sessions-api-openapi.yml
- filename: border0-socket-api-openapi.yml
  format: yaml
  label: Border0 Socket API
  slug: border0-socket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-socket-api-openapi.yml
- filename: border0-stats-api-openapi.yml
  format: yaml
  label: Border0 Stats API
  slug: border0-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-stats-api-openapi.yml
- filename: border0-user-api-openapi.yml
  format: yaml
  label: Border0 User API
  slug: border0-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-user-api-openapi.yml
- filename: border0-users-api-openapi.yml
  format: yaml
  label: Border0 Users API
  slug: border0-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Border0 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Border0 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Border0
provider_slug: border0
scheme_count: 1
schemes:
- in: header
  name: Border0_Token
  parameter: Authorization
  sources:
  - openapi/border0-openapi.json
  type: apiKey
slug: border0-authentication
source_filename: border0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/border0-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Border0_Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/border0-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/authentication/border0-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Zero Trust
- Network Access
- Security
- Identity and Access Management
- Infrastructure
- VPN
- SSH
- Databases
- Kubernetes
- Company
---
