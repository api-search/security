---
api_key_in:
- body
api_specs:
- filename: automattic-wordpress-com-rest-v1-1-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.1
  slug: wordpresscom-rest-api-v11
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-1-openapi.yml
- filename: automattic-wordpress-com-rest-v1-2-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.2
  slug: wordpresscom-rest-api-v12
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-2-openapi.yml
- filename: automattic-wordpress-com-rest-v1-3-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.3
  slug: wordpresscom-rest-api-v13
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-3-openapi.yml
- filename: automattic-wordpress-com-wp-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wp/v2 namespace
  slug: wordpresscom-rest-api-wpv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wp-v2-openapi.yml
- filename: automattic-wordpress-com-wpcom-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wpcom/v2 namespace
  slug: wordpresscom-rest-api-wpcomv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wpcom-v2-openapi.yml
- filename: automattic-akismet-openapi.yml
  format: yaml
  label: Akismet API
  slug: akismet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-akismet-openapi.yml
- filename: automattic-jetpack-ai-plugin-openapi.yaml
  format: yaml
  label: Jetpack AI-Plugin API
  slug: jetpack-ai-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-jetpack-ai-plugin-openapi.yaml
auth_types:
- oauth2
- openIdConnect
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Automattic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- clientCredentials
overview: Automattic secures its APIs with oauth2, openIdConnect, http, and apiKey across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and clientCredentials flow(s).
provider_name: Automattic
provider_slug: automattic
scheme_count: 6
schemes:
- applies_to:
  - /rest/v1.x
  - /wp/v2
  - /wpcom/v2
  - /wpcom/v2/mcp/v1
  discovery: https://public-api.wordpress.com/.well-known/oauth-authorization-server
  dynamic_client_registration: https://public-api.wordpress.com/oauth2-1/register
  flows:
  - authorizationUrl: https://public-api.wordpress.com/oauth2-1/authorize
    flow: authorizationCode
    scopes: 21
    tokenUrl: https://public-api.wordpress.com/oauth2-1/token
  - flow: refreshToken
    tokenUrl: https://public-api.wordpress.com/oauth2-1/token
  - flow: clientCredentials
    tokenUrl: https://public-api.wordpress.com/oauth2-1/token
  introspection: https://public-api.wordpress.com/oauth2-1/token-info
  issuer: https://public-api.wordpress.com
  name: oauth2
  pkce:
  - S256
  resource_indicators_supported: true
  revocation: https://public-api.wordpress.com/oauth2-1/revoke
  scopes_artifact: scopes/automattic-scopes.yml
  sources:
  - https://public-api.wordpress.com/.well-known/oauth-authorization-server
  - openapi/automattic-wordpress-com-rest-v1-1-openapi.yml
  - openapi/automattic-wordpress-com-wp-v2-openapi.yml
  - openapi/automattic-wordpress-com-wpcom-v2-openapi.yml
  spec: OAuth 2.1
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  token_expiry: two weeks
  type: oauth2
- claims_supported:
  - sub
  - iss
  - aud
  - exp
  - iat
  - auth_time
  - nonce
  - name
  - preferred_username
  - picture
  - email
  - email_verified
  - updated_at
  id_token_signing_alg_values_supported:
  - RS256
  jwks_uri: https://public-api.wordpress.com/.well-known/jwks.json
  name: openIdConnect
  openIdConnectUrl: https://public-api.wordpress.com/.well-known/openid-configuration
  sources:
  - https://public-api.wordpress.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
  userinfo_endpoint: https://public-api.wordpress.com/oauth2-1/userinfo
- bearer_methods_supported:
  - header
  description: 'Authorization: Bearer <access_token> — the wire format for every OAuth 2.1 token.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://public-api.wordpress.com/.well-known/oauth-protected-resource
  - openapi/automattic-wordpress-com-rest-v1-1-openapi.yml
  type: http
- description: Application Passwords are documented as a shortcut for personal and development use against WordPress.com, in place of the full OAuth2 flow.
  docs: https://developer.wordpress.com/docs/api/
  name: applicationPassword
  scheme: basic
  sources:
  - https://developer.wordpress.com/docs/api/
  type: http
- applies_to:
  - https://rest.akismet.com
  description: Akismet authenticates with an API key sent as a request field alongside a `blog` field identifying the site. There is no OAuth on this API and no bearer header.
  in: body
  name: akismetApiKey
  parameter_name: key
  sources:
  - openapi/automattic-akismet-openapi.yml
  - https://akismet.com/development/api/
  type: apiKey
- description: The WordPress VIP GraphQL Platform API requires a VIP token; unauthenticated requests to https://api.wpvip.com/graphql return 401 Unauthorized.
  docs: https://docs.wpvip.com/vip-api/getting-started
  name: vipPlatformToken
  scheme: bearer
  sources:
  - graphql/automattic-vip-platform-api.yml
  type: http
slug: automattic-authentication
source_filename: automattic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: searched\nsource: https://public-api.wordpress.com/.well-known/openid-configuration\ndocs: https://developer.wordpress.com/docs/api/oauth2/\nsummary:\n  types: [oauth2, openIdConnect, http, apiKey]\n  oauth2_flows: [authorizationCode, refreshToken, clientCredentials]\n  api_key_in: [body]\n  note: >-\n    One OAuth 2.1 / OpenID Connect authorization server covers all three WordPress.com REST\n    namespaces and the hosted MCP server. Akismet is the exception: it is a separate product on a\n    separate host with a plain API key passed as a request field.\nschemes:\n- name: oauth2\n  type: oauth2\n  spec: OAuth 2.1\n  issuer: https://public-api.wordpress.com\n  discovery: https://public-api.wordpress.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://public-api.wordpress.com/oauth2-1/authorize\n    tokenUrl: https://public-api.wordpress.com/oauth2-1/token\n    scopes: 21\n  - flow:\
  \ refreshToken\n    tokenUrl: https://public-api.wordpress.com/oauth2-1/token\n  - flow: clientCredentials\n    tokenUrl: https://public-api.wordpress.com/oauth2-1/token\n  pkce: [S256]\n  dynamic_client_registration: https://public-api.wordpress.com/oauth2-1/register\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  revocation: https://public-api.wordpress.com/oauth2-1/revoke\n  introspection: https://public-api.wordpress.com/oauth2-1/token-info\n  resource_indicators_supported: true\n  token_expiry: two weeks\n  scopes_artifact: scopes/automattic-scopes.yml\n  applies_to: [/rest/v1.x, /wp/v2, /wpcom/v2, /wpcom/v2/mcp/v1]\n  sources:\n  - https://public-api.wordpress.com/.well-known/oauth-authorization-server\n  - openapi/automattic-wordpress-com-rest-v1-1-openapi.yml\n  - openapi/automattic-wordpress-com-wp-v2-openapi.yml\n  - openapi/automattic-wordpress-com-wpcom-v2-openapi.yml\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://public-api.wordpress.com/.well-known/openid-configuration\n\
  \  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  userinfo_endpoint: https://public-api.wordpress.com/oauth2-1/userinfo\n  jwks_uri: https://public-api.wordpress.com/.well-known/jwks.json\n  claims_supported: [sub, iss, aud, exp, iat, auth_time, nonce, name, preferred_username, picture,\n    email, email_verified, updated_at]\n  sources: [https://public-api.wordpress.com/.well-known/openid-configuration]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <access_token> — the wire format for every OAuth 2.1 token.'\n  bearer_methods_supported: [header]\n  sources:\n  - https://public-api.wordpress.com/.well-known/oauth-protected-resource\n  - openapi/automattic-wordpress-com-rest-v1-1-openapi.yml\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    Application Passwords are documented as a shortcut for personal and development use against\n    WordPress.com, in place of the full\
  \ OAuth2 flow.\n  docs: https://developer.wordpress.com/docs/api/\n  sources: [https://developer.wordpress.com/docs/api/]\n- name: akismetApiKey\n  type: apiKey\n  in: body\n  parameter_name: key\n  description: >-\n    Akismet authenticates with an API key sent as a request field alongside a `blog` field\n    identifying the site. There is no OAuth on this API and no bearer header.\n  applies_to: [https://rest.akismet.com]\n  sources: [openapi/automattic-akismet-openapi.yml, https://akismet.com/development/api/]\n- name: vipPlatformToken\n  type: http\n  scheme: bearer\n  description: >-\n    The WordPress VIP GraphQL Platform API requires a VIP token; unauthenticated requests to\n    https://api.wpvip.com/graphql return 401 Unauthorized.\n  docs: https://docs.wpvip.com/vip-api/getting-started\n  sources: [graphql/automattic-vip-platform-api.yml]\nlegacy_and_deprecated:\n- item: implicit flow\n  status: legacy/deprecated\n  source: https://developer.wordpress.com/docs/api/oauth2/\n- item:\
  \ password grant\n  status: development and testing only\n  source: https://developer.wordpress.com/docs/api/oauth2/\n- item: /oauth2/authorize and /oauth2/token\n  status: >-\n    older endpoint pair still documented and still referenced by the ai-plugin manifest; the\n    /oauth2-1/ pair is what the discovery documents advertise.\nx-evidence:\n  fetched: '2026-07-31'\n  urls:\n  - https://public-api.wordpress.com/.well-known/openid-configuration\n  - https://public-api.wordpress.com/.well-known/oauth-authorization-server\n  - https://public-api.wordpress.com/.well-known/oauth-protected-resource\n  - https://developer.wordpress.com/docs/api/oauth2/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/authentication/automattic-authentication.yml
summary_line: oauth2/openIdConnect/http/apiKey · 6 schemes
tags:
- Company
- Content Management
- Publishing
- Blogging
- Website Hosting
- Web Publishing
- Content
- Comments
- Spam Filtering
- Media
- Analytics
- Domains
- E-Commerce
- Open Source
- Developer Tools
- Model Context Protocol
---
