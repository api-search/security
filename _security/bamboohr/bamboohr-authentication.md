---
api_key_in: []
api_specs:
- filename: bamboohr-asyncapi.yml
  format: yaml
  label: BambooHR Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-asyncapi.yml
- filename: bamboohr-directory-api-openapi.yml
  format: yaml
  label: BambooHR Directory API
  slug: bamboohr-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-directory-api-openapi.yml
- filename: bamboohr-employees-api-openapi.yml
  format: yaml
  label: BambooHR Employees API
  slug: bamboohr-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-employees-api-openapi.yml
- filename: bamboohr-files-api-openapi.yml
  format: yaml
  label: BambooHR Files API
  slug: bamboohr-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-files-api-openapi.yml
- filename: bamboohr-meta-api-openapi.yml
  format: yaml
  label: BambooHR Meta API
  slug: bamboohr-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-meta-api-openapi.yml
- filename: bamboohr-reports-api-openapi.yml
  format: yaml
  label: BambooHR Reports API
  slug: bamboohr-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-reports-api-openapi.yml
- filename: bamboohr-time-off-api-openapi.yml
  format: yaml
  label: BambooHR Time Off API
  slug: bamboohr-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-time-off-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bamboohr Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BambooHR secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BambooHR
provider_slug: bamboohr
scheme_count: 2
schemes:
- description: HTTP Basic auth. Use the API key as the username and any non-empty string as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bamboohr-openapi.yml
  type: http
- description: OAuth 2.0 authorization code flow (for multi-customer apps).
  flows:
  - authorizationUrl: https://api.bamboohr.com/oauth/authorize.php
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.bamboohr.com/token.php
  name: oauth2
  sources:
  - openapi/bamboohr-openapi.yml
  type: oauth2
slug: bamboohr-authentication
source_filename: bamboohr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bamboohr-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth. Use the API key as the username and any non-empty string as\n    the password.\n  sources:\n  - openapi/bamboohr-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bamboohr.com/oauth/authorize.php\n    tokenUrl: https://api.bamboohr.com/token.php\n    scopes: 1\n  description: OAuth 2.0 authorization code flow (for multi-customer apps).\n  sources:\n  - openapi/bamboohr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/authentication/bamboohr-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- HR
- HRIS
- Human Resources
- Payroll
- Time Tracking
- Applicant Tracking
- Performance Management
---
