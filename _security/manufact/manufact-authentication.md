---
anonymous_access: false
api_key_in: []
auth_types: []
description: Manufact authentication methods
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Manufact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Manufact (formerly mcp-use) declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Manufact (formerly mcp-use)
provider_slug: manufact
scheme_count: 4
schemes:
- evidence: 'Send it as a bearer token (an x-api-key header works too): curl -H "Authorization: Bearer mcp_..." https://cloud.manufact.com/api/v1/servers'
  header: Authorization
  how_to_obtain: Create an API key on the API Keys page; the key starts with mcp_ and is shown only once.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Send it as a bearer token (an x-api-key header works too): curl -H "Authorization: Bearer mcp_..." https://cloud.manufact.com/api/v1/servers'
  header: x-api-key
  how_to_obtain: Create an API key on the API Keys page; the key starts with mcp_ and is shown only once.
  location: header
  name: x-api-key header
  type: apiKey
- evidence: 'oauth : oauthWorkOSProvider ({ subdomain : process . env . WORKOS_SUBDOMAIN ! , requiredScopes : [ "shop" ], })'
  how_to_obtain: Configure WorkOS in the dashboard, enable Dynamic Client Registration, and provide the subdomain to the oauthWorkOSProvider.
  name: WorkOS OAuth
  scopes:
  - shop
  type: oauth2
- authorize_url: https://{domain}/authorize
  evidence: 'oauth : oauthProxy ({ authEndpoint : `https:// ${ domain } /authorize` , tokenEndpoint : `https:// ${ domain } /oauth/token` , issuer : `https:// ${ domain } /` , clientId , clientSecret , scopes : [ "openid" , "email" , "profile" ], ... })'
  how_to_obtain: Create a regular web app in the provider (e.g., Auth0) dashboard, note client_id and client_secret, then configure oauthProxy with those values.
  name: OAuth Proxy (e.g., Auth0)
  scopes:
  - openid
  - email
  - profile
  token_url: https://{domain}/oauth/token
  type: oauth2
slug: manufact-authentication
source_filename: manufact-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.manufact.com/dashboard/api-keys
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.manufact.com/dashboard/api-keys\nsources:\n- https://docs.manufact.com/dashboard/api-keys\n- https://manufact.com/blog/mixed-authentication\n- https://manufact.com/blog/oauth-mcp\n- https://manufact.com/blog/authentication\ndescription: Manufact authentication methods\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send it as a bearer token (an x-api-key header works too): curl -H \"Authorization: Bearer mcp_...\" https://cloud.manufact.com/api/v1/servers'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key on the API Keys page; the key starts with mcp_ and is shown only once.\n- type: apiKey\n  name: x-api-key header\n  evidence: 'Send it as a bearer token (an x-api-key header works too): curl -H \"Authorization: Bearer mcp_...\" https://cloud.manufact.com/api/v1/servers'\n  location: header\n  header: x-api-key\n  how_to_obtain:\
  \ Create an API key on the API Keys page; the key starts with mcp_ and is shown only once.\n- type: oauth2\n  name: WorkOS OAuth\n  evidence: 'oauth : oauthWorkOSProvider ({ subdomain : process . env . WORKOS_SUBDOMAIN ! , requiredScopes : [ \"shop\" ], })'\n  scopes:\n  - shop\n  how_to_obtain: Configure WorkOS in the dashboard, enable Dynamic Client Registration, and provide the subdomain to the oauthWorkOSProvider.\n- type: oauth2\n  name: OAuth Proxy (e.g., Auth0)\n  evidence: 'oauth : oauthProxy ({ authEndpoint : `https:// ${ domain } /authorize` , tokenEndpoint : `https:// ${ domain } /oauth/token` , issuer\n    : `https:// ${ domain } /` , clientId , clientSecret , scopes : [ \"openid\" , \"email\" , \"profile\" ], ... })'\n  token_url: https://{domain}/oauth/token\n  authorize_url: https://{domain}/authorize\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Create a regular web app in the provider (e.g., Auth0) dashboard, note client_id and client_secret, then configure\
  \ oauthProxy\n    with those values.\nnote: OAuth flows (authorization_code, client_credentials, etc.) are not explicitly listed on the pages; only provider‑specific configuration\n  is shown.\ndocs: https://docs.manufact.com/dashboard/api-keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manufact/refs/heads/main/authentication/manufact-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Manufacturing
- Data
- API
- SupplyChain
---
