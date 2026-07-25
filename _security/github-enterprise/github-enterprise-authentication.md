---
api_key_in:
- header
api_specs:
- filename: github-enterprise-actions-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Actions API
  slug: github-enterprise-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-actions-api-openapi.yml
- filename: github-enterprise-code-scanning-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Code Scanning API
  slug: github-enterprise-code-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-code-scanning-api-openapi.yml
- filename: github-enterprise-enterprise-admin-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Enterprise Admin API
  slug: github-enterprise-enterprise-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-enterprise-admin-api-openapi.yml
- filename: github-enterprise-issues-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Issues API
  slug: github-enterprise-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-issues-api-openapi.yml
- filename: github-enterprise-organizations-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Organizations API
  slug: github-enterprise-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-organizations-api-openapi.yml
- filename: github-enterprise-pull-requests-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Pull Requests API
  slug: github-enterprise-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-pull-requests-api-openapi.yml
- filename: github-enterprise-repositories-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Repositories API
  slug: github-enterprise-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-repositories-api-openapi.yml
- filename: github-enterprise-scim-api-openapi.yml
  format: yaml
  label: GitHub Enterprise SCIM API
  slug: github-enterprise-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-scim-api-openapi.yml
- filename: github-enterprise-users-api-openapi.yml
  format: yaml
  label: GitHub Enterprise Users API
  slug: github-enterprise-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/openapi/github-enterprise-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Github Enterprise Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitHub Enterprise secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GitHub Enterprise
provider_slug: github-enterprise
scheme_count: 2
schemes:
- bearerFormat: GitHub Token (PAT or App installation token)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/github-enterprise-openapi.yml
  type: http
- description: Use "token YOUR_PAT" for classic personal access tokens.
  in: header
  name: patAuth
  parameter: Authorization
  sources:
  - openapi/github-enterprise-openapi.yml
  type: apiKey
slug: github-enterprise-authentication
source_filename: github-enterprise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/github-enterprise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: GitHub Token (PAT or App installation token)\n  sources:\n  - openapi/github-enterprise-openapi.yml\n- name: patAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Use \"token YOUR_PAT\" for classic personal access tokens.\n  sources:\n  - openapi/github-enterprise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-enterprise/refs/heads/main/authentication/github-enterprise-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Source Control
- DevOps
- CI/CD
- Code Hosting
- Enterprise
- Self-Hosted
- SAML SSO
- SCIM
- Advanced Security
---
