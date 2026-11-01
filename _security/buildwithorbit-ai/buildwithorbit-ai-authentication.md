---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buildwithorbit-ai-integrate-api-openapi.yml
  format: yaml
  label: buildwithorbit-ai Integrate API
  slug: buildwithorbit-ai-integrate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildwithorbit-ai/openapi/buildwithorbit-ai-integrate-api-openapi.yml
- filename: buildwithorbit-ai-search-api-openapi.yml
  format: yaml
  label: buildwithorbit-ai Search API
  slug: buildwithorbit-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildwithorbit-ai/openapi/buildwithorbit-ai-search-api-openapi.yml
auth_types: []
description: Authentication methods for the Orbit integration endpoints as described in the task brief.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Buildwithorbit Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: buildwithorbit-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: buildwithorbit-ai
provider_slug: buildwithorbit-ai
scheme_count: 2
schemes:
- evidence: 'OpenWeatherMap: API key supplied as the required `appid` query parameter; replace `YOUR_API_KEY` with the actual key.'
  location: query
  name: OpenWeatherMap
  type: apiKey
- evidence: 'Slack: bot token supplied in the `token` form field/header value as `{{bot_token}}`, requiring the `chat:write` scope.'
  header: token
  location: header
  name: Slack
  scopes:
  - chat:write
  type: apiKey
slug: buildwithorbit-ai-authentication
source_filename: buildwithorbit-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.buildwithorbit.ai/docs/get-started/quickstart-guide.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.buildwithorbit.ai/docs/get-started/quickstart-guide.md\nsources:\n- https://docs.buildwithorbit.ai/docs/get-started/quickstart-guide.md\n- https://www.buildwithorbit.ai/docs/get-started/quickstart-guide\ndescription: Authentication methods for the Orbit integration endpoints as described in the task brief.\nschemes:\n- type: apiKey\n  name: OpenWeatherMap\n  evidence: 'OpenWeatherMap: API key supplied as the required `appid` query parameter; replace `YOUR_API_KEY` with the actual key.'\n  location: query\n- type: apiKey\n  name: Slack\n  evidence: 'Slack: bot token supplied in the `token` form field/header value as `{{bot_token}}`, requiring the `chat:write` scope.'\n  location: header\n  header: token\n  scopes:\n  - chat:write\ndocs: https://docs.buildwithorbit.ai/docs/get-started/quickstart-guide.md\n"
source_yaml_url: https://artifacts.apis.io/buildwithorbit-ai/authentication/buildwithorbit-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI
- API-Discovery
- Integration
- MCP
- Postman
- Platform
---
