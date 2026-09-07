---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: apicontext-platform-openapi.yml
  format: yaml
  label: APIContext Platform API
  slug: apicontext-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-platform-openapi.yml
- filename: apicontext-api-calls-api-openapi.yml
  format: yaml
  label: APIContext Calls API
  slug: apicontext-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-api-calls-api-openapi.yml
- filename: apicontext-schedules-api-openapi.yml
  format: yaml
  label: APIContext Schedules API
  slug: apicontext-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-schedules-api-openapi.yml
- filename: apicontext-webhooks-openapi.yml
  format: yaml
  label: APIContext Webhooks API
  slug: apicontext-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-webhooks-openapi.yml
- filename: apicontext-workflows-api-openapi.yml
  format: yaml
  label: APIContext Workflows API
  slug: apicontext-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-workflows-api-openapi.yml
- filename: apicontext-governance-openapi.yml
  format: yaml
  label: APIContext Governance API
  slug: apicontext-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-governance-openapi.yml
- filename: apicontext-statistics-api-openapi.yml
  format: yaml
  label: APIContext Stats API
  slug: apicontext-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-statistics-api-openapi.yml
- filename: apicontext-results-api-openapi.yml
  format: yaml
  label: APIContext Results API
  slug: apicontext-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-results-api-openapi.yml
- filename: apicontext-agents-api-openapi.yml
  format: yaml
  label: APIContext Agents API
  slug: apicontext-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-agents-api-openapi.yml
- filename: apicontext-projects-api-openapi.yml
  format: yaml
  label: APIContext Projects API
  slug: apicontext-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-projects-api-openapi.yml
- filename: apicontext-insights-api-openapi.yml
  format: yaml
  label: APIContext Insights API
  slug: apicontext-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-insights-api-openapi.yml
- filename: apicontext-tokens-api-openapi.yml
  format: yaml
  label: APIContext Auth Tokens API
  slug: apicontext-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-tokens-api-openapi.yml
- filename: apicontext-mcp-monitors-openapi.yml
  format: yaml
  label: APIContext MCP Monitors API
  slug: apicontext-mcp-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-mcp-monitors-openapi.yml
- filename: apicontext-reports-api-openapi.yml
  format: yaml
  label: APIContext Reports API
  slug: apicontext-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-reports-api-openapi.yml
- filename: apicontext-alerts-api-openapi.yml
  format: yaml
  label: APIContext Notifications API
  slug: apicontext-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-alerts-api-openapi.yml
- filename: apicontext-directory-api-openapi.yml
  format: yaml
  label: APIContext Suppliers API
  slug: apicontext-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/openapi/apicontext-directory-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Apicontext Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: APIContext secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: APIContext
provider_slug: apicontext
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://auth.apimetrics.io/authorize?audience=https://client.apimetrics.io
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://auth.apimetrics.io/oauth/token
  name: OAuth2
  sources:
  - openapi/apicontext-agents-api-openapi.yml
  - openapi/apicontext-alerts-api-openapi.yml
  - openapi/apicontext-api-calls-api-openapi.yml
  - openapi/apicontext-directory-api-openapi.yml
  - openapi/apicontext-governance-openapi.yml
  - openapi/apicontext-insights-api-openapi.yml
  - openapi/apicontext-mcp-monitors-openapi.yml
  - openapi/apicontext-platform-openapi.yml
  - openapi/apicontext-projects-api-openapi.yml
  - openapi/apicontext-reports-api-openapi.yml
  - openapi/apicontext-results-api-openapi.yml
  - openapi/apicontext-schedules-api-openapi.yml
  - openapi/apicontext-statistics-api-openapi.yml
  - openapi/apicontext-tokens-api-openapi.yml
  - openapi/apicontext-webhooks-openapi.yml
  - openapi/apicontext-workflows-api-openapi.yml
  type: oauth2
- in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - openapi/apicontext-agents-api-openapi.yml
  - openapi/apicontext-alerts-api-openapi.yml
  - openapi/apicontext-api-calls-api-openapi.yml
  - openapi/apicontext-directory-api-openapi.yml
  - openapi/apicontext-governance-openapi.yml
  - openapi/apicontext-insights-api-openapi.yml
  - openapi/apicontext-mcp-monitors-openapi.yml
  - openapi/apicontext-platform-openapi.yml
  - openapi/apicontext-projects-api-openapi.yml
  - openapi/apicontext-reports-api-openapi.yml
  - openapi/apicontext-results-api-openapi.yml
  - openapi/apicontext-schedules-api-openapi.yml
  - openapi/apicontext-statistics-api-openapi.yml
  - openapi/apicontext-tokens-api-openapi.yml
  - openapi/apicontext-webhooks-openapi.yml
  - openapi/apicontext-workflows-api-openapi.yml
  type: apiKey
slug: apicontext-authentication
source_filename: apicontext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/apicontext-agents-api-openapi.yml, openapi/apicontext-alerts-api-openapi.yml,\n  openapi/apicontext-api-calls-api-openapi.yml, openapi/apicontext-directory-api-openapi.yml,\n  openapi/apicontext-governance-openapi.yml, openapi/apicontext-insights-api-openapi.yml, openapi/apicontext-mcp-monitors-openapi.yml,\n  openapi/apicontext-platform-openapi.yml, openapi/apicontext-projects-api-openapi.yml, openapi/apicontext-reports-api-openapi.yml,\n  openapi/apicontext-results-api-openapi.yml, openapi/apicontext-schedules-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.apimetrics.io/authorize?audience=https://client.apimetrics.io\n    tokenUrl: https://auth.apimetrics.io/oauth/token\n    scopes: 3\n  sources:\n  - openapi/apicontext-agents-api-openapi.yml\n\
  \  - openapi/apicontext-alerts-api-openapi.yml\n  - openapi/apicontext-api-calls-api-openapi.yml\n  - openapi/apicontext-directory-api-openapi.yml\n  - openapi/apicontext-governance-openapi.yml\n  - openapi/apicontext-insights-api-openapi.yml\n  - openapi/apicontext-mcp-monitors-openapi.yml\n  - openapi/apicontext-platform-openapi.yml\n  - openapi/apicontext-projects-api-openapi.yml\n  - openapi/apicontext-reports-api-openapi.yml\n  - openapi/apicontext-results-api-openapi.yml\n  - openapi/apicontext-schedules-api-openapi.yml\n  - openapi/apicontext-statistics-api-openapi.yml\n  - openapi/apicontext-tokens-api-openapi.yml\n  - openapi/apicontext-webhooks-openapi.yml\n  - openapi/apicontext-workflows-api-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/apicontext-agents-api-openapi.yml\n  - openapi/apicontext-alerts-api-openapi.yml\n  - openapi/apicontext-api-calls-api-openapi.yml\n  - openapi/apicontext-directory-api-openapi.yml\n\
  \  - openapi/apicontext-governance-openapi.yml\n  - openapi/apicontext-insights-api-openapi.yml\n  - openapi/apicontext-mcp-monitors-openapi.yml\n  - openapi/apicontext-platform-openapi.yml\n  - openapi/apicontext-projects-api-openapi.yml\n  - openapi/apicontext-reports-api-openapi.yml\n  - openapi/apicontext-results-api-openapi.yml\n  - openapi/apicontext-schedules-api-openapi.yml\n  - openapi/apicontext-statistics-api-openapi.yml\n  - openapi/apicontext-tokens-api-openapi.yml\n  - openapi/apicontext-webhooks-openapi.yml\n  - openapi/apicontext-workflows-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicontext/refs/heads/main/authentication/apicontext-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- API Directory
- API Monitoring
- Agent Skills
- Conformance
- MCP Monitoring
- Observability
- OpenTelemetry
- Performance
- Platform
- SLO
- Synthetic Testing
- Testing
---
