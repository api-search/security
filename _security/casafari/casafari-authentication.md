---
anonymous_access: false
api_key_in: []
api_specs:
- filename: casafari-api-openapi.json
  format: json
  label: Casafari API API
  slug: casafari-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/casafari/refs/heads/main/openapi/_original/casafari-api-openapi.json
auth_types: []
description: Authentication methods for Casafari MCP and REST APIs as documented.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Casafari Authentication
name_suffix: Authentication
oauth_flows: []
overview: Casafari API and MCP Platform declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Casafari API and MCP Platform
provider_slug: casafari
scheme_count: 3
schemes:
- evidence: Casafari MCP uses OAuth 2.1 sign-in with no API key; the Casafari MCP server uses no OAuth scopes, and REST signs in with separate credentials.
  flows:
  - authorization_code
  - client_credentials
  how_to_obtain: Register a client via the registration endpoint to obtain a client_id (and client_secret for client credentials). Include the resource parameter from the protected resource metadata in all requests.
  name: Casafari MCP OAuth2
  type: oauth2
- evidence: 'Call the server with `Authorization: Bearer <access_token>`.'
  header: Authorization
  how_to_obtain: Obtain an access token by POSTing email and password to `https://api.casafari.com/login` (REST API) or via the OAuth flows for MCP.
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'The platform''s REST API takes an API key (`cf_sk_…`) in the `X-API-Key` header or as `Authorization: Bearer <api_key>`.'
  header: X-API-Key
  how_to_obtain: Generate an API key in the Casafari account dashboard and include it in the request header.
  location: header
  name: X-API-Key
  type: apiKey
slug: casafari-authentication
source_filename: casafari-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.casafari.com/docs/authentication.md
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.casafari.com/docs/authentication.md\nsources:\n- https://developers.casafari.com/docs/authentication.md\n- https://developers.casafari.com/docs/rest/authentication/login.md\n- https://developers.casafari.com/docs/rest/authentication/refresh-token.md\n- https://developers.casafari.com/docs/faq/how-authentication-works.md\ndescription: Authentication methods for Casafari MCP and REST APIs as documented.\nschemes:\n- type: oauth2\n  name: Casafari MCP OAuth2\n  evidence: Casafari MCP uses OAuth 2.1 sign-in with no API key; the Casafari MCP server uses no OAuth scopes, and REST signs in with separate\n    credentials.\n  flows:\n  - authorization_code\n  - client_credentials\n  how_to_obtain: Register a client via the registration endpoint to obtain a client_id (and client_secret for client credentials). Include the\n    resource parameter from the protected resource\
  \ metadata in all requests.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Call the server with `Authorization: Bearer <access_token>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an access token by POSTing email and password to `https://api.casafari.com/login` (REST API) or via the OAuth flows for\n    MCP.\n- type: apiKey\n  name: X-API-Key\n  evidence: 'The platform''s REST API takes an API key (`cf_sk_…`) in the `X-API-Key` header or as `Authorization: Bearer <api_key>`.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Generate an API key in the Casafari account dashboard and include it in the request header.\ndocs: https://developers.casafari.com/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/casafari/refs/heads/main/authentication/casafari-authentication.yml
summary_line: 3 schemes
tags:
- Real Estate Data
- Property Sourcing
- Valuation
- Market Analytics
- API
- CRM
- Real Estate Software
---
