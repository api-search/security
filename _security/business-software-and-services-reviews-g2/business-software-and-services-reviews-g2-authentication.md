---
api_key_in: []
api_specs:
- filename: business-software-and-services-reviews-g2-v2-openapi.yml
  format: yaml
  label: G2 API V2
  slug: g2-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-v2-openapi.yml
- filename: business-software-and-services-reviews-g2-v2-openapi.yml
  format: yaml
  label: G2 Buyer Intent Data API
  slug: g2-buyer-intent-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-v2-openapi.yml
- filename: business-software-and-services-reviews-g2-data-solutions-openapi.yml
  format: yaml
  label: G2 Data Solutions API
  slug: g2-data-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml
auth_types:
- http
- oauth2
description: G2 runs two parallel auth models against the same API. AccountAPIToken is an HTTP Bearer access token issued self-serve in the G2 Developer Portal, scoped to a User or an Organization, with per-endpoint permissions chosen at issue time and a hard one-year expiry; it secures 52 of the 62 published operations. G2OAuth is OAuth 2.0 Authorization Code with PKCE against G2's own authorization server, used for delegated access and required by the MCP server. G2 does NOT support RFC 7591 Dynamic Client Registration — OAuth apps are pre-registered by hand — and its authorization callback omits the `state` parameter, which breaks stock MCP SDK callback handlers.
kind: authentication
layout: security
method: searched
name: Business Software And Services Reviews G2 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Business Software and Services Reviews | G2 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Business Software and Services Reviews | G2
provider_slug: business-software-and-services-reviews-g2
scheme_count: 2
schemes:
- name: AccountAPIToken
  scheme: bearer
  sources:
  - openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml
  - openapi/business-software-and-services-reviews-g2-v2-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://www.g2.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://www.g2.com/oauth/token
  name: G2OAuth
  sources:
  - openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml
  - openapi/business-software-and-services-reviews-g2-v2-openapi.yml
  type: oauth2
slug: business-software-and-services-reviews-g2-authentication
source_filename: business-software-and-services-reviews-g2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/business-software-and-services-reviews-g2-v2-openapi.yml, openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml,\n  https://documentation.g2.com/docs/developer-portal, https://documentation.g2.com/docs/g2-mcp-server,\n  https://www.g2.com/.well-known/openid-configuration\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: AccountAPIToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml\n  - openapi/business-software-and-services-reviews-g2-v2-openapi.yml\n- name: G2OAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.g2.com/oauth/authorize\n    tokenUrl: https://www.g2.com/oauth/token\n    scopes: 6\n  sources:\n  - openapi/business-software-and-services-reviews-g2-data-solutions-openapi.yml\n  - openapi/business-software-and-services-reviews-g2-v2-openapi.yml\n\
  docs: https://documentation.g2.com/docs/developer-portal\ndescription: G2 runs two parallel auth models against the same API. AccountAPIToken is an HTTP Bearer\n  access token issued self-serve in the G2 Developer Portal, scoped to a User or an Organization, with\n  per-endpoint permissions chosen at issue time and a hard one-year expiry; it secures 52 of the 62 published\n  operations. G2OAuth is OAuth 2.0 Authorization Code with PKCE against G2's own authorization server,\n  used for delegated access and required by the MCP server. G2 does NOT support RFC 7591 Dynamic Client\n  Registration — OAuth apps are pre-registered by hand — and its authorization callback omits the `state`\n  parameter, which breaks stock MCP SDK callback handlers.\ndiscovery:\n  openid_configuration: well-known/business-software-and-services-reviews-g2-openid-configuration.json\n  oauth_authorization_server: well-known/business-software-and-services-reviews-g2-oauth-authorization-server.json\n  mcp_protected_resource:\
  \ well-known/business-software-and-services-reviews-g2-mcp-oauth-protected-resource.json\n  issuer: https://g2.com\n  authorization_endpoint: https://www.g2.com/oauth/authorize\n  token_endpoint: https://www.g2.com/oauth/token\n  revocation_endpoint: https://www.g2.com/oauth/revoke\n  introspection_endpoint: https://www.g2.com/oauth/introspect\n  userinfo_endpoint: https://www.g2.com/oauth/userinfo\n  jwks_uri: https://www.g2.com/oauth/discovery/keys\n  id_token_signing_alg: RS256\n  subject_types: pairwise\n  pkce_methods:\n  - plain\n  - S256\n  grant_types:\n  - authorization_code\n  - implicit_oidc\n  - refresh_token\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\nregistration:\n  url: https://my.g2.com/developers\n  dynamic_client_registration: false\n  confidential_clients: true\n  public_clients: true\n  note: Register the OAuth app in the Developer Portal, choose per-endpoint Read permissions, and read\n    client_id/client_secret from the app\
  \ details panel. Requested scopes must match enabled permissions\n    or the token request fails with \"requested scope is invalid, unknown, or malformed\".\ntokens:\n  access_token_lifetime: 1 year (Developer Portal access tokens)\n  refresh: refresh_token grant supported on the OAuth path\n  resource_owner: User or Organization, chosen at token creation\n  transport: 'Authorization: Bearer <token>'\ndeviations:\n- No RFC 7591 Dynamic Client Registration.\n- Authorization callback returns `code` without `state`.\n- The MCP server validates tokens via G2's introspection endpoint using its own credentials; without cross-application\n  token introspection enabled on your OAuth app you get 401 after a successful OAuth flow.\nscopes: scopes/business-software-and-services-reviews-g2-scopes.yml\nunauthenticated_surface: openapi/business-software-and-services-reviews-g2-chatgpt-plugin-openapi.json\n  declares auth type \"none\" for two product/report search operations on www.g2.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/business-software-and-services-reviews-g2/refs/heads/main/authentication/business-software-and-services-reviews-g2-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- B2B
- SaaS
- Software Reviews
- Buyer Intent
- Competitive Intelligence
- Market Intelligence
- Marketplace
- MCP
---
