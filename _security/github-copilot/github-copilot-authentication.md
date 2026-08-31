---
api_key_in: []
api_specs:
- filename: github-copilot-copilot-billing-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Billing API
  slug: github-copilot-copilot-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-billing-api-openapi.yml
- filename: github-copilot-copilot-content-exclusion-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Content Exclusion API
  slug: github-copilot-copilot-content-exclusion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-content-exclusion-api-openapi.yml
- filename: github-copilot-copilot-metrics-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Metrics API
  slug: github-copilot-copilot-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-metrics-api-openapi.yml
- filename: github-copilot-copilot-seats-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Seats API
  slug: github-copilot-copilot-seats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-seats-api-openapi.yml
- filename: github-copilot-copilot-usage-reports-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot Usage Reports API
  slug: github-copilot-copilot-usage-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-usage-reports-api-openapi.yml
- filename: github-copilot-copilot-user-management-api-openapi.yml
  format: yaml
  label: GitHub Copilot Copilot User Management API
  slug: github-copilot-copilot-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/openapi/github-copilot-copilot-user-management-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Github Copilot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: GitHub Copilot secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: GitHub Copilot
provider_slug: github-copilot
scheme_count: 2
schemes:
- description: Personal access token (classic) with manage_billing:copilot, read:org, or read:enterprise scopes; or fine-grained token with GitHub Copilot Business (read) or Administration (read) permissions.
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/github-copilot-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://github.com/login/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://github.com/login/oauth/access_token
  name: OAuthToken
  sources:
  - openapi/github-copilot-openapi.yml
  type: oauth2
slug: github-copilot-authentication
source_filename: github-copilot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/github-copilot-openapi.yml\ndocs: https://docs.github.com/en/rest/authentication/authenticating-to-the-rest-api\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: Personal access token (classic) with manage_billing:copilot, read:org, or read:enterprise\n    scopes; or fine-grained token with GitHub Copilot Business (read) or Administration (read)\n    permissions.\n  sources:\n  - openapi/github-copilot-openapi.yml\n- name: OAuthToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://github.com/login/oauth/authorize\n    tokenUrl: https://github.com/login/oauth/access_token\n    scopes: 5\n  sources:\n  - openapi/github-copilot-openapi.yml\ntoken_types:\n- Personal access token (classic) — Authorization bearer; carries OAuth scopes (see scopes/github-copilot-scopes.yml).\n\
  - Fine-grained personal access token — uses org \"GitHub Copilot Business\" (read) and \"Administration\" permissions.\n- OAuth app token / GitHub App installation token — Authorization bearer.\nnotes: >-\n  All GitHub REST requests require a User-Agent header and send the bearer token\n  in the Authorization header. Docs:\n  https://docs.github.com/en/rest/authentication/authenticating-to-the-rest-api\n  and https://docs.github.com/en/rest/copilot/copilot-user-management for the\n  Copilot per-endpoint permission matrix.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/github-copilot/refs/heads/main/authentication/github-copilot-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Agents
- Artificial Intelligence
- Code Generation
- Code Review
- Coding Agent
- Custom Instructions
- Developer Tools
- Extensions
- IDE
- Machine-Learning
- MCP
- Metrics
- Productivity
---
