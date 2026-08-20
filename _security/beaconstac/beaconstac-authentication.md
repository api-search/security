---
api_key_in:
- header
api_specs:
- filename: postman.yaml
  format: yaml
  label: Uniqode QR Code API
  slug: uniqode-qr-code-api
  spec_type: Postman
  url: https://apidocs.uniqode.com/
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Beaconstac Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Beaconstac secures its APIs with apiKey, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Beaconstac
provider_slug: beaconstac
scheme_count: 4
schemes:
- applies_to: REST API
  description: A dashboard-issued API key sent as a Token in the Authorization header. The key is found in the API section of the Uniqode dashboard sidebar. All requests must be made over HTTPS; plain HTTP and unauthenticated requests fail. API access requires a Pro plan or above.
  example: 'curl -X "GET" "https://api.uniqode.com/api/2.0/qrcodes/" -H "Authorization: Token <API_KEY>" -H "Content-Type: application/json"'
  format: 'Authorization: Token <API_KEY>'
  in: header
  name: TokenAuth
  parameter_name: Authorization
  sources:
  - https://apidocs.uniqode.com/
  - https://docs.uniqode.com/en/articles/6064771-getting-started-with-static-and-dynamic-qr-code-api
  type: apiKey
- applies_to: REST API
  description: Organization identifier from the dashboard API section. Required for accounts with multi-user access management, to scope a request to a specific organization. The published collection sends it as an `organization` query parameter on Digital Business Card, Analytics and Feedback Form requests (the collection variable is ORG_ID); the help-center article describes it as a value copied alongside the API key.
  in: query
  name: OrganizationId
  parameter_name: organization
  sources:
  - https://apidocs.uniqode.com/
  - https://docs.uniqode.com/en/articles/6064771-getting-started-with-static-and-dynamic-qr-code-api
  type: apiKey
- applies_to: MCP server
  bearer_methods_supported:
  - header
  description: The hosted MCP server is an OAuth 2.0 protected resource (RFC 9728). Anonymous calls return 401 with a WWW-Authenticate Bearer challenge naming the resource metadata document. Dynamic client registration is open at https://auth.uniqode.com/oidc/register.
  flows:
  - authorizationUrl: https://auth.uniqode.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    scope_count: 6
    tokenUrl: https://auth.uniqode.com/oauth/token
  - deviceAuthorizationUrl: https://auth.uniqode.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.uniqode.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.uniqode.com/oauth/token
  name: UniqodeMCPOAuth
  ref: scopes/beaconstac-scopes.yml
  sources:
  - https://mcp.uniqode.com/.well-known/oauth-protected-resource
  - https://auth.uniqode.com/.well-known/oauth-authorization-server
  type: oauth2
- applies_to: Dashboard + MCP identity
  backchannel_logout_supported: true
  id_token_signing_alg_values_supported:
  - HS256
  - RS256
  - PS256
  issuer: https://auth.uniqode.com/
  name: UniqodeOIDC
  openIdConnectUrl: https://auth.uniqode.com/.well-known/openid-configuration
  platform: Auth0, on Uniqode's own auth.uniqode.com custom domain
  sources:
  - https://auth.uniqode.com/.well-known/openid-configuration
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
slug: beaconstac-authentication
source_filename: beaconstac-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://apidocs.uniqode.com/ (published Postman collection),\n  https://docs.uniqode.com/en/articles/6064771-getting-started-with-static-and-dynamic-qr-code-api,\n  https://mcp.uniqode.com/.well-known/oauth-protected-resource,\n  https://auth.uniqode.com/.well-known/openid-configuration\ndocs: https://docs.uniqode.com/en/articles/6064771-getting-started-with-static-and-dynamic-qr-code-api\n# Uniqode runs TWO distinct auth models on two distinct surfaces, and they do not share a\n# credential. No OpenAPI is published; the REST model is read from the provider's own published\n# Postman collection + help-center article, the MCP model from probed discovery documents.\nsummary:\n  types: [apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken]\nsurfaces:\n- surface: REST API (https://api.uniqode.com/api/2.0/)\n  model: static account token\n-\
  \ surface: MCP server (https://mcp.uniqode.com/mcp)\n  model: OAuth 2.1 bearer, authorization server https://auth.uniqode.com/\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: \"Authorization: Token <API_KEY>\"\n  applies_to: REST API\n  description: >-\n    A dashboard-issued API key sent as a Token in the Authorization header. The key is found in\n    the API section of the Uniqode dashboard sidebar. All requests must be made over HTTPS;\n    plain HTTP and unauthenticated requests fail. API access requires a Pro plan or above.\n  example: >-\n    curl -X \"GET\" \"https://api.uniqode.com/api/2.0/qrcodes/\"\n    -H \"Authorization: Token <API_KEY>\" -H \"Content-Type: application/json\"\n  sources:\n  - https://apidocs.uniqode.com/\n  - https://docs.uniqode.com/en/articles/6064771-getting-started-with-static-and-dynamic-qr-code-api\n- name: OrganizationId\n  type: apiKey\n  in: query\n  parameter_name: organization\n  applies_to:\
  \ REST API\n  description: >-\n    Organization identifier from the dashboard API section. Required for accounts with\n    multi-user access management, to scope a request to a specific organization. The published\n    collection sends it as an `organization` query parameter on Digital Business Card, Analytics\n    and Feedback Form requests (the collection variable is ORG_ID); the help-center article\n    describes it as a value copied alongside the API key.\n  sources:\n  - https://apidocs.uniqode.com/\n  - https://docs.uniqode.com/en/articles/6064771-getting-started-with-static-and-dynamic-qr-code-api\n- name: UniqodeMCPOAuth\n  type: oauth2\n  applies_to: MCP server\n  bearer_methods_supported: [header]\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.uniqode.com/authorize\n    tokenUrl: https://auth.uniqode.com/oauth/token\n    pkce: [S256, plain]\n    scope_count: 6\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.uniqode.com/oauth/device/code\n\
  \    tokenUrl: https://auth.uniqode.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.uniqode.com/oauth/token\n  description: >-\n    The hosted MCP server is an OAuth 2.0 protected resource (RFC 9728). Anonymous calls return\n    401 with a WWW-Authenticate Bearer challenge naming the resource metadata document.\n    Dynamic client registration is open at https://auth.uniqode.com/oidc/register.\n  ref: scopes/beaconstac-scopes.yml\n  sources:\n  - https://mcp.uniqode.com/.well-known/oauth-protected-resource\n  - https://auth.uniqode.com/.well-known/oauth-authorization-server\n- name: UniqodeOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://auth.uniqode.com/.well-known/openid-configuration\n  issuer: https://auth.uniqode.com/\n  applies_to: Dashboard + MCP identity\n  id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  backchannel_logout_supported:\
  \ true\n  platform: Auth0, on Uniqode's own auth.uniqode.com custom domain\n  sources: [https://auth.uniqode.com/.well-known/openid-configuration]\nnotes:\n- Dashboard sign-in additionally supports 2FA and SAML-based SSO with role-based access control (uniqode.com/security).\n- >-\n  The REST token and the MCP OAuth token are separate credentials on separate hosts; an MCP\n  access token is not accepted by api.uniqode.com and vice versa.\n- No API key rotation, expiry, or scoping policy is published for the REST token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beaconstac/refs/heads/main/authentication/beaconstac-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 4 schemes
tags:
- Company
- Big Data
- QR Codes
- Digital Business Cards
- Marketing
- Analytics
- Software-as-a-Service
- Proximity
- Webhook
- MCP
---
