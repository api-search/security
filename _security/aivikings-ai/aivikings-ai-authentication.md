---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aivikings-ai-prices-api-openapi.yml
  format: yaml
  label: AiVikings.ai Prices API
  slug: aivikings-ai-prices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivikings-ai/openapi/aivikings-ai-prices-api-openapi.yml
- filename: aivikings-ai-pricing-api-openapi.yml
  format: yaml
  label: AiVikings.ai Pricing API
  slug: aivikings-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivikings-ai/openapi/aivikings-ai-pricing-api-openapi.yml
- filename: aivikings-ai-quote-api-openapi.yml
  format: yaml
  label: AiVikings.ai Quote API
  slug: aivikings-ai-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivikings-ai/openapi/aivikings-ai-quote-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AiVikings.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: AiVikings.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AiVikings.ai
provider_slug: aivikings-ai
scheme_count: 2
schemes:
- description: 'Customer bearer token for API calls, sent as Authorization: Bearer <token>'
  scheme: bearer
  type: http
- description: OAuth2 flow for user-authorized access to domain operations.
  flows:
    authorizationCode:
      authorizationUrl: https://api.aivikings.ai/oauth/authorize
      scopes:
        read: Read access to domain data
        write: Write access to domain registrations
      tokenUrl: https://api.aivikings.ai/oauth/token
  type: oauth2
slug: aivikings-ai-authentication
source_filename: aivikings-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://aivikings.ai/docs/authentication/\nname: AiVikings.ai authentication\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Customer bearer token for API calls, sent as Authorization: Bearer <token>\"\n  - type: oauth2\n    description: \"OAuth2 flow for user-authorized access to domain operations.\"\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://api.aivikings.ai/oauth/authorize\"\n        tokenUrl: \"https://api.aivikings.ai/oauth/token\"\n        scopes:\n          read: \"Read access to domain data\"\n          write: \"Write access to domain registrations\"\n"
source_yaml_url: https://artifacts.apis.io/aivikings-ai/authentication/aivikings-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Domain Registrar
- MCP
- REST API
- DNS
- Automation
---
