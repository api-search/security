---
anonymous_access: false
api_key_in: []
api_specs:
- filename: condux-ai-admin-api-openapi.yml
  format: yaml
  label: Condux Admin API
  slug: condux-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-admin-api-openapi.yml
- filename: condux-ai-alerts-api-openapi.yml
  format: yaml
  label: Condux Alerts API
  slug: condux-ai-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-alerts-api-openapi.yml
- filename: condux-ai-auth-api-openapi.yml
  format: yaml
  label: Condux Auth API
  slug: condux-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-auth-api-openapi.yml
- filename: condux-ai-billing-api-openapi.yml
  format: yaml
  label: Condux Billing API
  slug: condux-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-billing-api-openapi.yml
- filename: condux-ai-conductor-api-openapi.yml
  format: yaml
  label: Condux Conductor API
  slug: condux-ai-conductor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-conductor-api-openapi.yml
- filename: condux-ai-debugfiles-api-openapi.yml
  format: yaml
  label: Condux Debug Files API
  slug: condux-ai-debugfiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-debugfiles-api-openapi.yml
- filename: condux-ai-github-api-openapi.yml
  format: yaml
  label: Condux GitHub API
  slug: condux-ai-github-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-github-api-openapi.yml
- filename: condux-ai-invites-api-openapi.yml
  format: yaml
  label: Condux Invites API
  slug: condux-ai-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-invites-api-openapi.yml
- filename: condux-ai-issues-api-openapi.yml
  format: yaml
  label: Condux Issues API
  slug: condux-ai-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-issues-api-openapi.yml
- filename: condux-ai-linear-api-openapi.yml
  format: yaml
  label: Condux Linear API
  slug: condux-ai-linear-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-linear-api-openapi.yml
- filename: condux-ai-mcptokens-api-openapi.yml
  format: yaml
  label: Condux MCP Tokens API
  slug: condux-ai-mcptokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-mcptokens-api-openapi.yml
- filename: condux-ai-members-api-openapi.yml
  format: yaml
  label: Condux Members API
  slug: condux-ai-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-members-api-openapi.yml
- filename: condux-ai-notifications-api-openapi.yml
  format: yaml
  label: Condux Notifications API
  slug: condux-ai-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-notifications-api-openapi.yml
- filename: condux-ai-onboarding-api-openapi.yml
  format: yaml
  label: Condux Onboarding API
  slug: condux-ai-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-onboarding-api-openapi.yml
- filename: condux-ai-provisioning-api-openapi.yml
  format: yaml
  label: Condux Provisioning API
  slug: condux-ai-provisioning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-provisioning-api-openapi.yml
- filename: condux-ai-releasetokens-api-openapi.yml
  format: yaml
  label: Condux Release Tokens API
  slug: condux-ai-releasetokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-releasetokens-api-openapi.yml
- filename: condux-ai-repos-api-openapi.yml
  format: yaml
  label: Condux Repos API
  slug: condux-ai-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-repos-api-openapi.yml
- filename: condux-ai-runnertokens-api-openapi.yml
  format: yaml
  label: Condux Runner Tokens API
  slug: condux-ai-runnertokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-runnertokens-api-openapi.yml
- filename: condux-ai-sourcemaps-api-openapi.yml
  format: yaml
  label: Condux Source Maps API
  slug: condux-ai-sourcemaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-sourcemaps-api-openapi.yml
- filename: condux-ai-weeklysummary-api-openapi.yml
  format: yaml
  label: Condux Weekly Summary API
  slug: condux-ai-weeklysummary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/condux-ai/openapi/condux-ai-weeklysummary-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Condux Authentication
name_suffix: Authentication
oauth_flows: []
overview: Condux declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Condux
provider_slug: condux-ai
scheme_count: 4
schemes:
- description: Each project has a DSN of the form https://<key>@ingest.condux.ai/<project>.
  in: url
  name: DSN key
  source: https://condux.ai/docs/
  type: apiKey
  use: event ingest
- description: Project-scoped token minted in the MCP tab; read-only unless minted with triage.
  name: MCP token
  prefix: condux_mcp_
  scheme: bearer
  source: https://condux.ai/integrations/mcp/
  type: http
  use: MCP endpoint https://app.condux.ai/api/mcp
- name: Release token
  source: https://raw.githubusercontent.com/tripledownab/condux/main/CHANGELOG.md
  type: other
  use: source map and debug file uploads
- description: A GitHub App with short-lived, installation-scoped tokens.
  name: GitHub App installation token
  source: https://condux.ai/integrations/github/
  type: oauth2-app
  use: Conductor fix PRs (provider-side)
slug: condux-ai-authentication
source_filename: condux-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: 'generated: ''2026-11-04''

  method: searched

  source: https://condux.ai/integrations/mcp/

  docs: https://condux.ai/docs/

  note: The OpenAPI (app.condux.ai/openapi/v1.json) declares no securitySchemes; the schemes below are what the docs and llms.txt state. The dashboard/control plane uses a sign-in session (email/password and Google OAuth sign-in on app.condux.ai), not documented as an API credential.

  schemes:

  - {name: DSN key, type: apiKey, in: url, use: event ingest, description: ''Each project has a DSN of the form https://<key>@ingest.condux.ai/<project>.'', source: https://condux.ai/docs/}

  - {name: MCP token, type: http, scheme: bearer, use: MCP endpoint https://app.condux.ai/api/mcp, prefix: condux_mcp_, description: ''Project-scoped token minted in the MCP tab; read-only unless minted with triage.'', source: https://condux.ai/integrations/mcp/}

  - {name: Release token, type: other, use: source map and debug file uploads, source: https://raw.githubusercontent.com/tripledownab/condux/main/CHANGELOG.md}

  - {name: GitHub App installation token, type: oauth2-app, use: Conductor fix PRs (provider-side), description: ''A GitHub App with short-lived, installation-scoped tokens.'', source: https://condux.ai/integrations/github/}

  '
source_yaml_url: https://artifacts.apis.io/condux-ai/authentication/condux-ai-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Error Monitoring
- Observability
- Artificial Intelligence
- Developer Tools
- OpenTelemetry
- MCP
- Self-Hosted
---
