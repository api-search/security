---
anonymous_access: false
api_key_in: []
api_specs:
- filename: asoskill-com-authentication-api-openapi.yml
  format: yaml
  label: asoskill-com Authentication API
  slug: asoskill-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-authentication-api-openapi.yml
- filename: asoskill-com-billing-api-openapi.yml
  format: yaml
  label: asoskill-com Billing API
  slug: asoskill-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-billing-api-openapi.yml
- filename: asoskill-com-credits-api-openapi.yml
  format: yaml
  label: asoskill-com Credits API
  slug: asoskill-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-credits-api-openapi.yml
- filename: asoskill-com-data-api-openapi.yml
  format: yaml
  label: asoskill-com Data API
  slug: asoskill-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-data-api-openapi.yml
- filename: asoskill-com-mcp-api-openapi.yml
  format: yaml
  label: asoskill-com MCP API
  slug: asoskill-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-mcp-api-openapi.yml
- filename: asoskill-com-operations-api-openapi.yml
  format: yaml
  label: asoskill-com Operations API
  slug: asoskill-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asoskill-com/openapi/asoskill-com-operations-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Asoskill Com Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: asoskill-com secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: asoskill-com
provider_slug: asoskill-com
scheme_count: 2
schemes:
- bearerFormat: aso_live_...
  description: 'Long-lived secret created in the ASO Skill developer dashboard. Send it as `Authorization: Bearer <key>` and keep it on the server.'
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/asoskill-com-openapi.yaml
  type: http
- description: OAuth authorization code with S256 PKCE, dynamic client registration, exact MCP resource binding, refresh rotation, and revocation.
  flows:
  - authorizationUrl: https://api.asoskill.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.asoskill.com/oauth/token
  name: mcpOAuth
  sources:
  - openapi/asoskill-com-openapi.yaml
  type: oauth2
slug: asoskill-com-authentication
source_filename: asoskill-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/asoskill-com-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: aso_live_...\n  description: 'Long-lived secret created in the ASO Skill developer dashboard. Send it as `Authorization:\n    Bearer <key>` and keep it on the server.'\n  sources:\n  - openapi/asoskill-com-openapi.yaml\n- name: mcpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.asoskill.com/oauth/authorize\n    tokenUrl: https://api.asoskill.com/oauth/token\n    scopes: 2\n  description: OAuth authorization code with S256 PKCE, dynamic client registration, exact MCP\n    resource binding, refresh rotation, and revocation.\n  sources:\n  - openapi/asoskill-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/asoskill-com/authentication/asoskill-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- ASO
- AppStore
- API
- Data
---
