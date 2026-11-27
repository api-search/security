---
anonymous_access: false
api_key_in: []
api_specs:
- filename: userintuition-ai-public-account-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Account API
  slug: userintuition-ai-public-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-account-api-openapi.yml
- filename: userintuition-ai-public-exports-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Exports API
  slug: userintuition-ai-public-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-exports-api-openapi.yml
- filename: userintuition-ai-public-external-panels-api-openapi.yml
  format: yaml
  label: userintuition-ai Public External Panels API
  slug: userintuition-ai-public-external-panels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-external-panels-api-openapi.yml
- filename: userintuition-ai-public-feasibility-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Feasibility API
  slug: userintuition-ai-public-feasibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-feasibility-api-openapi.yml
- filename: userintuition-ai-public-intelligence-hub-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Intelligence Hub API
  slug: userintuition-ai-public-intelligence-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-intelligence-hub-api-openapi.yml
- filename: userintuition-ai-public-interviews-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Interviews API
  slug: userintuition-ai-public-interviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-interviews-api-openapi.yml
- filename: userintuition-ai-public-observers-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Observers API
  slug: userintuition-ai-public-observers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-observers-api-openapi.yml
- filename: userintuition-ai-public-organizations-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Organizations API
  slug: userintuition-ai-public-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-organizations-api-openapi.yml
- filename: userintuition-ai-public-panel-countries-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Panel Countries API
  slug: userintuition-ai-public-panel-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-panel-countries-api-openapi.yml
- filename: userintuition-ai-public-participants-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Participants API
  slug: userintuition-ai-public-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-participants-api-openapi.yml
- filename: userintuition-ai-public-reference-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Reference API
  slug: userintuition-ai-public-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-reference-api-openapi.yml
- filename: userintuition-ai-public-research-search-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Research Search API
  slug: userintuition-ai-public-research-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-research-search-api-openapi.yml
- filename: userintuition-ai-public-studies-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Studies API
  slug: userintuition-ai-public-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-studies-api-openapi.yml
- filename: userintuition-ai-public-targeting-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Targeting API
  slug: userintuition-ai-public-targeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-targeting-api-openapi.yml
- filename: userintuition-ai-public-usage-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Usage API
  slug: userintuition-ai-public-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-usage-api-openapi.yml
- filename: userintuition-ai-public-webhooks-api-openapi.yml
  format: yaml
  label: userintuition-ai Public Webhooks API
  slug: userintuition-ai-public-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userintuition-ai/openapi/userintuition-ai-public-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: userintuition-ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: userintuition-ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: userintuition-ai
provider_slug: userintuition-ai
scheme_count: 2
schemes:
- evidence: Use hosted OAuth or an organization API key, including with headless hosted clients.
  header: Authorization
  how_to_obtain: Complete the hosted OAuth authorization flow as described on the authentication page.
  location: header
  name: Hosted OAuth
  type: http-bearer
- evidence: 'Headless clients can instead send an organization API key to the same hosted endpoint in an Authorization: Bearer ui_sk_… header.'
  header: Authorization
  how_to_obtain: Create an API key under Settings → API Keys; keys start with ui_sk_.
  location: header
  name: API Key
  type: http-bearer
slug: userintuition-ai-authentication
source_filename: userintuition-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.userintuition.ai/mcp-server/authentication
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.userintuition.ai/mcp-server/authentication\nsources:\n- https://docs.userintuition.ai/mcp-server/authentication\n- https://docs.userintuition.ai/api-reference/public-external-panels/regenerate-study-external-panel-token\n- https://docs.userintuition.ai/api-reference/staging-quickstart\n- https://docs.userintuition.ai/mcp-server/quickstart\nschemes:\n- type: http-bearer\n  name: Hosted OAuth\n  evidence: Use hosted OAuth or an organization API key, including with headless hosted clients.\n  location: header\n  header: Authorization\n  how_to_obtain: Complete the hosted OAuth authorization flow as described on the authentication page.\n- type: http-bearer\n  name: API Key\n  evidence: 'Headless clients can instead send an organization API key to the same hosted endpoint in an Authorization: Bearer ui_sk_… header.'\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Create an API key under Settings → API Keys; keys start with ui_sk_.\ndocs: https://docs.userintuition.ai/mcp-server/authentication\n"
source_yaml_url: https://artifacts.apis.io/userintuition-ai/authentication/userintuition-ai-authentication.yml
summary_line: 2 schemes
tags:
- Qualitative Research
- AI Moderation
- Customer Insights
- Research Platforms
- Panel Recruitment
---
