---
api_key_in:
- query
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Singular Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Singular secures its APIs with apiKey and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Singular
provider_slug: singular
scheme_count: 5
schemes:
- applies_to:
  - Reporting API (api.singular.net/api/v2.0/)
  - SKAdNetwork API
  - Ad Monetization API
  - Singular Links API
  - Custom Fraud Rules API
  - Publisher Blacklist API
  - Partner Configuration Changes Log API
  - Testing Console API
  description: '"All API requests require an API key. To retrieve the key, log into your account and go to Developer Tools > API Keys. You can insert the key in the api_key parameter in your request, or provide the token under an Authorization HTTP header."'
  in: query
  name: apiKey-query
  parameter: api_key
  sources:
  - docs:support.singular.net/360045245692
  - docs:support.singular.net/360056377792
  type: apiKey
- bearer_prefix: false
  description: 'The same account API key may be sent as a bare Authorization header value. Singular''s Custom Fraud Rules reference is explicit: "Put the API key in the authorization HTTP header ... Do not prefix the header value with Bearer." Singular''s own Python client (singular-labs/singular_api_client) sends `headers = {"Authorization": self.api_key}`.'
  in: header
  name: apiKey-authorization-header
  parameter: Authorization
  sources:
  - docs:support.singular.net/53262822713755
  - https://github.com/singular-labs/singular_api_client/blob/master/singular_api_client/singular_client.py
  type: apiKey
- applies_to:
  - iOS/Android/Unity/Flutter/React Native/Cordova/Web SDKs
  - Server-to-Server endpoints
  description: Client-side attribution SDKs and the s2s.singular.net ingestion endpoints authenticate with an SDK Key (and the `a` parameter on S2S calls), issued per app from the Singular console. This is a distinct credential from the server-side Reporting API key.
  in: sdk-configuration
  name: sdk-key
  parameter: SDK Key / SDK Secret
  sources:
  - docs:support.singular.net/31394799175963
  - docs:support.singular.net/31496864868635
  type: apiKey
- applies_to:
  - Singular MCP (mcp.singular.net/mcp-server/mcp)
  description: 'The Singular MCP server is a full OAuth 2.1-style protected resource: RFC 8414 authorization-server metadata, RFC 9728 protected-resource metadata, RFC 7591 dynamic client registration, PKCE S256, and a published JWKS at https://mcp.singular.net/.well-known/jwks.json. Bearer token in the Authorization header; a call without one returns 401 with a WWW-Authenticate challenge naming the resource metadata document.'
  flows:
  - authorizationUrl: https://mcp.singular.net/oauth_server/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    pkce:
    - S256
    registrationUrl: https://mcp.singular.net/oauth_server/register
    scopes:
    - mcp:read
    tokenUrl: https://mcp.singular.net/oauth_server/token
    token_endpoint_auth_methods:
    - client_secret_post
    - none
  name: oauth2-mcp
  sources:
  - https://mcp.singular.net/.well-known/oauth-authorization-server
  - https://mcp.singular.net/.well-known/oauth-protected-resource
  - docs:support.singular.net/37923459892507
  type: oauth2
- applies_to:
  - www.singular.net/wp-json/mcp/mcp-oauth-server
  description: A second OAuth authorization server advertised by the WordPress marketing site for its WP MCP adapter endpoint. Separate from the product MCP above.
  flows:
  - authorizationUrl: https://www.singular.net/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    revocationUrl: https://www.singular.net/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://www.singular.net/oauth/token
    token_endpoint_auth_methods:
    - none
  name: oauth2-wordpress-mcp
  sources:
  - https://www.singular.net/.well-known/oauth-authorization-server
  - https://www.singular.net/.well-known/oauth-protected-resource
  type: oauth2
slug: singular-authentication
source_filename: singular-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://support.singular.net/hc/en-us/articles/360045245692-Reporting-API-Reference +\n  https://support.singular.net/hc/en-us/articles/53262822713755-Custom-Fraud-Rules-API-Reference +\n  https://support.singular.net/hc/en-us/articles/37923459892507-Singular-MCP +\n  https://mcp.singular.net/.well-known/oauth-authorization-server (200) +\n  live probes of api.singular.net and s2s.singular.net\ndocs: https://support.singular.net/hc/en-us/articles/207553433-Getting-Started-with-the-Singular-Reporting-API\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [query, header]\n  oauth2_flows: [authorizationCode]\nschemes:\n  - name: apiKey-query\n    type: apiKey\n    in: query\n    parameter: api_key\n    applies_to:\n      - Reporting API (api.singular.net/api/v2.0/)\n      - SKAdNetwork API\n      - Ad Monetization API\n      - Singular Links API\n      - Custom Fraud Rules API\n      - Publisher Blacklist API\n      - Partner\
  \ Configuration Changes Log API\n      - Testing Console API\n    description: >-\n      \"All API requests require an API key. To retrieve the key, log into your account and go\n      to Developer Tools > API Keys. You can insert the key in the api_key parameter in your\n      request, or provide the token under an Authorization HTTP header.\"\n    sources: [docs:support.singular.net/360045245692, docs:support.singular.net/360056377792]\n  - name: apiKey-authorization-header\n    type: apiKey\n    in: header\n    parameter: Authorization\n    bearer_prefix: false\n    description: >-\n      The same account API key may be sent as a bare Authorization header value. Singular's\n      Custom Fraud Rules reference is explicit: \"Put the API key in the authorization HTTP\n      header ... Do not prefix the header value with Bearer.\" Singular's own Python client\n      (singular-labs/singular_api_client) sends `headers = {\"Authorization\": self.api_key}`.\n    sources:\n      - docs:support.singular.net/53262822713755\n\
  \      - https://github.com/singular-labs/singular_api_client/blob/master/singular_api_client/singular_client.py\n  - name: sdk-key\n    type: apiKey\n    in: sdk-configuration\n    parameter: SDK Key / SDK Secret\n    applies_to: [iOS/Android/Unity/Flutter/React Native/Cordova/Web SDKs, Server-to-Server endpoints]\n    description: >-\n      Client-side attribution SDKs and the s2s.singular.net ingestion endpoints authenticate\n      with an SDK Key (and the `a` parameter on S2S calls), issued per app from the Singular\n      console. This is a distinct credential from the server-side Reporting API key.\n    sources: [docs:support.singular.net/31394799175963, docs:support.singular.net/31496864868635]\n  - name: oauth2-mcp\n    type: oauth2\n    applies_to: [Singular MCP (mcp.singular.net/mcp-server/mcp)]\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.singular.net/oauth_server/authorize\n        tokenUrl: https://mcp.singular.net/oauth_server/token\n\
  \        registrationUrl: https://mcp.singular.net/oauth_server/register\n        scopes: [mcp:read]\n        pkce: [S256]\n        token_endpoint_auth_methods: [client_secret_post, none]\n        dynamic_client_registration: true\n    description: >-\n      The Singular MCP server is a full OAuth 2.1-style protected resource: RFC 8414\n      authorization-server metadata, RFC 9728 protected-resource metadata, RFC 7591 dynamic\n      client registration, PKCE S256, and a published JWKS at\n      https://mcp.singular.net/.well-known/jwks.json. Bearer token in the Authorization\n      header; a call without one returns 401 with a WWW-Authenticate challenge naming the\n      resource metadata document.\n    sources:\n      - https://mcp.singular.net/.well-known/oauth-authorization-server\n      - https://mcp.singular.net/.well-known/oauth-protected-resource\n      - docs:support.singular.net/37923459892507\n  - name: oauth2-wordpress-mcp\n    type: oauth2\n    applies_to: [www.singular.net/wp-json/mcp/mcp-oauth-server]\n\
  \    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.singular.net/oauth/authorize\n        tokenUrl: https://www.singular.net/oauth/token\n        revocationUrl: https://www.singular.net/oauth/revoke\n        scopes: [mcp]\n        pkce: [S256]\n        token_endpoint_auth_methods: [none]\n    description: >-\n      A second OAuth authorization server advertised by the WordPress marketing site for its\n      WP MCP adapter endpoint. Separate from the product MCP above.\n    sources:\n      - https://www.singular.net/.well-known/oauth-authorization-server\n      - https://www.singular.net/.well-known/oauth-protected-resource\nconsole_access:\n  mfa: true\n  sso: true\n  note: >-\n    \"Singular supports 2FA as well as SSO\" (SSO is listed as an Enterprise-plan feature on\n    the pricing page).\n  source: https://www.singular.net/data-security-privacy/\nx-evidence:\n  - {url: 'https://api.singular.net/api/v2.0/reporting', http_status: 401, body: '{\"status\"\
  : 1, \"substatus\": 1, \"value\": \"Missing API Key\"}', fetched: '2026-08-12'}\n  - {url: 'https://api.singular.net/api/v1/fraud/rules/meta', http_status: 401, body: '{\"status\": 1, \"substatus\": 1, \"value\": \"Missing API Key\"}', fetched: '2026-08-12'}\n  - {url: 'https://mcp.singular.net/mcp-server/mcp', http_status: 401, body: 'invalid_token (WWW-Authenticate Bearer)', fetched: '2026-08-12'}\nnotes: >-\n  No OpenAPI/Swagger document is published on any Singular host, so this profile is read from\n  the provider's prose reference plus live probes and the published OAuth metadata rather\n  than from securitySchemes. No OpenID Connect discovery document is served\n  (/.well-known/openid-configuration is 404 on every host including mcp.singular.net).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singular/refs/heads/main/authentication/singular-authentication.yml
summary_line: apiKey/oauth2 · 5 schemes
tags:
- Company
- Marketing Analytics
- Mobile Attribution
- Attribution
- Marketing
- Advertising
- Analytics
- Mobile Measurement Partner
- SKAdNetwork
- Deep Linking
- Fraud Prevention
- ETL
- MCP
- Ad Monetization
- Privacy
---
