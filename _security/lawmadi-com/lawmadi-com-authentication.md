---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lawmadi-com-agent-discovery-api-openapi.yml
  format: yaml
  label: Lawmadi Agent discovery API
  slug: lawmadi-com-agent-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-agent-discovery-api-openapi.yml
- filename: lawmadi-com-ask-api-openapi.yml
  format: yaml
  label: Lawmadi Ask API
  slug: lawmadi-com-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-ask-api-openapi.yml
- filename: lawmadi-com-ask-stream-api-openapi.yml
  format: yaml
  label: Lawmadi Ask Stream API
  slug: lawmadi-com-ask-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-ask-stream-api-openapi.yml
- filename: lawmadi-com-pricing-api-openapi.yml
  format: yaml
  label: Lawmadi Pricing API
  slug: lawmadi-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lawmadi-com/openapi/lawmadi-com-pricing-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Lawmadi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lawmadi secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lawmadi
provider_slug: lawmadi-com
scheme_count: 2
schemes:
- description: 'Customer API key — `Authorization: Bearer lmk_live_…`. Issue one after email sign-in at https://lawmadi.com/mcp-key-guide-en, or obtain one through the OAuth flow below (an OAuth access token IS such a key, so quotas and billing behave identically). Costs are not duplicated here: GET /plans returns the current pricing as JSON, and the MCP tool `get_pricing` needs no auth.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/lawmadi-com-openapi.json
  type: http
- description: 'Authorization code + PKCE (S256 only). Dynamic client registration is open (RFC 7591). Scope `mcp:read` cannot spend the user''s credits. Server metadata: https://lawmadi.com/.well-known/oauth-authorization-server (RFC 8414); protected resource metadata: https://lawmadi.com/mcp/.well-known/oauth-protected-resource (RFC 9728).'
  flows:
  - authorizationUrl: https://lawmadi.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://lawmadi.com/oauth/token
  name: oauth2
  sources:
  - openapi/lawmadi-com-openapi.json
  type: oauth2
slug: lawmadi-com-authentication
source_filename: lawmadi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lawmadi-com-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Customer API key — `Authorization: Bearer lmk_live_…`. Issue one after email\n    sign-in at https://lawmadi.com/mcp-key-guide-en, or obtain one through the OAuth flow below\n    (an OAuth access token IS such a key, so quotas and billing behave identically). Costs are\n    not duplicated here: GET /plans returns the current pricing as JSON, and the MCP tool `get_pricing`\n    needs no auth.'\n  sources:\n  - openapi/lawmadi-com-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lawmadi.com/oauth/authorize\n    tokenUrl: https://lawmadi.com/oauth/token\n    scopes: 2\n  description: 'Authorization code + PKCE (S256 only). Dynamic client registration is open (RFC\n    7591). Scope\
  \ `mcp:read` cannot spend the user''s credits. Server metadata: https://lawmadi.com/.well-known/oauth-authorization-server\n    (RFC 8414); protected resource metadata: https://lawmadi.com/mcp/.well-known/oauth-protected-resource\n    (RFC 9728).'\n  sources:\n  - openapi/lawmadi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/lawmadi-com/authentication/lawmadi-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Legal Tech
- Artificial Intelligence
- Korean
- Law
---
