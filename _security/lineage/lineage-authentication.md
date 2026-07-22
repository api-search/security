---
api_key_in: []
auth_types:
- openIdConnect
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lineage Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Lineage secures its APIs with openIdConnect and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Lineage
provider_slug: lineage
scheme_count: 2
schemes:
- authorization_endpoint: https://lineage-ciam.us.auth0.com/authorize
  code_challenge_methods:
  - S256
  - plain
  custom_domain: https://ciam.lineageapps.com
  device_authorization_endpoint: https://lineage-ciam.us.auth0.com/oauth/device/code
  issuer: https://lineage-ciam.us.auth0.com/
  jwks_uri: https://lineage-ciam.us.auth0.com/.well-known/jwks.json
  name: LineageLinkCIAM
  openIdConnectUrl: https://lineage-ciam.us.auth0.com/.well-known/openid-configuration
  pkce: true
  provider: Auth0
  purpose: Customer identity (CIAM) for the Lineage Link supply chain platform
  registration_endpoint: https://lineage-ciam.us.auth0.com/oidc/register
  revocation_endpoint: https://lineage-ciam.us.auth0.com/oauth/revoke
  sources:
  - well-known/lineage-ciam-openid-configuration.json
  token_endpoint: https://lineage-ciam.us.auth0.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://lineage-ciam.us.auth0.com/userinfo
- authorization_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/authorize
  id_token_signing_alg:
  - RS256
  introspection_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/introspect
  issuer: https://lineagelinkhelp.onelineage.com/support
  jwks_uri: https://lineagelinkhelp.onelineage.com/support/id/keys
  name: LineageLinkHelpCommunity
  openIdConnectUrl: https://lineagelinkhelp.onelineage.com/.well-known/openid-configuration
  provider: Salesforce Experience Cloud
  purpose: Identity for the Lineage Link Help support community
  registration_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/register
  revocation_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/revoke
  sources:
  - well-known/lineage-linkhelp-openid-configuration.json
  token_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/userinfo
slug: lineage-authentication
source_filename: lineage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  OIDC discovery documents fetched from lineage-ciam.us.auth0.com and\n  lineagelinkhelp.onelineage.com on 2026-07-19\nscope_of_this_profile: >-\n  Lineage publishes no public API and no developer portal, so there is no\n  documented API authentication contract. What is documented below is the\n  customer-facing IDENTITY surface behind the Lineage Link platform and its help\n  community — real, verified OpenID Connect endpoints, but end-user portal SSO\n  rather than a programmatic API auth scheme. Do not read this as evidence of a\n  public API.\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\n  - refreshToken\n  api_key_in: []\n  public_api_documented: false\nschemes:\n- name: LineageLinkCIAM\n  type: openIdConnect\n  provider: Auth0\n  purpose: Customer identity (CIAM) for the Lineage Link supply chain platform\n  custom_domain: https://ciam.lineageapps.com\n\
  \  issuer: https://lineage-ciam.us.auth0.com/\n  openIdConnectUrl: https://lineage-ciam.us.auth0.com/.well-known/openid-configuration\n  authorization_endpoint: https://lineage-ciam.us.auth0.com/authorize\n  token_endpoint: https://lineage-ciam.us.auth0.com/oauth/token\n  userinfo_endpoint: https://lineage-ciam.us.auth0.com/userinfo\n  jwks_uri: https://lineage-ciam.us.auth0.com/.well-known/jwks.json\n  revocation_endpoint: https://lineage-ciam.us.auth0.com/oauth/revoke\n  device_authorization_endpoint: https://lineage-ciam.us.auth0.com/oauth/device/code\n  registration_endpoint: https://lineage-ciam.us.auth0.com/oidc/register\n  pkce: true\n  code_challenge_methods:\n  - S256\n  - plain\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  sources:\n  - well-known/lineage-ciam-openid-configuration.json\n- name: LineageLinkHelpCommunity\n  type: openIdConnect\n  provider: Salesforce Experience Cloud\n  purpose: Identity for the\
  \ Lineage Link Help support community\n  issuer: https://lineagelinkhelp.onelineage.com/support\n  openIdConnectUrl: https://lineagelinkhelp.onelineage.com/.well-known/openid-configuration\n  authorization_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/authorize\n  token_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/token\n  userinfo_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/userinfo\n  jwks_uri: https://lineagelinkhelp.onelineage.com/support/id/keys\n  revocation_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/revoke\n  introspection_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/introspect\n  registration_endpoint: https://lineagelinkhelp.onelineage.com/support/services/oauth2/register\n  id_token_signing_alg:\n  - RS256\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  sources:\n  - well-known/lineage-linkhelp-openid-configuration.json\n\
  customer_login: https://www.onelineage.com/customer-login\nrelated:\n- scopes/lineage-scopes.yml\n- well-known/lineage-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lineage/refs/heads/main/authentication/lineage-authentication.yml
summary_line: openIdConnect/oauth2 · 2 schemes
tags:
- Company
- Logistics
- Cold Chain
- Warehousing
- Supply Chain
- Temperature Controlled
- Freight
- Transportation
- Food and Beverage
- REIT
---
