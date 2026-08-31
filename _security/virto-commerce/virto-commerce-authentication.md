---
api_key_in:
- header
- query
api_specs:
- filename: virto-commerce-catalog-api-openapi.yml
  format: yaml
  label: Virto Commerce Catalog API
  slug: virto-commerce-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-catalog-api-openapi.yml
- filename: virto-commerce-companies-and-contacts-api-openapi.yml
  format: yaml
  label: Virto Commerce Companies and Contacts API
  slug: virto-commerce-companies-and-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-companies-and-contacts-api-openapi.yml
- filename: virto-commerce-inventory-api-openapi.yml
  format: yaml
  label: Virto Commerce Inventory API
  slug: virto-commerce-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-inventory-api-openapi.yml
- filename: virto-commerce-marketing-api-openapi.yml
  format: yaml
  label: Virto Commerce Marketing API
  slug: virto-commerce-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-marketing-api-openapi.yml
- filename: virto-commerce-order-management-api-openapi.yml
  format: yaml
  label: Virto Commerce Order Management API
  slug: virto-commerce-order-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-order-management-api-openapi.yml
- filename: virto-commerce-pricing-api-openapi.yml
  format: yaml
  label: Virto Commerce Pricing API
  slug: virto-commerce-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-pricing-api-openapi.yml
- filename: virto-commerce-quotes-api-openapi.yml
  format: yaml
  label: Virto Commerce Quotes API
  slug: virto-commerce-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-quotes-api-openapi.yml
- filename: virto-commerce-shopping-cart-api-openapi.yml
  format: yaml
  label: Virto Commerce Shopping Cart API
  slug: virto-commerce-shopping-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-shopping-cart-api-openapi.yml
- filename: virto-commerce-store-api-openapi.yml
  format: yaml
  label: Virto Commerce Store API
  slug: virto-commerce-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-store-api-openapi.yml
- filename: virto-commerce-virtocommerce-platform-api-openapi.yml
  format: yaml
  label: Virto Commerce VirtoCommerce Platform API
  slug: virto-commerce-virtocommerce-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
- filename: virto-commerce-webhooks-api-openapi.yml
  format: yaml
  label: Virto Commerce Webhooks API
  slug: virto-commerce-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-webhooks-api-openapi.yml
- filename: virto-commerce-returns-api-openapi.yml
  format: yaml
  label: Virto Commerce Returns API
  slug: virto-commerce-returns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-returns-api-openapi.yml
- filename: virto-commerce-event-bus-module-api-openapi.yml
  format: yaml
  label: Virto Commerce Event Bus module API
  slug: virto-commerce-event-bus-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/openapi/virto-commerce-event-bus-module-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Virto Commerce Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Virto Commerce secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Virto Commerce
provider_slug: virto-commerce
scheme_count: 5
schemes:
- description: OAuth2 Resource Owner Password Grant flow
  flows:
  - flow: password
    scopes: 0
    tokenUrl: /connect/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /connect/token
  name: oauth2
  sources:
  - openapi/virto-commerce-catalog-api-openapi.yml
  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml
  - openapi/virto-commerce-event-bus-api-openapi.yml
  - openapi/virto-commerce-inventory-api-openapi.yml
  - openapi/virto-commerce-marketing-api-openapi.yml
  - openapi/virto-commerce-order-management-api-openapi.yml
  - openapi/virto-commerce-pricing-api-openapi.yml
  - openapi/virto-commerce-quotes-api-openapi.yml
  - openapi/virto-commerce-returns-api-openapi.yml
  - openapi/virto-commerce-shopping-cart-api-openapi.yml
  - openapi/virto-commerce-store-api-openapi.yml
  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
  - openapi/virto-commerce-webhooks-api-openapi.yml
  type: oauth2
- description: API Key authentication
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/virto-commerce-catalog-api-openapi.yml
  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml
  - openapi/virto-commerce-event-bus-api-openapi.yml
  - openapi/virto-commerce-inventory-api-openapi.yml
  - openapi/virto-commerce-marketing-api-openapi.yml
  - openapi/virto-commerce-order-management-api-openapi.yml
  - openapi/virto-commerce-pricing-api-openapi.yml
  - openapi/virto-commerce-quotes-api-openapi.yml
  - openapi/virto-commerce-returns-api-openapi.yml
  - openapi/virto-commerce-shopping-cart-api-openapi.yml
  - openapi/virto-commerce-store-api-openapi.yml
  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
  - openapi/virto-commerce-webhooks-api-openapi.yml
  type: apiKey
- description: API Key authentication (alternative via header)
  in: header
  name: api_key_header
  parameter: api_key
  sources:
  - openapi/virto-commerce-catalog-api-openapi.yml
  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml
  - openapi/virto-commerce-event-bus-api-openapi.yml
  - openapi/virto-commerce-inventory-api-openapi.yml
  - openapi/virto-commerce-marketing-api-openapi.yml
  - openapi/virto-commerce-order-management-api-openapi.yml
  - openapi/virto-commerce-pricing-api-openapi.yml
  - openapi/virto-commerce-quotes-api-openapi.yml
  - openapi/virto-commerce-returns-api-openapi.yml
  - openapi/virto-commerce-shopping-cart-api-openapi.yml
  - openapi/virto-commerce-store-api-openapi.yml
  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
  - openapi/virto-commerce-webhooks-api-openapi.yml
  type: apiKey
- description: HTTP Signature authentication using Authorization header
  name: http-signature
  scheme: signature
  sources:
  - openapi/virto-commerce-catalog-api-openapi.yml
  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml
  - openapi/virto-commerce-event-bus-api-openapi.yml
  - openapi/virto-commerce-inventory-api-openapi.yml
  - openapi/virto-commerce-marketing-api-openapi.yml
  - openapi/virto-commerce-order-management-api-openapi.yml
  - openapi/virto-commerce-pricing-api-openapi.yml
  - openapi/virto-commerce-quotes-api-openapi.yml
  - openapi/virto-commerce-returns-api-openapi.yml
  - openapi/virto-commerce-shopping-cart-api-openapi.yml
  - openapi/virto-commerce-store-api-openapi.yml
  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
  - openapi/virto-commerce-webhooks-api-openapi.yml
  type: http
- description: Basic authentication using username and password
  name: basic
  scheme: basic
  sources:
  - openapi/virto-commerce-catalog-api-openapi.yml
  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml
  - openapi/virto-commerce-event-bus-api-openapi.yml
  - openapi/virto-commerce-inventory-api-openapi.yml
  - openapi/virto-commerce-marketing-api-openapi.yml
  - openapi/virto-commerce-order-management-api-openapi.yml
  - openapi/virto-commerce-pricing-api-openapi.yml
  - openapi/virto-commerce-quotes-api-openapi.yml
  - openapi/virto-commerce-returns-api-openapi.yml
  - openapi/virto-commerce-shopping-cart-api-openapi.yml
  - openapi/virto-commerce-store-api-openapi.yml
  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml
  - openapi/virto-commerce-webhooks-api-openapi.yml
  type: http
slug: virto-commerce-authentication
source_filename: virto-commerce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: 'openapi/virto-commerce-catalog-api-openapi.yml, openapi/virto-commerce-companies-and-contacts-api-openapi.yml,\n  openapi/virto-commerce-event-bus-api-openapi.yml, openapi/virto-commerce-inventory-api-openapi.yml,\n  openapi/virto-commerce-marketing-api-openapi.yml, openapi/virto-commerce-order-management-api-openapi.yml,\n  openapi/virto-commerce-pricing-api-openapi.yml, openapi/virto-commerce-quotes-api-openapi.yml, openapi/virto-commerce-returns-api-openapi.yml,\n  openapi/virto-commerce-shopping-cart-api-openapi.yml, openapi/virto-commerce-store-api-openapi.yml,\n  openapi/virto-commerce-virtocommerce-platform-api-openapi.yml ...\n\n  ; upgraded 2026-08-13 from the live discovery document https://virtostart-demo-admin.govirto.com/.well-known/openid-configuration\n  (HTTP 200, captured in well-known/virto-commerce-openid-configuration.json) and https://docs.virtocommerce.org/platform/developer-guide/Fundamentals/Security/authentication/api-key-authentication/'\n\
  summary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - clientCredentials\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /connect/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: /connect/token\n    scopes: 0\n  description: OAuth2 Resource Owner Password Grant flow\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n  - openapi/virto-commerce-inventory-api-openapi.yml\n  - openapi/virto-commerce-marketing-api-openapi.yml\n  - openapi/virto-commerce-order-management-api-openapi.yml\n  - openapi/virto-commerce-pricing-api-openapi.yml\n  - openapi/virto-commerce-quotes-api-openapi.yml\n  - openapi/virto-commerce-returns-api-openapi.yml\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n  - openapi/virto-commerce-store-api-openapi.yml\n\
  \  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API Key authentication\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n  - openapi/virto-commerce-inventory-api-openapi.yml\n  - openapi/virto-commerce-marketing-api-openapi.yml\n  - openapi/virto-commerce-order-management-api-openapi.yml\n  - openapi/virto-commerce-pricing-api-openapi.yml\n  - openapi/virto-commerce-quotes-api-openapi.yml\n  - openapi/virto-commerce-returns-api-openapi.yml\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n  - openapi/virto-commerce-store-api-openapi.yml\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- name: api_key_header\n  type: apiKey\n\
  \  in: header\n  parameter: api_key\n  description: API Key authentication (alternative via header)\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n  - openapi/virto-commerce-inventory-api-openapi.yml\n  - openapi/virto-commerce-marketing-api-openapi.yml\n  - openapi/virto-commerce-order-management-api-openapi.yml\n  - openapi/virto-commerce-pricing-api-openapi.yml\n  - openapi/virto-commerce-quotes-api-openapi.yml\n  - openapi/virto-commerce-returns-api-openapi.yml\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n  - openapi/virto-commerce-store-api-openapi.yml\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- name: http-signature\n  type: http\n  scheme: signature\n  description: HTTP Signature authentication using Authorization header\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n\
  \  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n  - openapi/virto-commerce-inventory-api-openapi.yml\n  - openapi/virto-commerce-marketing-api-openapi.yml\n  - openapi/virto-commerce-order-management-api-openapi.yml\n  - openapi/virto-commerce-pricing-api-openapi.yml\n  - openapi/virto-commerce-quotes-api-openapi.yml\n  - openapi/virto-commerce-returns-api-openapi.yml\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n  - openapi/virto-commerce-store-api-openapi.yml\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n  - openapi/virto-commerce-webhooks-api-openapi.yml\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic authentication using username and password\n  sources:\n  - openapi/virto-commerce-catalog-api-openapi.yml\n  - openapi/virto-commerce-companies-and-contacts-api-openapi.yml\n  - openapi/virto-commerce-event-bus-api-openapi.yml\n  - openapi/virto-commerce-inventory-api-openapi.yml\n\
  \  - openapi/virto-commerce-marketing-api-openapi.yml\n  - openapi/virto-commerce-order-management-api-openapi.yml\n  - openapi/virto-commerce-pricing-api-openapi.yml\n  - openapi/virto-commerce-quotes-api-openapi.yml\n  - openapi/virto-commerce-returns-api-openapi.yml\n  - openapi/virto-commerce-shopping-cart-api-openapi.yml\n  - openapi/virto-commerce-store-api-openapi.yml\n  - openapi/virto-commerce-virtocommerce-platform-api-openapi.yml\n  - openapi/virto-commerce-webhooks-api-openapi.yml\ndocs: https://docs.virtocommerce.org/platform/developer-guide/Fundamentals/Security/authentication/api-key-authentication/\ndeployment_note: 'Virto Commerce is self-hosted: the authorization server is the operator''s own platform\n  instance, running OpenIddict. All endpoints below are relative to that host. The issuer recorded here\n  is Virto''s own public reference deployment.'\ndiscovery:\n  openid_configuration: well-known/virto-commerce-openid-configuration.json\n  oauth_authorization_server:\
  \ well-known/virto-commerce-oauth-authorization-server.json\n  issuer: https://virtostart-demo-admin.govirto.com/\n  authorization_endpoint: /connect/authorize\n  token_endpoint: /connect/token\n  userinfo_endpoint: /connect/userinfo\n  end_session_endpoint: /connect/logout\n  jwks_uri: /.well-known/jwks\n  jwks_note: Non-conventional path — /.well-known/jwks, not jwks.json. Served, HTTP 200.\n  grant_types_supported:\n  - password\n  - refresh_token\n  - client_credentials\n  - authorization_code\n  - impersonate\n  - external_sign_in\n  grant_types_note: impersonate and external_sign_in are Virto-specific grants beyond the four the OpenAPI\n    declares; the spec only shows password and client_credentials.\n  code_challenge_methods_supported:\n  - plain\n  - S256\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - private_key_jwt\n  - client_secret_basic\n  id_token_signing_alg_values_supported:\n  - RS256\n  response_types_supported:\n  - code\n  scopes_supported:\n\
  \  - openid\n  - offline_access\n  require_pushed_authorization_requests: false\n  mtls_bound_tokens: false\napi_key:\n  schemes:\n  - api_key_header (header)\n  - api_key (query string)\n  recommended: api_key_header\n  warning: The query-string variant places a credential in access logs and proxy history; prefer the header.\n  used_by: Virto's own MCP adapter authenticates with a platform API key in the api_key header.\nauthorization_model:\n  mechanism: platform permissions, not OAuth scopes\n  note: scopes_supported is openid + offline_access only. Access control is Virto's fine-grained permission\n    system — colon-namespaced strings such as webhooks:read, webhooks:update, webhooks:feed:read — granted\n    to roles. Permissions are NOT expressed in the OpenAPI, so a client cannot discover the permission\n    an operation needs; a 403 comes back with an empty body.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virto-commerce/refs/heads/main/authentication/virto-commerce-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- B2B E-Commerce
- Catalog Management
- Order Management
- Pricing
- Inventory
- Shopping Cart
- Customer Management
- Marketing
- Payments
- Shipping
- Subscription
- Headless Commerce
- Open-Source
- .NET
- Webhook
- Event-Driven
- CloudEvents
- GraphQL
- Returns
- MCP
- B2B Quotes
---
