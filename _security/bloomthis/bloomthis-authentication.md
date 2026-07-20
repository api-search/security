---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Bloomthis Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: BloomThis secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: BloomThis
provider_slug: bloomthis
scheme_count: 2
schemes:
- authorization_endpoint: https://shopify.com/authentication/7814423/oauth/authorize
  code_challenge_methods_supported:
  - S256
  end_session_endpoint: https://shopify.com/authentication/7814423/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/7814423
  jwks_uri: https://shopify.com/authentication/7814423/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://bloomthis.co/.well-known/openid-configuration
  sources:
  - well-known/bloomthis-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/7814423/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
- description: Agent-driven checkout through the UCP MCP endpoint requires contemporaneous buyer approval at the moment of payment; agents must not complete payment without explicit consent.
  name: UCPBuyerApproval
  sources:
  - well-known/bloomthis-ucp.json
  - llms/bloomthis-llms.txt
  type: consent
slug: bloomthis-authentication
source_filename: bloomthis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://bloomthis.co/.well-known/openid-configuration\nnotes: >-\n  Auth is provided by the Shopify Customer Account API (OpenID Connect / OAuth 2.0),\n  discovered live at /.well-known/openid-configuration and /.well-known/oauth-authorization-server.\n  The UCP MCP shopping endpoint layers buyer-approval consent on top for agent-driven checkout.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  issuer: https://shopify.com/authentication/7814423\n  openIdConnectUrl: https://bloomthis.co/.well-known/openid-configuration\n  authorization_endpoint: https://shopify.com/authentication/7814423/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/7814423/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/7814423/logout\n\
  \  jwks_uri: https://shopify.com/authentication/7814423/.well-known/jwks.json\n  token_endpoint_auth_methods_supported: [client_secret_basic]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [S256]\n  sources: [well-known/bloomthis-openid-configuration.json]\n- name: UCPBuyerApproval\n  type: consent\n  description: >-\n    Agent-driven checkout through the UCP MCP endpoint requires contemporaneous buyer\n    approval at the moment of payment; agents must not complete payment without explicit consent.\n  sources: [well-known/bloomthis-ucp.json, llms/bloomthis-llms.txt]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomthis/refs/heads/main/authentication/bloomthis-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Flowers
- Gifting
- Ecommerce
- Retail
- Shopify
- Agent Commerce
- MCP
- Malaysia
---
