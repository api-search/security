---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Kaggle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaggle declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Kaggle
provider_slug: kaggle
scheme_count: 3
schemes:
- authorizationUrl: https://www.kaggle.com/api/v1/oauth2/authorize
  flow: authorization_code (PKCE S256) + refresh_token
  registration_endpoint: https://www.kaggle.com/api/v1/oauth2/register
  scopes:
  - resources.admin:*
  tokenUrl: https://www.kaggle.com/api/v1/oauth2/token
  type: oauth2
  used_by:
  - kaggle auth login
  - https://www.kaggle.com/mcp
- description: API token from https://www.kaggle.com/settings/api ("Generate New Token"), supplied via KAGGLE_API_TOKEN env var or ~/.kaggle/access_token
  scheme: bearer
  type: http
- description: 'Legacy API key: kaggle.json (username + key) stored at ~/.kaggle/kaggle.json, created via "Create Legacy API Key"'
  type: legacy-credentials-file
slug: kaggle-authentication
source_filename: kaggle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Kaggle authentication\ngenerated: '2026-11-11'\nmethod: searched\nsource: https://raw.githubusercontent.com/Kaggle/kaggle-api/main/docs/README.md; https://www.kaggle.com/.well-known/oauth-authorization-server\ndocs: https://github.com/Kaggle/kaggle-cli/blob/main/docs/README.md\nschemes:\n- type: oauth2\n  flow: authorization_code (PKCE S256) + refresh_token\n  authorizationUrl: https://www.kaggle.com/api/v1/oauth2/authorize\n  tokenUrl: https://www.kaggle.com/api/v1/oauth2/token\n  registration_endpoint: https://www.kaggle.com/api/v1/oauth2/register\n  scopes:\n  - resources.admin:*\n  used_by:\n  - kaggle auth login\n  - https://www.kaggle.com/mcp\n- type: http\n  scheme: bearer\n  description: API token from https://www.kaggle.com/settings/api (\"Generate New Token\"),\n    supplied via KAGGLE_API_TOKEN env var or ~/.kaggle/access_token\n- type: legacy-credentials-file\n  description: 'Legacy API key: kaggle.json (username + key) stored at ~/.kaggle/kaggle.json,\n \
  \   created via \"Create Legacy API Key\"'\ncredential_page: https://www.kaggle.com/settings/api\n"
source_yaml_url: https://artifacts.apis.io/kaggle/authentication/kaggle-authentication.yml
summary_line: 3 schemes
tags:
- CLI
- Competitions
- Data Science
- Datasets
- MCP
- Machine Learning
- Open Data
- Public APIs
---
