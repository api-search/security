---
api_key_in:
- header
api_specs:
- filename: archastro-activity-feed-api-openapi.yml
  format: yaml
  label: Archastro Activity Feed API
  slug: archastro-activity-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-activity-feed-api-openapi.yml
- filename: archastro-agents-api-openapi.yml
  format: yaml
  label: Archastro Agents API
  slug: archastro-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-agents-api-openapi.yml
- filename: archastro-auth-api-openapi.yml
  format: yaml
  label: Archastro auth API
  slug: archastro-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-auth-api-openapi.yml
- filename: archastro-files-api-openapi.yml
  format: yaml
  label: Archastro Files API
  slug: archastro-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-files-api-openapi.yml
- filename: archastro-oauth-api-openapi.yml
  format: yaml
  label: Archastro Oauth API
  slug: archastro-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-oauth-api-openapi.yml
- filename: archastro-s2s-api-openapi.yml
  format: yaml
  label: Archastro s2s API
  slug: archastro-s2s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-s2s-api-openapi.yml
- filename: archastro-slack-channel-bindings-api-openapi.yml
  format: yaml
  label: Archastro Slack Channel Bindings API
  slug: archastro-slack-channel-bindings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-slack-channel-bindings-api-openapi.yml
- filename: archastro-teams-api-openapi.yml
  format: yaml
  label: Archastro Teams API
  slug: archastro-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-teams-api-openapi.yml
- filename: archastro-threads-api-openapi.yml
  format: yaml
  label: Archastro Threads API
  slug: archastro-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-threads-api-openapi.yml
- filename: archastro-users-api-openapi.yml
  format: yaml
  label: Archastro Users API
  slug: archastro-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/openapi/archastro-users-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Archastro Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Archastro secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Archastro
provider_slug: archastro
scheme_count: 3
schemes:
- description: Session/access token bearer auth; also used by realtime channels.
  format: 'Authorization: Bearer $ARCHASTRO_ACCESS_TOKEN'
  header: Authorization
  in: header
  name: bearerToken
  scheme: bearer
  type: http
- description: Publishable API key for client-side calls; sandbox vs production keys select the workspace.
  format: 'x-archastro-api-key: $ARCHASTRO_PUBLISHABLE_KEY'
  in: header
  name: publishableKey
  parameter: x-archastro-api-key
  type: apiKey
- description: OAuth 2.0 Device Authorization flow for CLI / coding-agent login. GET /oauth/scopes lists available scopes (requires authentication); scope values are not published in the docs.
  endpoints:
    approve: /oauth/device/approve
    authorize: /oauth/device/authorize
    deny: /oauth/device/deny
    scopes: /oauth/scopes
    token: /oauth/token
  flow: deviceCode
  name: oauthDevice
  type: oauth2
slug: archastro-authentication
source_filename: archastro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.archastro.ai/docs/api-reference\ndocs: https://docs.archastro.ai/docs/api-reference\nnote: >-\n  The published openapi.json declares no components.securitySchemes, so this profile\n  is captured from the API reference documentation rather than derived from the spec.\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [deviceCode]\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Authorization: Bearer $ARCHASTRO_ACCESS_TOKEN\"\n  description: Session/access token bearer auth; also used by realtime channels.\n- name: publishableKey\n  type: apiKey\n  in: header\n  parameter: x-archastro-api-key\n  format: \"x-archastro-api-key: $ARCHASTRO_PUBLISHABLE_KEY\"\n  description: Publishable API key for client-side calls; sandbox vs production keys select the workspace.\n- name: oauthDevice\n  type: oauth2\n  flow: deviceCode\n\
  \  endpoints:\n    authorize: /oauth/device/authorize\n    approve: /oauth/device/approve\n    deny: /oauth/device/deny\n    token: /oauth/token\n    scopes: /oauth/scopes\n  description: >-\n    OAuth 2.0 Device Authorization flow for CLI / coding-agent login. GET /oauth/scopes\n    lists available scopes (requires authentication); scope values are not published in the docs.\nkey_separation:\n  secret_keys: server-side setup (sandbox secret keys never access production)\n  publishable_keys: client-side work (sandbox publishable keys)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archastro/refs/heads/main/authentication/archastro-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Company
- AI Agents
- Agentic
- Developer Platform
- Automation
- Integration
- MCP
- Workflows
---
