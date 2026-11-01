---
anonymous_access: false
api_key_in: []
api_specs:
- filename: communicate-so-account-credentials-api-openapi.yml
  format: yaml
  label: communicate-so Account credentials API
  slug: communicate-so-account-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-account-credentials-api-openapi.yml
- filename: communicate-so-account-preferences-api-openapi.yml
  format: yaml
  label: communicate-so Account preferences API
  slug: communicate-so-account-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-account-preferences-api-openapi.yml
- filename: communicate-so-agents-api-openapi.yml
  format: yaml
  label: communicate-so Agents API
  slug: communicate-so-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-agents-api-openapi.yml
- filename: communicate-so-authentication-api-openapi.yml
  format: yaml
  label: communicate-so Authentication API
  slug: communicate-so-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-authentication-api-openapi.yml
- filename: communicate-so-chat-api-openapi.yml
  format: yaml
  label: communicate-so Chat API
  slug: communicate-so-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-chat-api-openapi.yml
- filename: communicate-so-discovery-api-openapi.yml
  format: yaml
  label: communicate-so Discovery API
  slug: communicate-so-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-discovery-api-openapi.yml
- filename: communicate-so-grill-api-openapi.yml
  format: yaml
  label: communicate-so Grill API
  slug: communicate-so-grill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-grill-api-openapi.yml
- filename: communicate-so-inbox-api-openapi.yml
  format: yaml
  label: communicate-so Inbox API
  slug: communicate-so-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-inbox-api-openapi.yml
- filename: communicate-so-learnings-api-openapi.yml
  format: yaml
  label: communicate-so Learnings API
  slug: communicate-so-learnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-learnings-api-openapi.yml
- filename: communicate-so-notifications-api-openapi.yml
  format: yaml
  label: communicate-so Notifications API
  slug: communicate-so-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-notifications-api-openapi.yml
- filename: communicate-so-sources-api-openapi.yml
  format: yaml
  label: communicate-so Sources API
  slug: communicate-so-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-sources-api-openapi.yml
- filename: communicate-so-teams-api-openapi.yml
  format: yaml
  label: communicate-so Teams API
  slug: communicate-so-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-teams-api-openapi.yml
- filename: communicate-so-workspace-members-api-openapi.yml
  format: yaml
  label: communicate-so Workspace members API
  slug: communicate-so-workspace-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-workspace-members-api-openapi.yml
- filename: communicate-so-workspaces-api-openapi.yml
  format: yaml
  label: communicate-so Workspaces API
  slug: communicate-so-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/communicate-so/openapi/communicate-so-workspaces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Communicate So Authentication
name_suffix: Authentication
oauth_flows: []
overview: communicate-so declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: communicate-so
provider_slug: communicate-so
scheme_count: 2
schemes:
- flow: client_credentials
  scopes:
    agents:read: List agents in the workspace
    chat:write: Send chat turns to workspace agents
  tokenUrl: https://app.communicate.so/api/v1/oauth/token
  type: oauth2
- description: Workspace API key prefixed with ck_ used as Bearer token
  in: header
  name: Authorization
  type: apiKey
slug: communicate-so-authentication
source_filename: communicate-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://developer.communicate.so/docs/authentication.md\nschemes:\n  - type: oauth2\n    flow: client_credentials\n    tokenUrl: https://app.communicate.so/api/v1/oauth/token\n    scopes:\n      agents:read: List agents in the workspace\n      chat:write: Send chat turns to workspace agents\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Workspace API key prefixed with ck_ used as Bearer token\n"
source_yaml_url: https://artifacts.apis.io/communicate-so/authentication/communicate-so-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Customer Support
- Chatbot
- SaaS
- Automation
---
