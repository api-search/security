---
api_key_in:
- header
api_specs:
- filename: rest-api-description
  format: yaml
  label: GitHub Enterprise Cloud REST API
  slug: cloud-rest-api
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
- filename: rest-api-description
  format: yaml
  label: GitHub Enterprise Server REST API
  slug: server-rest-api
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
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
