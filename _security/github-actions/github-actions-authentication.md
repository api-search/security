---
api_key_in: []
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Actions API
  slug: github-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Github Actions Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitHub Actions secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: GitHub Actions
provider_slug: github-actions
scheme_count: 2
schemes:
- description: 'Authorization: Bearer <token>. Accepts a fine-grained or classic personal access token, an OAuth user-to-server token, a GitHub App installation access token, or the automatic GITHUB_TOKEN inside a workflow run.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/github-actions-openapi.yml
  type: http
- description: Fine-grained personal access token scoped with Actions permissions.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/github-actions-openapi.yml
  type: http
slug: github-actions-authentication
source_filename: github-actions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: https://docs.github.com/en/rest/authentication/authenticating-to-the-rest-api\ndocs: https://docs.github.com/en/rest/authentication/authenticating-to-the-rest-api\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  token_types:\n  - fine-grained-pat\n  - classic-pat\n  - oauth-user-token\n  - github-app-installation-token\n  - github-actions-job-token\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Authorization: Bearer <token>. Accepts a fine-grained or classic personal\n    access token, an OAuth user-to-server token, a GitHub App installation\n    access token, or the automatic GITHUB_TOKEN inside a workflow run.\n  sources:\n  - openapi/github-actions-openapi.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  description: Fine-grained personal access token scoped with Actions permissions.\n  sources:\n  - openapi/github-actions-openapi.yml\nnotes:\n  - Access\
  \ is governed by classic OAuth scopes or fine-grained token/App permissions; see scopes/github-actions-scopes.yml.\n  - Basic auth with username + PAT is deprecated; bearer-token auth is required.\n  - GITHUB_TOKEN permissions inside a workflow are declared via the workflow `permissions:` block.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/authentication/github-actions-authentication.yml
summary_line: http · 2 schemes
tags: []
---
