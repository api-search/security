---
api_key_in: []
api_specs:
- filename: github-actions-artifacts-api-openapi.yml
  format: yaml
  label: GitHub Actions Artifacts API
  slug: github-actions-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-artifacts-api-openapi.yml
- filename: github-actions-cache-api-openapi.yml
  format: yaml
  label: GitHub Actions Cache API
  slug: github-actions-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-cache-api-openapi.yml
- filename: github-actions-jobs-api-openapi.yml
  format: yaml
  label: GitHub Actions Jobs API
  slug: github-actions-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-jobs-api-openapi.yml
- filename: github-actions-oidc-api-openapi.yml
  format: yaml
  label: GitHub Actions OIDC API
  slug: github-actions-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-oidc-api-openapi.yml
- filename: github-actions-permissions-api-openapi.yml
  format: yaml
  label: GitHub Actions Permissions API
  slug: github-actions-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-permissions-api-openapi.yml
- filename: github-actions-secrets-api-openapi.yml
  format: yaml
  label: GitHub Actions Secrets API
  slug: github-actions-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-secrets-api-openapi.yml
- filename: github-actions-self-hosted-runner-groups-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runner Groups API
  slug: github-actions-self-hosted-runner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-self-hosted-runner-groups-api-openapi.yml
- filename: github-actions-self-hosted-runners-api-openapi.yml
  format: yaml
  label: GitHub Actions Self-Hosted Runners API
  slug: github-actions-self-hosted-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-self-hosted-runners-api-openapi.yml
- filename: github-actions-variables-api-openapi.yml
  format: yaml
  label: GitHub Actions Variables API
  slug: github-actions-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-variables-api-openapi.yml
- filename: github-actions-workflow-runs-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflow Runs API
  slug: github-actions-workflow-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-workflow-runs-api-openapi.yml
- filename: github-actions-workflows-api-openapi.yml
  format: yaml
  label: GitHub Actions Workflows API
  slug: github-actions-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/openapi/github-actions-workflows-api-openapi.yml
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
