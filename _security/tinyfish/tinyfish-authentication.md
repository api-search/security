---
api_key_in:
- header
api_specs:
- filename: tinyfish-automation-api-openapi.yml
  format: yaml
  label: TinyFish Automation API
  slug: tinyfish-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-automation-api-openapi.yml
- filename: tinyfish-runs-api-openapi.yml
  format: yaml
  label: TinyFish Runs API
  slug: tinyfish-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-runs-api-openapi.yml
- filename: tinyfish-tinyfish-browser-api-api-openapi.yml
  format: yaml
  label: TinyFish TinyFish Browser API API
  slug: tinyfish-tinyfish-browser-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-tinyfish-browser-api-api-openapi.yml
- filename: tinyfish-tinyfish-fetch-api-api-openapi.yml
  format: yaml
  label: TinyFish TinyFish Fetch API API
  slug: tinyfish-tinyfish-fetch-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-tinyfish-fetch-api-api-openapi.yml
- filename: tinyfish-tinyfish-search-api-api-openapi.yml
  format: yaml
  label: TinyFish TinyFish Search API API
  slug: tinyfish-tinyfish-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-tinyfish-search-api-api-openapi.yml
- filename: tinyfish-usage-api-openapi.yml
  format: yaml
  label: TinyFish Usage API
  slug: tinyfish-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-usage-api-openapi.yml
- filename: tinyfish-vault-api-openapi.yml
  format: yaml
  label: TinyFish Vault API
  slug: tinyfish-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/openapi/tinyfish-vault-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tinyfish Authentication
name_suffix: Authentication
oauth_flows: []
overview: TinyFish secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TinyFish
provider_slug: tinyfish
scheme_count: 2
schemes:
- description: API key for authentication. Get your key from the API Keys page (agent.tinyfish.ai/api-keys).
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/tinyfish-main-openapi.json
  - openapi/tinyfish-search-openapi.json
  - openapi/tinyfish-fetch-openapi.json
  - openapi/tinyfish-browser-openapi.json
  type: apiKey
- description: OIDC discovery for TinyFish dashboard/user login via Clerk. Not used for programmatic API calls (those use X-API-Key).
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://clerk.tinyfish.ai
  name: ClerkOIDC
  openIdConnectUrl: https://clerk.tinyfish.ai/.well-known/openid-configuration
  scope: dashboard-sso-only
  scopes_supported:
  - openid
  - email
  - profile
  - offline_access
  - public_metadata
  - private_metadata
  sources:
  - well-known/tinyfish-openid-configuration.json
  type: openIdConnect
slug: tinyfish-authentication
source_filename: tinyfish-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tinyfish-main-openapi.json, openapi/tinyfish-search-openapi.json, openapi/tinyfish-fetch-openapi.json, openapi/tinyfish-browser-openapi.json\ndocs: https://docs.tinyfish.ai/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_name: X-API-Key\n  oauth2_flows: []\n  notes: >-\n    All four public TinyFish APIs (Agent/Automation, Search, Fetch, Browser)\n    authenticate with an X-API-Key request header. Keys are issued from the\n    dashboard at agent.tinyfish.ai/api-keys. A separate OIDC/OAuth surface\n    (issuer clerk.tinyfish.ai) exists for dashboard/user SSO login only and is\n    not the programmatic API auth model.\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    description: API key for authentication. Get your key from the API Keys page (agent.tinyfish.ai/api-keys).\n    sources:\n      - openapi/tinyfish-main-openapi.json\n      - openapi/tinyfish-search-openapi.json\n\
  \      - openapi/tinyfish-fetch-openapi.json\n      - openapi/tinyfish-browser-openapi.json\n  - name: ClerkOIDC\n    type: openIdConnect\n    scope: dashboard-sso-only\n    openIdConnectUrl: https://clerk.tinyfish.ai/.well-known/openid-configuration\n    issuer: https://clerk.tinyfish.ai\n    grant_types: [authorization_code, refresh_token]\n    scopes_supported: [openid, email, profile, offline_access, public_metadata, private_metadata]\n    description: >-\n      OIDC discovery for TinyFish dashboard/user login via Clerk. Not used for\n      programmatic API calls (those use X-API-Key).\n    sources:\n      - well-known/tinyfish-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tinyfish/refs/heads/main/authentication/tinyfish-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Web Automation
- Web Scraping
- Search
- Browser Automation
- MCP
- Data Extraction
---
