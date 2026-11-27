---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nowgetitdone-com-api-keys-api-openapi.yml
  format: yaml
  label: GetItDone API keys API
  slug: nowgetitdone-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-api-keys-api-openapi.yml
- filename: nowgetitdone-com-attachments-api-openapi.yml
  format: yaml
  label: GetItDone Attachments API
  slug: nowgetitdone-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-attachments-api-openapi.yml
- filename: nowgetitdone-com-daily-plan-api-openapi.yml
  format: yaml
  label: GetItDone Daily plan API
  slug: nowgetitdone-com-daily-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-daily-plan-api-openapi.yml
- filename: nowgetitdone-com-members-api-openapi.yml
  format: yaml
  label: GetItDone Members API
  slug: nowgetitdone-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-members-api-openapi.yml
- filename: nowgetitdone-com-notes-api-openapi.yml
  format: yaml
  label: GetItDone Notes API
  slug: nowgetitdone-com-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-notes-api-openapi.yml
- filename: nowgetitdone-com-organizations-api-openapi.yml
  format: yaml
  label: GetItDone Organizations API
  slug: nowgetitdone-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-organizations-api-openapi.yml
- filename: nowgetitdone-com-projects-api-openapi.yml
  format: yaml
  label: GetItDone Projects API
  slug: nowgetitdone-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-projects-api-openapi.yml
- filename: nowgetitdone-com-task-dependencies-api-openapi.yml
  format: yaml
  label: GetItDone Task dependencies API
  slug: nowgetitdone-com-task-dependencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-task-dependencies-api-openapi.yml
- filename: nowgetitdone-com-task-occurrences-api-openapi.yml
  format: yaml
  label: GetItDone Task occurrences API
  slug: nowgetitdone-com-task-occurrences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-task-occurrences-api-openapi.yml
- filename: nowgetitdone-com-tasks-api-openapi.yml
  format: yaml
  label: GetItDone Tasks API
  slug: nowgetitdone-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-tasks-api-openapi.yml
- filename: nowgetitdone-com-usage-api-openapi.yml
  format: yaml
  label: GetItDone Usage API
  slug: nowgetitdone-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-usage-api-openapi.yml
- filename: nowgetitdone-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: GetItDone Webhook endpoints API
  slug: nowgetitdone-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nowgetitdone-com/openapi/nowgetitdone-com-webhook-endpoints-api-openapi.yml
auth_types: []
description: Authentication methods for GetItDone API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GetItDone Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetItDone declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GetItDone
provider_slug: nowgetitdone-com
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer gid_YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create an API key in the app (Profile → API Keys) or obtain an OAuth 2.1 access token via sign‑in.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Sign‑ins use OAuth 2.1 with PKCE, and access tokens last 30 days by default.
  how_to_obtain: Sign in through the MCP server; the flow uses PKCE but URLs are not published on the page.
  name: OAuth 2.1
  type: oauth2
slug: nowgetitdone-com-authentication
source_filename: nowgetitdone-com-authentication.yml
source_heading: Authentication Profile
source_url: https://nowgetitdone.com/blog/invalid-access-token-api-key-meaning
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nowgetitdone.com/blog/invalid-access-token-api-key-meaning\nsources:\n- https://nowgetitdone.com/blog/invalid-access-token-api-key-meaning\n- https://nowgetitdone.com/docs/api-reference/api-keys/listApiKeys\n- https://nowgetitdone.com/docs/api\n- https://docs.nowgetitdone.com/docs/api\ndescription: Authentication methods for GetItDone API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer gid_YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the app (Profile → API Keys) or obtain an OAuth 2.1 access token via sign‑in.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Sign‑ins use OAuth 2.1 with PKCE, and access tokens last 30 days by default.\n  how_to_obtain: Sign in through the MCP server; the flow uses PKCE but URLs are not published on the page.\ndocs: https://nowgetitdone.com/blog/invalid-access-token-api-key-meaning\n"
source_yaml_url: https://artifacts.apis.io/nowgetitdone-com/authentication/nowgetitdone-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Task Management
- Collaboration
- Productivity
- Software-as-a-Service
---
