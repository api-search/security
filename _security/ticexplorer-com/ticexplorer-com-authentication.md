---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ticexplorer-com-admin-api-openapi.yml
  format: yaml
  label: ticexplorer-com Admin API
  slug: ticexplorer-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-admin-api-openapi.yml
- filename: ticexplorer-com-analytics-api-openapi.yml
  format: yaml
  label: ticexplorer-com Analytics API
  slug: ticexplorer-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-analytics-api-openapi.yml
- filename: ticexplorer-com-claims-api-openapi.yml
  format: yaml
  label: ticexplorer-com Claims API
  slug: ticexplorer-com-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-claims-api-openapi.yml
- filename: ticexplorer-com-codes-api-openapi.yml
  format: yaml
  label: ticexplorer-com Codes API
  slug: ticexplorer-com-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-codes-api-openapi.yml
- filename: ticexplorer-com-guide-api-openapi.yml
  format: yaml
  label: ticexplorer-com Guide API
  slug: ticexplorer-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-guide-api-openapi.yml
- filename: ticexplorer-com-plans-api-openapi.yml
  format: yaml
  label: ticexplorer-com Plans API
  slug: ticexplorer-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-plans-api-openapi.yml
- filename: ticexplorer-com-providers-api-openapi.yml
  format: yaml
  label: ticexplorer-com Providers API
  slug: ticexplorer-com-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-providers-api-openapi.yml
- filename: ticexplorer-com-rates-api-openapi.yml
  format: yaml
  label: ticexplorer-com Rates API
  slug: ticexplorer-com-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ticexplorer-com/openapi/ticexplorer-com-rates-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ticexplorer Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ticexplorer-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ticexplorer-com
provider_slug: ticexplorer-com
scheme_count: 2
schemes:
- description: API key (tic_live_...) or OAuth access token.
  name: HTTPBearer
  scheme: bearer
  type: http
- description: OAuth 2.1 (authorization code + PKCE) for MCP clients; see /.well-known/oauth-authorization-server
  flows:
    authorizationCode:
      authorizationUrl: /authorize
      scopes:
        read: Query prices
      tokenUrl: /token
  type: oauth2
slug: ticexplorer-com-authentication
source_filename: ticexplorer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: \"https://api.ticexplorer.com/openapi.json\"\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"API key (tic_live_...) or OAuth access token.\"\n    name: HTTPBearer\n  - type: oauth2\n    description: \"OAuth 2.1 (authorization code + PKCE) for MCP clients; see /.well-known/oauth-authorization-server\"\n    flows:\n      authorizationCode:\n        authorizationUrl: \"/authorize\"\n        tokenUrl: \"/token\"\n        scopes:\n          read: \"Query prices\"\n"
source_yaml_url: https://artifacts.apis.io/ticexplorer-com/authentication/ticexplorer-com-authentication.yml
summary_line: 2 schemes
tags:
- Health
- Finance
- API
- Transparency
- Healthcare
---
