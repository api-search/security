---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clousd-com-account-api-openapi.yml
  format: yaml
  label: Clousd Account API
  slug: clousd-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-account-api-openapi.yml
- filename: clousd-com-adb-api-openapi.yml
  format: yaml
  label: Clousd ADB API
  slug: clousd-com-adb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-adb-api-openapi.yml
- filename: clousd-com-ai-agents-api-openapi.yml
  format: yaml
  label: Clousd AI agents API
  slug: clousd-com-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-ai-agents-api-openapi.yml
- filename: clousd-com-apps-api-openapi.yml
  format: yaml
  label: Clousd Apps API
  slug: clousd-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-apps-api-openapi.yml
- filename: clousd-com-devices-api-openapi.yml
  format: yaml
  label: Clousd Devices API
  slug: clousd-com-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-devices-api-openapi.yml
- filename: clousd-com-files-and-media-api-openapi.yml
  format: yaml
  label: Clousd Files and media API
  slug: clousd-com-files-and-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-files-and-media-api-openapi.yml
- filename: clousd-com-network-api-openapi.yml
  format: yaml
  label: Clousd Network API
  slug: clousd-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-network-api-openapi.yml
- filename: clousd-com-screen-and-input-api-openapi.yml
  format: yaml
  label: Clousd Screen and input API
  slug: clousd-com-screen-and-input-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-screen-and-input-api-openapi.yml
- filename: clousd-com-tasks-api-openapi.yml
  format: yaml
  label: Clousd Tasks API
  slug: clousd-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-tasks-api-openapi.yml
- filename: clousd-com-webhooks-api-openapi.yml
  format: yaml
  label: Clousd Webhooks API
  slug: clousd-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clousd-com/openapi/clousd-com-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clousd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clousd secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Clousd
provider_slug: clousd-com
scheme_count: 2
schemes:
- header: 'Authorization: Bearer cl_live_…'
  key_prefix: cl_live_
  name: bearer
  notes: 'One key opens the REST API, the Python SDK and the MCP server. Keys are created and revoked in Settings → Connections : Access → API keys; the key is shown once. Each key has a scope (read or control) and covers all phones of the account or a chosen list; a phone outside the list answers 404. Revoking stops it at once. Keys belong to the account, not a person.'
  scheme: bearer
  sources:
  - openapi/clousd-com-openapi.yml
  - https://clousd.com/docs/api-keys/
  type: http
- applies_to: hosted MCP server https://api.clousd.com/mcp
  flow: authorizationCode
  metadata_url: https://clousd.com/.well-known/oauth-authorization-server
  name: mcp-oauth
  notes: 'Docs: "The connection is standard OAuth 2.1 with PKCE". Used by connector apps (Claude, ChatGPT, Perplexity); the user chooses "See and control" or "Only see". Not declared in the OpenAPI. A key in the URL is refused; without a header the MCP server answers 401 with the OAuth metadata.'
  pkce: true
  sources:
  - https://clousd.com/docs/mcp/
  type: oauth2
slug: clousd-com-authentication
source_filename: clousd-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clousd.com/docs/api-keys/, https://clousd.com/docs/mcp/, openapi/clousd-com-openapi.yml\ndocs: https://clousd.com/docs/api-keys/\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer cl_live_…'\n  key_prefix: cl_live_\n  sources:\n  - openapi/clousd-com-openapi.yml\n  - https://clousd.com/docs/api-keys/\n  notes: 'One key opens the REST API, the Python SDK and the MCP server. Keys are created and revoked in Settings → Connections\n    : Access → API keys; the key is shown once. Each key has a scope (read or control) and covers all phones of the account\n    or a chosen list; a phone outside the list answers 404. Revoking stops it at once. Keys belong to the account, not a person.'\n- name: mcp-oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  applies_to: hosted MCP server https://api.clousd.com/mcp\n  metadata_url: https://clousd.com/.well-known/oauth-authorization-server\n\
  \  sources:\n  - https://clousd.com/docs/mcp/\n  notes: 'Docs: \"The connection is standard OAuth 2.1 with PKCE\". Used by connector apps (Claude, ChatGPT, Perplexity); the\n    user chooses \"See and control\" or \"Only see\". Not declared in the OpenAPI. A key in the URL is refused; without a header\n    the MCP server answers 401 with the OAuth metadata.'\n"
source_yaml_url: https://artifacts.apis.io/clousd-com/authentication/clousd-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Android
- Cloud Phones
- AI Agents
- MCP
- Mobile Testing
- QA
- Emulators
---
