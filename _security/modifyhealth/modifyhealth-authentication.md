---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Modifyhealth Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ModifyHealth secures its APIs with none, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ModifyHealth
provider_slug: modifyhealth
scheme_count: 3
schemes:
- detail: The MCP endpoint requires no credential. tools/list returns HTTP 200 with all 13 tools and full inputSchemas anonymously. Tool invocation requires a meta.ucp-agent profile URI, which is an agent identity hint for UCP discovery, not a secret.
  name: ucp-mcp-anonymous
  sources:
  - mcp/modifyhealth-mcp-tools.json
  surface: https://modifyhealth.com/api/ucp/mcp
  type: none
- detail: Customer-account sign-in for the ModifyHealth storefront, delegated to Shopify as the authorization server. The oauth-protected-resource document served at modifyhealth.com names resource https://modifyhealth.com with authorization_servers [https://shopify.com/authentication/7887683702], which is what makes the cross-domain issuer legitimate rather than a mismatch.
  issuer: https://shopify.com/authentication/7887683702
  name: shopify-customer-account-oidc
  openIdConnectUrl: https://modifyhealth.com/.well-known/openid-configuration
  sources:
  - well-known/modifyhealth-openid-configuration.json
  - well-known/modifyhealth-oauth-protected-resource.json
  type: openIdConnect
- bearer_methods_supported:
  - header
  end_session_endpoint: https://shopify.com/authentication/7887683702/logout
  flows:
  - authorizationUrl: https://shopify.com/authentication/7887683702/oauth/authorize
    flow: authorizationCode
    scope_count: 4
    tokenUrl: https://shopify.com/authentication/7887683702/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg:
  - RS256
  jwks_uri: https://shopify.com/authentication/7887683702/.well-known/jwks.json
  name: shopify-customer-account-oauth2
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  sources:
  - well-known/modifyhealth-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: modifyhealth-authentication
source_filename: modifyhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://modifyhealth.com/.well-known/openid-configuration,\n  /.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource,\n  and live tools/list on https://modifyhealth.com/api/ucp/mcp\nnote: >-\n  Derived by hand from probed discovery documents, not from an OpenAPI: ModifyHealth\n  publishes no spec, so 0-working/derive-authentication.py had nothing to read. Two\n  distinct auth surfaces exist and must not be conflated.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ucp-mcp-anonymous\n  type: none\n  surface: https://modifyhealth.com/api/ucp/mcp\n  detail: >-\n    The MCP endpoint requires no credential. tools/list returns HTTP 200 with all 13\n    tools and full inputSchemas anonymously. Tool invocation requires a meta.ucp-agent\n    profile URI, which is an agent identity hint for UCP discovery, not a secret.\n\
  \  sources:\n  - mcp/modifyhealth-mcp-tools.json\n- name: shopify-customer-account-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://modifyhealth.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/7887683702\n  detail: >-\n    Customer-account sign-in for the ModifyHealth storefront, delegated to Shopify as the\n    authorization server. The oauth-protected-resource document served at\n    modifyhealth.com names resource https://modifyhealth.com with authorization_servers\n    [https://shopify.com/authentication/7887683702], which is what makes the cross-domain\n    issuer legitimate rather than a mismatch.\n  sources:\n  - well-known/modifyhealth-openid-configuration.json\n  - well-known/modifyhealth-oauth-protected-resource.json\n- name: shopify-customer-account-oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://shopify.com/authentication/7887683702/oauth/authorize\n    tokenUrl: https://shopify.com/authentication/7887683702/oauth/token\n\
  \    scope_count: 4\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  pkce:\n    supported: true\n    code_challenge_methods:\n    - S256\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  jwks_uri: https://shopify.com/authentication/7887683702/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/7887683702/logout\n  bearer_methods_supported:\n  - header\n  sources:\n  - well-known/modifyhealth-oauth-authorization-server.json\nhuman_signin: https://modifyhealth.com/account/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modifyhealth/refs/heads/main/authentication/modifyhealth-authentication.yml
summary_line: none/oauth2/openIdConnect · 3 schemes
tags:
- Health
- Food and Beverage
- Nutrition
- Meal Delivery
- Food as Medicine
- eCommerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Direct to Consumer
---
