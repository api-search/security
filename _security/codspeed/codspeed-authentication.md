---
api_key_in: []
auth_types:
- oauth2
- oidc
- token
- github-app
description: ''
kind: authentication
layout: security
method: searched
name: Codspeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodSpeed secures its APIs with oauth2, oidc, token, and github-app across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CodSpeed
provider_slug: codspeed
scheme_count: 4
schemes:
- detail: The hosted MCP server uses OAuth. On first connect the client opens a browser to log in to CodSpeed and authorize access; tokens are stored and refreshed automatically. Grants the same repository/data access as the account.
  name: mcp-oauth
  source: https://codspeed.io/docs/ai/mcp
  surface: MCP Server (mcp.codspeed.io/mcp)
  type: oauth2
- detail: 'Benchmark runs authenticate to CodSpeed from GitHub Actions via OIDC, requiring the workflow `id-token: write` permission (no stored secret).'
  name: ci-oidc
  source: https://codspeed.io/docs/integrations/ci/github-actions/index
  surface: GitHub Actions CI
  type: openIdConnect
- detail: Browser-based `codspeed auth login` links the CLI to your CodSpeed account.
  name: cli-login
  source: https://codspeed.io/docs/cli
  surface: CodSpeed CLI
  type: token
- detail: CodSpeed integrates with repositories via a GitHub App (and GitLab); source code is never stored.
  name: github-app
  source: https://codspeed.io/docs/integrations/providers/github
  surface: Repository integration
  type: github-app
slug: codspeed-authentication
source_filename: codspeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://codspeed.io/docs\nnotes: >-\n  CodSpeed publishes no standalone public REST API OpenAPI, so this profile is\n  searched from the docs rather than derived from a spec. It documents the auth\n  models across CodSpeed's programmatic surfaces.\nsummary:\n  types: [oauth2, oidc, token, github-app]\nschemes:\n  - name: mcp-oauth\n    surface: MCP Server (mcp.codspeed.io/mcp)\n    type: oauth2\n    detail: >-\n      The hosted MCP server uses OAuth. On first connect the client opens a\n      browser to log in to CodSpeed and authorize access; tokens are stored and\n      refreshed automatically. Grants the same repository/data access as the\n      account.\n    source: https://codspeed.io/docs/ai/mcp\n  - name: ci-oidc\n    surface: GitHub Actions CI\n    type: openIdConnect\n    detail: >-\n      Benchmark runs authenticate to CodSpeed from GitHub Actions via OIDC,\n      requiring the workflow `id-token: write` permission\
  \ (no stored secret).\n    source: https://codspeed.io/docs/integrations/ci/github-actions/index\n  - name: cli-login\n    surface: CodSpeed CLI\n    type: token\n    detail: Browser-based `codspeed auth login` links the CLI to your CodSpeed account.\n    source: https://codspeed.io/docs/cli\n  - name: github-app\n    surface: Repository integration\n    type: github-app\n    detail: >-\n      CodSpeed integrates with repositories via a GitHub App (and GitLab);\n      source code is never stored.\n    source: https://codspeed.io/docs/integrations/providers/github\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codspeed/refs/heads/main/authentication/codspeed-authentication.yml
summary_line: oauth2/oidc/token/github-app · 4 schemes
tags:
- Company
- Performance
- Benchmarking
- Continuous Integration
- Developer Tools
- Observability
- Testing
- DevOps
- AI
- MCP
---
