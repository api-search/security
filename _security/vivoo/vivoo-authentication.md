---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Vivoo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Vivoo secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Vivoo
provider_slug: vivoo
scheme_count: 1
schemes:
- authorization_endpoint: https://shopify.com/authentication/85119664427/oauth/authorize
  end_session_endpoint: https://shopify.com/authentication/85119664427/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/85119664427
  jwks_uri: https://shopify.com/authentication/85119664427/.well-known/jwks.json
  name: ShopifyCustomerAccountOIDC
  openIdConnectUrl: https://www.vivoo.io/.well-known/openid-configuration
  response_types_supported:
  - code
  sources:
  - well-known/vivoo-openid-configuration.json
  token_endpoint: https://shopify.com/authentication/85119664427/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  type: openIdConnect
slug: vivoo-authentication
source_filename: vivoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.vivoo.io/.well-known/openid-configuration\ndocs: https://shopify.dev/docs/api/customer\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    Vivoo runs on Shopify. Buyer/customer identity is served by the Shopify Customer\n    Account API via OpenID Connect (issuer https://shopify.com/authentication/85119664427).\n    Agent-driven commerce goes through the UCP shopping MCP server, where checkout\n    requires explicit human buyer approval rather than a machine credential. There is\n    no first-party developer API key program published by Vivoo itself.\nschemes:\n- name: ShopifyCustomerAccountOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://www.vivoo.io/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/85119664427\n  authorization_endpoint: https://shopify.com/authentication/85119664427/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/85119664427/oauth/token\n\
  \  jwks_uri: https://shopify.com/authentication/85119664427/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/85119664427/logout\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  sources:\n  - well-known/vivoo-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vivoo/refs/heads/main/authentication/vivoo-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Company
- Health
- Wellness
- Consumer Health
- Nutrition
- Diagnostics
- E-Commerce
- Agentic Commerce
- MCP
---
