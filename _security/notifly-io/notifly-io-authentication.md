---
anonymous_access: false
api_key_in: []
api_specs:
- filename: notifly-io-agents-api-openapi.yml
  format: yaml
  label: Notifly Agents API
  slug: notifly-io-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-agents-api-openapi.yml
- filename: notifly-io-channel-connections-api-openapi.yml
  format: yaml
  label: Notifly Channel Connections API
  slug: notifly-io-channel-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-channel-connections-api-openapi.yml
- filename: notifly-io-channel-endpoints-api-openapi.yml
  format: yaml
  label: Notifly Channel Endpoints API
  slug: notifly-io-channel-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-channel-endpoints-api-openapi.yml
- filename: notifly-io-contexts-api-openapi.yml
  format: yaml
  label: Notifly Contexts API
  slug: notifly-io-contexts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-contexts-api-openapi.yml
- filename: notifly-io-environment-variables-api-openapi.yml
  format: yaml
  label: Notifly Environment Variables API
  slug: notifly-io-environment-variables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-environment-variables-api-openapi.yml
- filename: notifly-io-environments-api-openapi.yml
  format: yaml
  label: Notifly Environments API
  slug: notifly-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-environments-api-openapi.yml
- filename: notifly-io-events-api-openapi.yml
  format: yaml
  label: Notifly Events API
  slug: notifly-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-events-api-openapi.yml
- filename: notifly-io-integrations-api-openapi.yml
  format: yaml
  label: Notifly Integrations API
  slug: notifly-io-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-integrations-api-openapi.yml
- filename: notifly-io-layouts-api-openapi.yml
  format: yaml
  label: Notifly Layouts API
  slug: notifly-io-layouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-layouts-api-openapi.yml
- filename: notifly-io-messages-api-openapi.yml
  format: yaml
  label: Notifly Messages API
  slug: notifly-io-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-messages-api-openapi.yml
- filename: notifly-io-notifications-api-openapi.yml
  format: yaml
  label: Notifly Notifications API
  slug: notifly-io-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-notifications-api-openapi.yml
- filename: notifly-io-subscribers-api-openapi.yml
  format: yaml
  label: Notifly Subscribers API
  slug: notifly-io-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-subscribers-api-openapi.yml
- filename: notifly-io-topics-api-openapi.yml
  format: yaml
  label: Notifly Topics API
  slug: notifly-io-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-topics-api-openapi.yml
- filename: notifly-io-webhooks-api-openapi.yml
  format: yaml
  label: Notifly Webhooks API
  slug: notifly-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-webhooks-api-openapi.yml
- filename: notifly-io-workflows-api-openapi.yml
  format: yaml
  label: Notifly Workflows API
  slug: notifly-io-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notifly-io/openapi/notifly-io-workflows-api-openapi.yml
auth_types: []
description: Authentication methods published for Notifly
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Notifly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notifly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Notifly
provider_slug: notifly-io
scheme_count: 2
schemes:
- evidence: 'Authenticate every request with the ApiKey scheme in the Authorization header:'
  header: Authorization
  how_to_obtain: Get an API key from the Notifly dashboard under API Keys; keys are environment‑scoped secrets.
  location: header
  name: ApiKey
  type: apiKey
- evidence: 'Auth: OAuth 2.1, built into the platform — clients sign in with a standard OAuth flow (including dynamic client registration), so there is no API-key pasting.'
  how_to_obtain: Clients sign in via the Notifly MCP server (https://api.notifly.io/mcp) using the standard OAuth 2.1 flow; dynamic client registration is performed by the platform.
  name: OAuth 2.1
  type: oauth2
slug: notifly-io-authentication
source_filename: notifly-io-authentication.yml
source_heading: Authentication Profile
source_url: https://notifly.io/docs/getting-started
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://notifly.io/docs/getting-started\nsources:\n- https://notifly.io/docs/getting-started\n- https://notifly.io/docs/api\n- https://notifly.io/docs/connecting-ai-assistants\n- https://notifly.io/docs/http-request-signing\ndescription: Authentication methods published for Notifly\nschemes:\n- type: apiKey\n  name: ApiKey\n  evidence: 'Authenticate every request with the ApiKey scheme in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Get an API key from the Notifly dashboard under API Keys; keys are environment‑scoped secrets.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'Auth: OAuth 2.1, built into the platform — clients sign in with a standard OAuth flow (including dynamic client registration), so\n    there is no API-key pasting.'\n  how_to_obtain: Clients sign in via the Notifly MCP server (https://api.notifly.io/mcp) using the\
  \ standard OAuth 2.1 flow; dynamic client registration\n    is performed by the platform.\ndocs: https://notifly.io/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/notifly-io/authentication/notifly-io-authentication.yml
summary_line: 2 schemes
tags:
- Notification
- Messaging
- Multi-Channel
- Software-as-a-Service
---
