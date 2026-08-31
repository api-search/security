---
api_key_in:
- header
- query
api_specs:
- filename: brand-api-brands-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Brands API
  slug: brand-api-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-brands-api-openapi.yml
- filename: brand-api-context-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Context API
  slug: brand-api-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-context-api-openapi.yml
- filename: brand-api-search-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Search API
  slug: brand-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-search-api-openapi.yml
- filename: brand-api-viewer-api-openapi.yml
  format: yaml
  label: Brand API (Brandfetch) Viewer API
  slug: brand-api-viewer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/openapi/brand-api-viewer-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Brand Api Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Brand API (Brandfetch) secures its APIs with http, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Brand API (Brandfetch)
provider_slug: brand-api
scheme_count: 4
schemes:
- applies_to:
  - Brand API
  - Brand Context API
  - Transaction API
  - Viewer API
  declared_on_operations:
  - getBrandData
  - getBrandDataByDomain
  - getBrandDataByTicker
  - getBrandDataByIsin
  - getBrandDataByCrypto
  - getBrandContext
  - getBrandFromTransaction
  - getViewer
  format: 'Authorization: Bearer <api_key>'
  in: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/brand-api-brandfetch-openapi.yml
  type: http
- applies_to:
  - Logo API
  - Brand Search API
  format: ?c=<client_id>
  in: query
  name: clientId
  note: Present in the spec as a required query parameter on searchBrands rather than as a securityScheme, which is why the mechanical derive missed it. The Client ID is embedded in the `src` of a public <img> tag and is explicitly not a secret — it scopes fair-use rate limiting, not authorization. Logo CDN requests additionally require a Referer header and a Referrer-Policy of origin, origin-when-cross-origin, strict-origin, strict-origin-when-cross-origin or unsafe-url.
  parameter: c
  secret: false
  sources:
  - openapi/brand-api-brandfetch-openapi.yml
  - https://docs.brandfetch.com/logo-api/overview
  type: apiKey
- applies_to:
  - MCP server
  flows:
  - authorizationUrl: https://developers.brandfetch.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://developers.brandfetch.com/api/oauth/register
    scopes:
      read: Read access to Brandfetch brand data
    tokenUrl: https://developers.brandfetch.com/api/oauth/token
  issuer: https://developers.brandfetch.com
  name: mcpOAuth
  see: scopes/brand-api-scopes.yml
  sources:
  - https://developers.brandfetch.com/.well-known/oauth-authorization-server
  - https://mcp.brandfetch.io/.well-known/oauth-protected-resource
  type: oauth2
- applies_to:
  - MCP server
  in: header
  name: mcpToken
  note: Non-interactive fallback for MCP clients that cannot run an OAuth flow (CI, scripted agents). Minted in the Keys and MCP section of the developer dashboard.
  parameter: Authorization
  prefix: bf1.
  scheme: bearer
  sources:
  - https://docs.brandfetch.com/mcp/overview
  type: http
slug: brand-api-authentication
source_filename: brand-api-authentication.yml
source_heading: Authentication Profile
source_url: openapi/brand-api-brandfetch-openapi.yml
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.brandfetch.com/.well-known/agent-skills/brandfetch/skill.md\nsources:\n  - openapi/brand-api-brandfetch-openapi.yml\n  - https://docs.brandfetch.com/.well-known/agent-skills/brandfetch/skill.md\n  - https://docs.brandfetch.com/logo-api/overview\n  - https://docs.brandfetch.com/mcp/overview\n  - https://developers.brandfetch.com/.well-known/oauth-authorization-server\n  - https://mcp.brandfetch.io/.well-known/oauth-protected-resource\nnote: >-\n  The OpenAPI declares only one scheme (http bearer). That is a thin spec, not the whole\n  auth model: Brandfetch actually runs THREE distinct credential types across four\n  surfaces, and mixing them up is the failure mode Brandfetch itself calls out in its\n  published Agent Skill. This file is upgraded from the derived baseline with the docs.\nsummary:\n  types: [http, apiKey, oauth2]\n  api_key_in: [header, query]\n  oauth2_flows: [authorizationCode]\n  surfaces: 4\n\
  schemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: 'Authorization: Bearer <api_key>'\n    applies_to: [Brand API, Brand Context API, Transaction API, Viewer API]\n    sources: [openapi/brand-api-brandfetch-openapi.yml]\n    declared_on_operations:\n      - getBrandData\n      - getBrandDataByDomain\n      - getBrandDataByTicker\n      - getBrandDataByIsin\n      - getBrandDataByCrypto\n      - getBrandContext\n      - getBrandFromTransaction\n      - getViewer\n  - name: clientId\n    type: apiKey\n    in: query\n    parameter: c\n    format: '?c=<client_id>'\n    applies_to: [Logo API, Brand Search API]\n    secret: false\n    sources:\n      - openapi/brand-api-brandfetch-openapi.yml\n      - https://docs.brandfetch.com/logo-api/overview\n    note: >-\n      Present in the spec as a required query parameter on searchBrands rather than as a\n      securityScheme, which is why the mechanical derive missed it. The\
  \ Client ID is\n      embedded in the `src` of a public <img> tag and is explicitly not a secret — it\n      scopes fair-use rate limiting, not authorization. Logo CDN requests additionally\n      require a Referer header and a Referrer-Policy of origin, origin-when-cross-origin,\n      strict-origin, strict-origin-when-cross-origin or unsafe-url.\n  - name: mcpOAuth\n    type: oauth2\n    applies_to: [MCP server]\n    issuer: https://developers.brandfetch.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://developers.brandfetch.com/oauth/authorize\n        tokenUrl: https://developers.brandfetch.com/api/oauth/token\n        registrationUrl: https://developers.brandfetch.com/api/oauth/register\n        pkce: [S256]\n        scopes: {read: Read access to Brandfetch brand data}\n    sources:\n      - https://developers.brandfetch.com/.well-known/oauth-authorization-server\n      - https://mcp.brandfetch.io/.well-known/oauth-protected-resource\n    see: scopes/brand-api-scopes.yml\n\
  \  - name: mcpToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    prefix: 'bf1.'\n    applies_to: [MCP server]\n    sources: [https://docs.brandfetch.com/mcp/overview]\n    note: >-\n      Non-interactive fallback for MCP clients that cannot run an OAuth flow (CI,\n      scripted agents). Minted in the Keys and MCP section of the developer dashboard.\ncredential_introspection:\n  operation: getViewer\n  path: GET /v2/viewer\n  returns: 'ViewerApiKeyResponse | ViewerUserResponse — a `type` field says which credential was presented.'\n  semantics: '200 = valid credential; 401 = missing/unknown; 403 = revoked key or expired session.'\n  note: 'A genuinely useful integration-time affordance most providers do not ship.'\nfailure_modes:\n  - 'Sending a Client ID as a Bearer token (or an API key as ?c=) returns 401 Unauthorized.'\n  - 'Logo CDN requests without an acceptable Referrer-Policy can be rate limited or blocked.'\ndocs: https://docs.brandfetch.com/get-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brand-api/refs/heads/main/authentication/brand-api-authentication.yml
summary_line: http/apiKey/oauth2 · 4 schemes
tags:
- Brands
- Logos
- Brand Assets
- Company Data
- Firmographics
- Brand Context
- Merchant Enrichment
- Agent Tools
---
