---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: probed
name: Blue Origin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
- implicit
overview: Blue Origin secures its APIs with oauth2, openIdConnect, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, jwtBearer, and implicit flow(s).
provider_name: Blue Origin
provider_slug: blue-origin
scheme_count: 3
schemes:
- end_session_endpoint: https://shopify.com/authentication/30100881545/logout
  flows:
  - authorizationUrl: https://shopify.com/authentication/30100881545/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://shopify.com/authentication/30100881545/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/30100881545
  jwks_uri: https://shopify.com/authentication/30100881545/.well-known/jwks.json
  name: shopify-customer-account
  openIdConnectUrl: https://shop.blueorigin.com/.well-known/openid-configuration
  protected_resource:
    authorization_servers:
    - https://shopify.com/authentication/30100881545
    bearer_methods_supported:
    - header
    metadata: well-known/blue-origin-shop-oauth-protected-resource.json
    resource: https://shop.blueorigin.com
    rfc: RFC 9728
  source: well-known/blue-origin-shop-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- end_session_endpoint: https://payloads.blueorigin.com/services/auth/idp/oidc/logout
  flows:
  - authorizationUrl: https://payloads.blueorigin.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://payloads.blueorigin.com/services/oauth2/token
  - authorizationUrl: https://payloads.blueorigin.com/services/oauth2/authorize
    flow: implicit
    note: response_types_supported includes token and token id_token
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://payloads.blueorigin.com/services/oauth2/introspect
  issuer: https://payloads.blueorigin.com
  jwks_uri: https://payloads.blueorigin.com/id/keys
  name: salesforce-payloads-portal
  openIdConnectUrl: https://payloads.blueorigin.com/.well-known/openid-configuration
  registration_endpoint: https://payloads.blueorigin.com/services/oauth2/register
  revocation_endpoint: https://payloads.blueorigin.com/services/oauth2/revoke
  source: well-known/blue-origin-payloads-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://payloads.blueorigin.com/services/oauth2/userinfo
- end_session_endpoint: https://bodp.blueorigin.com/services/auth/idp/oidc/logout
  flows:
  - authorizationUrl: https://bodp.blueorigin.com/services/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://bodp.blueorigin.com/services/oauth2/token
  id_token_signing_alg:
  - RS256
  issuer: https://bodp.blueorigin.com
  jwks_uri: https://bodp.blueorigin.com/id/keys
  name: salesforce-bodp-portal
  openIdConnectUrl: https://bodp.blueorigin.com/.well-known/openid-configuration
  source: well-known/blue-origin-bodp-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
slug: blue-origin-authentication
source_filename: blue-origin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live /.well-known/openid-configuration + /.well-known/oauth-authorization-server\n  + /.well-known/oauth-protected-resource probes on Blue Origin hosts\nnote: >-\n  Blue Origin publishes no OpenAPI, no developer portal and no authentication\n  documentation, so nothing here is derived from a spec — every scheme below was read\n  from a discovery document the host served anonymously. Three distinct identity\n  surfaces exist, none of them Blue Origin-built: a Shopify customer-account\n  authorization server behind the Blue Origin Shop, and one Salesforce Experience Cloud\n  identity provider fronting each of the two customer/data portals (both portals sit on\n  the same Salesforce org, 00D8Y0000008AXY). The MCP server at shop.blueorigin.com/api/mcp\n  needs no credential for tools/list, search_catalog, get_product_details, get_cart,\n  update_cart or search_shop_policies_and_faqs; only checkout requires buyer identity\n  and contemporaneous\
  \ approval.\nsummary:\n  types: [oauth2, openIdConnect, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, refreshToken, jwtBearer, implicit]\n  unauthenticated_surfaces:\n  - https://shop.blueorigin.com/api/mcp (tools/list and read tools)\n  - https://shop.blueorigin.com/products.json\n  - https://payloads.blueorigin.com/services/data (version list only)\n  - https://bodp.blueorigin.com/services/data (version list only)\nschemes:\n- name: shopify-customer-account\n  type: openIdConnect\n  source: well-known/blue-origin-shop-openid-configuration.json\n  openIdConnectUrl: https://shop.blueorigin.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/30100881545\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/30100881545/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/30100881545/oauth/token\n    pkce: [S256]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n\
  \  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  jwks_uri: https://shopify.com/authentication/30100881545/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/30100881545/logout\n  protected_resource:\n    metadata: well-known/blue-origin-shop-oauth-protected-resource.json\n    rfc: RFC 9728\n    resource: https://shop.blueorigin.com\n    authorization_servers: [https://shopify.com/authentication/30100881545]\n    bearer_methods_supported: [header]\n- name: salesforce-payloads-portal\n  type: openIdConnect\n  source: well-known/blue-origin-payloads-openid-configuration.json\n  openIdConnectUrl: https://payloads.blueorigin.com/.well-known/openid-configuration\n  issuer: https://payloads.blueorigin.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://payloads.blueorigin.com/services/oauth2/authorize\n    tokenUrl: https://payloads.blueorigin.com/services/oauth2/token\n  - flow: implicit\n    authorizationUrl:\
  \ https://payloads.blueorigin.com/services/oauth2/authorize\n    note: response_types_supported includes token and token id_token\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_alg: [RS256]\n  jwks_uri: https://payloads.blueorigin.com/id/keys\n  userinfo_endpoint: https://payloads.blueorigin.com/services/oauth2/userinfo\n  introspection_endpoint: https://payloads.blueorigin.com/services/oauth2/introspect\n  revocation_endpoint: https://payloads.blueorigin.com/services/oauth2/revoke\n  registration_endpoint: https://payloads.blueorigin.com/services/oauth2/register\n  end_session_endpoint: https://payloads.blueorigin.com/services/auth/idp/oidc/logout\n- name: salesforce-bodp-portal\n  type: openIdConnect\n  source: well-known/blue-origin-bodp-openid-configuration.json\n  openIdConnectUrl: https://bodp.blueorigin.com/.well-known/openid-configuration\n  issuer: https://bodp.blueorigin.com\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://bodp.blueorigin.com/services/oauth2/authorize\n    tokenUrl: https://bodp.blueorigin.com/services/oauth2/token\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, private_key_jwt]\n  id_token_signing_alg: [RS256]\n  jwks_uri: https://bodp.blueorigin.com/id/keys\n  end_session_endpoint: https://bodp.blueorigin.com/services/auth/idp/oidc/logout\nobserved_auth_errors:\n- surface: https://payloads.blueorigin.com/services/oauth2/userinfo\n  http_status: 403\n  body: Missing_OAuth_Token\n- surface: https://payloads.blueorigin.com/openapi.json\n  http_status: 401\n- surface: https://bodp.blueorigin.com/openapi.json\n  http_status: 401\nx-evidence:\n  fetched: '2026-08-02'\n  discovery_documents: 3\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-origin/refs/heads/main/authentication/blue-origin-authentication.yml
summary_line: oauth2/openIdConnect/none · 3 schemes
tags:
- Company
- Aerospace
- Space
- Spaceflight
- Launch Services
- Satellites
- Rocket Engines
- Defense
- Manufacturing
- E-Commerce
- MCP
---
