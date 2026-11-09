---
anonymous_access: true
api_key_in: []
api_specs:
- filename: anahana-com-discovery-api-openapi.yml
  format: yaml
  label: Anahana Discovery API
  slug: anahana-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-discovery-api-openapi.yml
- filename: anahana-com-mcp-api-openapi.yml
  format: yaml
  label: Anahana MCP API
  slug: anahana-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-mcp-api-openapi.yml
- filename: anahana-com-oauth-api-openapi.yml
  format: yaml
  label: Anahana OAuth API
  slug: anahana-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-oauth-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Anahana Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anahana declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Anahana
provider_slug: anahana-com
scheme_count: 2
schemes:
- description: Anonymous access, no credentials required for public content.
  rate_limit:
    limit: 30
    scope: ip
    window: minute
  type: none
- description: OAuth 2.1 Authorization Code with PKCE for registered clients.
  flows:
    authorizationCode:
      authorizationUrl: https://www.anahana.com/mcp/authorize
      scopes: {}
      tokenUrl: https://www.anahana.com/mcp/token
  rate_limit:
    limit: 120
    scope: client
    window: minute
  registration:
    url: https://www.anahana.com/mcp/register
  type: oauth2
slug: anahana-com-authentication
source_filename: anahana-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://www.anahana.com/auth.md\nschemes:\n  - type: none\n    description: Anonymous access, no credentials required for public content.\n    rate_limit:\n      limit: 30\n      window: minute\n      scope: ip\n  - type: oauth2\n    description: OAuth 2.1 Authorization Code with PKCE for registered clients.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://www.anahana.com/mcp/authorize\n        tokenUrl: https://www.anahana.com/mcp/token\n        scopes: {}\n    registration:\n      url: https://www.anahana.com/mcp/register\n    rate_limit:\n      limit: 120\n      window: minute\n      scope: client\n"
source_yaml_url: https://artifacts.apis.io/anahana-com/authentication/anahana-com-authentication.yml
summary_line: 2 schemes
tags:
- SpiritualWellness
- Personal Growth
- Astrology
- Meditation
- Yoga
---
