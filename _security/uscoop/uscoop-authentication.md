---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Uscoop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: uScoop secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: uScoop
provider_slug: uscoop
scheme_count: 2
schemes:
- issuer: https://shopify.com/authentication/63049990366
  name: shopify-customer-accounts-oidc
  openIdConnectUrl: https://tnuck.com/.well-known/openid-configuration
  sources:
  - well-known/uscoop-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://shopify.com/authentication/63049990366/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://shopify.com/authentication/63049990366/oauth/token
  name: shopify-customer-accounts-oauth2
  sources:
  - well-known/uscoop-oauth-authorization-server.json
  type: oauth2
slug: uscoop-authentication
source_filename: uscoop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tnuck.com/.well-known/openid-configuration\ndocs: https://tnuck.com/.well-known/oauth-authorization-server\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://tnuck.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/63049990366\n  sources:\n  - well-known/uscoop-openid-configuration.json\n- name: shopify-customer-accounts-oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/63049990366/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/63049990366/oauth/token\n  sources:\n  - well-known/uscoop-oauth-authorization-server.json\nnotes:\n- Customer-account authentication is delegated to Shopify (issuer\n  shopify.com/authentication/63049990366); discovery documents were\
  \ fetched\n  live from tnuck.com on 2026-07-21.\n- The UCP MCP commerce endpoint additionally requires an agent profile URI\n  (see mcp/uscoop-mcp.yml probe).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uscoop/refs/heads/main/authentication/uscoop-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Retail
- Fashion
- eCommerce
- Agentic Commerce
- Shopping
---
