---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commareports-com-account-api-openapi.yml
  format: yaml
  label: Comma Account API
  slug: commareports-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-account-api-openapi.yml
- filename: commareports-com-assets-api-openapi.yml
  format: yaml
  label: Comma Assets API
  slug: commareports-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-assets-api-openapi.yml
- filename: commareports-com-comments-api-openapi.yml
  format: yaml
  label: Comma Comments API
  slug: commareports-com-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-comments-api-openapi.yml
- filename: commareports-com-connectors-api-openapi.yml
  format: yaml
  label: Comma Connectors API
  slug: commareports-com-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-connectors-api-openapi.yml
- filename: commareports-com-meta-api-openapi.yml
  format: yaml
  label: Comma Meta API
  slug: commareports-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-meta-api-openapi.yml
- filename: commareports-com-notifications-api-openapi.yml
  format: yaml
  label: Comma Notifications API
  slug: commareports-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-notifications-api-openapi.yml
- filename: commareports-com-reports-api-openapi.yml
  format: yaml
  label: Comma Reports API
  slug: commareports-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reports-api-openapi.yml
- filename: commareports-com-reviewers-api-openapi.yml
  format: yaml
  label: Comma Reviewers API
  slug: commareports-com-reviewers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reviewers-api-openapi.yml
- filename: commareports-com-reviews-api-openapi.yml
  format: yaml
  label: Comma Reviews API
  slug: commareports-com-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-reviews-api-openapi.yml
- filename: commareports-com-revisions-api-openapi.yml
  format: yaml
  label: Comma Revisions API
  slug: commareports-com-revisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-revisions-api-openapi.yml
- filename: commareports-com-routines-api-openapi.yml
  format: yaml
  label: Comma Routines API
  slug: commareports-com-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-routines-api-openapi.yml
- filename: commareports-com-sharing-api-openapi.yml
  format: yaml
  label: Comma Sharing API
  slug: commareports-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-sharing-api-openapi.yml
- filename: commareports-com-skills-api-openapi.yml
  format: yaml
  label: Comma Skills API
  slug: commareports-com-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commareports-com/openapi/commareports-com-skills-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Comma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comma secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Comma
provider_slug: commareports-com
scheme_count: 2
schemes:
- bearerFormat: comma_sk_…
  description: Comma personal API token (Settings → API tokens). Scoped, revocable, optionally expiring. The same token also authenticates the MCP server at /api/mcp.
  expiry: Tokens can carry an expiry date; expired tokens fail with 401.
  header: 'Authorization: Bearer comma_sk_…'
  name: commaApiToken
  provisioning: Settings → API tokens → New token in the app; the value is shown once at creation and stored hashed server-side.
  revocation: Revocation from Settings → API tokens is immediate and applies to the REST API and the MCP server in the same motion.
  scheme: bearer
  scopes_docs: https://commareports.com/docs/api-tokens
  sources:
  - openapi/commareports-com-openapi.yml
  - https://commareports.com/docs/api-tokens
  type: http
- bearerFormat: JWT
  description: Supabase user-session access token — the signed-in browser path. Only accepted where an operation explicitly lists it.
  name: supabaseSessionJwt
  scheme: bearer
  sources:
  - openapi/_original/commareports-com-openapi.json
  type: http
slug: commareports-com-authentication
source_filename: commareports-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commareports.com/docs/api-tokens\ndocs: https://commareports.com/docs/api-tokens\nsummary:\n  types:\n  - http\n  token_format: comma_sk_…\n  same_token_surfaces: [REST API, MCP server, Claude Code plugin]\nschemes:\n- name: commaApiToken\n  type: http\n  scheme: bearer\n  bearerFormat: comma_sk_…\n  description: Comma personal API token (Settings → API tokens). Scoped, revocable, optionally expiring. The same token also authenticates the MCP server at /api/mcp.\n  header: 'Authorization: Bearer comma_sk_…'\n  provisioning: Settings → API tokens → New token in the app; the value is shown once at creation and stored hashed server-side.\n  scopes_docs: https://commareports.com/docs/api-tokens\n  expiry: Tokens can carry an expiry date; expired tokens fail with 401.\n  revocation: Revocation from Settings → API tokens is immediate and applies to the REST API and the MCP server in the same motion.\n  sources:\n  - openapi/commareports-com-openapi.yml\n\
  \  - https://commareports.com/docs/api-tokens\n- name: supabaseSessionJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Supabase user-session access token — the signed-in browser path. Only accepted where an operation explicitly lists it.\n  sources:\n  - openapi/_original/commareports-com-openapi.json\nerrors:\n  missing_scope: '403 Token missing scope: …'\n  bad_or_expired_token: '401'\n"
source_yaml_url: https://artifacts.apis.io/commareports-com/authentication/commareports-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Reports
- Collaboration
- Comments
- HTML
- MCP
- AI Agents
- Data Visualization
---
