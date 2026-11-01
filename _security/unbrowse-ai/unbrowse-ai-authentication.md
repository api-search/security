---
anonymous_access: false
api_key_in: []
api_specs:
- filename: unbrowse-ai-account-api-openapi.yml
  format: yaml
  label: unbrowse-ai Account API
  slug: unbrowse-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-account-api-openapi.yml
- filename: unbrowse-ai-apps-tools-api-openapi.yml
  format: yaml
  label: unbrowse-ai Apps & tools API
  slug: unbrowse-ai-apps-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-apps-tools-api-openapi.yml
- filename: unbrowse-ai-capabilities-api-openapi.yml
  format: yaml
  label: unbrowse-ai Capabilities API
  slug: unbrowse-ai-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-capabilities-api-openapi.yml
- filename: unbrowse-ai-connected-apps-api-openapi.yml
  format: yaml
  label: unbrowse-ai Connected apps API
  slug: unbrowse-ai-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-connected-apps-api-openapi.yml
- filename: unbrowse-ai-indexing-api-openapi.yml
  format: yaml
  label: unbrowse-ai Indexing API
  slug: unbrowse-ai-indexing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-indexing-api-openapi.yml
- filename: unbrowse-ai-learning-api-openapi.yml
  format: yaml
  label: unbrowse-ai Learning API
  slug: unbrowse-ai-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-learning-api-openapi.yml
- filename: unbrowse-ai-logins-vault-api-openapi.yml
  format: yaml
  label: unbrowse-ai Logins & vault API
  slug: unbrowse-ai-logins-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-logins-vault-api-openapi.yml
- filename: unbrowse-ai-marketplace-api-openapi.yml
  format: yaml
  label: unbrowse-ai Marketplace API
  slug: unbrowse-ai-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-marketplace-api-openapi.yml
- filename: unbrowse-ai-orgs-api-openapi.yml
  format: yaml
  label: unbrowse-ai Orgs API
  slug: unbrowse-ai-orgs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-orgs-api-openapi.yml
- filename: unbrowse-ai-pages-api-openapi.yml
  format: yaml
  label: unbrowse-ai Pages API
  slug: unbrowse-ai-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-pages-api-openapi.yml
- filename: unbrowse-ai-replays-api-openapi.yml
  format: yaml
  label: unbrowse-ai Replays API
  slug: unbrowse-ai-replays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-replays-api-openapi.yml
- filename: unbrowse-ai-runs-api-openapi.yml
  format: yaml
  label: unbrowse-ai Runs API
  slug: unbrowse-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-runs-api-openapi.yml
- filename: unbrowse-ai-saved-queries-api-openapi.yml
  format: yaml
  label: unbrowse-ai Saved queries API
  slug: unbrowse-ai-saved-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-saved-queries-api-openapi.yml
- filename: unbrowse-ai-sites-api-openapi.yml
  format: yaml
  label: unbrowse-ai Sites API
  slug: unbrowse-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unbrowse-ai/openapi/unbrowse-ai-sites-api-openapi.yml
auth_types: []
description: Authentication methods for Unbrowse AI API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Unbrowse Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: unbrowse-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: unbrowse-ai
provider_slug: unbrowse-ai
scheme_count: 2
schemes:
- evidence: 'Send the key as a bearer token: Authorization: Bearer ub_live_…'
  header: Authorization
  how_to_obtain: Create a key in the signed‑in console at https://unbrowse.ai/app
  location: header
  name: UNBROWSE_API_KEY
  type: http-bearer
- evidence: Complete OAuth in your client's browser sign-in.
  how_to_obtain: OAuth flow is performed in the client’s browser when adding the MCP endpoint.
  name: Remote MCP OAuth
  type: oauth2
slug: unbrowse-ai-authentication
source_filename: unbrowse-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.unbrowse.ai/install.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.unbrowse.ai/install.md\nsources:\n- https://docs.unbrowse.ai/install.md\n- https://unbrowse.ai/docs/quickstart\n- https://unbrowse.ai/docs/quickstart.md\ndescription: Authentication methods for Unbrowse AI API\nschemes:\n- type: http-bearer\n  name: UNBROWSE_API_KEY\n  evidence: 'Send the key as a bearer token: Authorization: Bearer ub_live_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the signed‑in console at https://unbrowse.ai/app\n- type: oauth2\n  name: Remote MCP OAuth\n  evidence: Complete OAuth in your client's browser sign-in.\n  how_to_obtain: OAuth flow is performed in the client’s browser when adding the MCP endpoint.\ndocs: https://docs.unbrowse.ai/install.md\n"
source_yaml_url: https://artifacts.apis.io/unbrowse-ai/authentication/unbrowse-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Developer Tools
---
