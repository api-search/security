---
anonymous_access: false
api_key_in: []
api_specs:
- filename: github-actions-oidc-api-openapi.yml
  format: yaml
  label: GitHub Actions OIDC API
  slug: github-actions-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-oidc-api-openapi.yml
- filename: github-actions-actions-api-openapi.yml
  format: yaml
  label: GitHub Actions Actions API
  slug: github-actions-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-actions-api-openapi.yml
- filename: github-actions-merge-queue-api-openapi.yml
  format: yaml
  label: GitHub Actions Merge Queue API
  slug: github-actions-merge-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/github-actions/openapi/github-actions-merge-queue-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GitHub Actions Authentication
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
source_yaml_url: https://artifacts.apis.io/github-actions/authentication/github-actions-authentication.yml
summary_line: http · 2 schemes
tags:
- CI/CD
- Continuous Integration
- Continuous Deployment
- DevOps
- Pipelines
- Workflows
- Automation
- Developer Tools
- Software Development
- Build Automation
- T1
- GitHub
---
