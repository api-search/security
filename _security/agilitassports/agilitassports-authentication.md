---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Agilitassports Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agilitas Sports declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Agilitas Sports
provider_slug: agilitassports
scheme_count: 4
schemes:
- detail: 'No Authorization header is sent or accepted on the UCP MCP endpoint. Probed anonymously on 2026-09-12: initialize HTTP 200, tools/list HTTP 200 returning all 13 tools with full input schemas. Also anonymous on https://agilitas.com/api/mcp (storefront policy/FAQ server).'
  id: none
  required: false
  surface: Agilitas Commerce MCP API (https://agilitas.com/api/ucp/mcp)
  type: none
- applies_to: all 13 UCP tools
  detail: 'Not authentication and not authorization — the server does not issue or verify a secret — but it IS a hard gate. Every tool declares meta and meta.ucp-agent.profile as required, and a call that omits it is rejected before tool logic runs with JSON-RPC error -32001 "UCP discovery failed", data.code "invalid_profile_url", data.content "Unable to fetch agent profile: Missing profile uri". Observed live on tools/call, prompts/list and resources/list.'
  evidence:
    http_status: 200
    probed: '2026-09-12'
    url: https://agilitas.com/api/ucp/mcp
  field: meta.ucp-agent.profile
  format: URI
  id: ucp-agent-profile
  required: true
  surface: Agilitas Commerce MCP API
  type: caller-identity
- detail: Payment is carried per-call as a checkout payment instrument (handler_id + credential token), not as a server credential the agent holds. Declared handlers in the UCP profile are com.google.pay (gateway "shopify", gatewayMerchantId 99796025642) and dev.shopify.card accepting visa, master, american_express, discover and diners_club. Apple Pay token shape is present in the schema branch but no apple-pay handler is advertised in this store's UCP profile.
  human_approval_required: true
  human_approval_source: https://agilitas.com/llms.txt and https://agilitas.com/robots.txt both state that checkout, payment and order placement must not be completed by an agent without an explicit, contemporaneous human approval step.
  id: buyer-payment-instrument
  required: true for complete_checkout
  surface: Agilitas Commerce MCP API — checkout
  type: buyer-supplied credential
- authorization_endpoint: https://shopify.com/authentication/99796025642/oauth/authorize
  detail: Discovery documents are served on the Agilitas domain, but every endpoint they name lives on shopify.com and the operator policy/terms URIs in the document are Shopify's (op_policy_uri https://www.shopify.com/legal/privacy, op_tos_uri https://www.shopify.com/legal/terms). This is Shopify's customer-account identity provider for this shop, offered to shoppers, not a developer OAuth program Agilitas runs. No client registration path is published, and there is no public client_id for third-party integrators.
  discovery: https://agilitas.com/.well-known/openid-configuration
  end_session_endpoint: https://shopify.com/authentication/99796025642/logout
  flows:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: oauth2-oidc-customer-account
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/99796025642
  jwks_uri: https://shopify.com/authentication/99796025642/.well-known/jwks.json
  note: The customer-account-mcp-api:full scope indicates a Shopify-side authenticated customer MCP API exists as a product; nothing on an Agilitas host advertises or documents it and it was not probed because it requires a customer token.
  pkce: S256
  protected_resource_metadata: https://agilitas.com/.well-known/oauth-protected-resource
  rfc9728: true
  scopes_supported:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  surface: Shopify customer account (shopper sign-in), not the agent API
  token_endpoint: https://shopify.com/authentication/99796025642/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: agilitassports-authentication
source_filename: agilitassports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://agilitas.com/.well-known/openid-configuration (200),\n  https://agilitas.com/.well-known/oauth-protected-resource (200),\n  https://agilitas.com/.well-known/ucp (200), live MCP initialize + tools/list on\n  https://agilitas.com/api/ucp/mcp (200), https://agilitas.com/llms.txt (200)\nname: Agilitas authentication profile\nslug: agilitassports\n\nsummary: >-\n  There is no developer API program, so there is no API key, no client registration and no developer\n  credential of any kind. The agent commerce surface is deliberately anonymous at the transport\n  layer: initialize, tools/list, catalog search, cart and checkout creation all answer without a\n  token. What is required instead is agent IDENTITY (a UCP agent profile URI on every call) and, at\n  the moment money moves, a buyer-supplied payment instrument plus contemporaneous human approval.\n  A separate OAuth 2.0 / OpenID Connect authorization server exists\
  \ for shoppers signing in to their\n  own customer account; it is Shopify-operated and is not an API-access mechanism.\n\nschemes:\n- id: none\n  surface: Agilitas Commerce MCP API (https://agilitas.com/api/ucp/mcp)\n  type: none\n  required: false\n  detail: >-\n    No Authorization header is sent or accepted on the UCP MCP endpoint. Probed anonymously on\n    2026-09-12: initialize HTTP 200, tools/list HTTP 200 returning all 13 tools with full input\n    schemas. Also anonymous on https://agilitas.com/api/mcp (storefront policy/FAQ server).\n\n- id: ucp-agent-profile\n  surface: Agilitas Commerce MCP API\n  type: caller-identity\n  required: true\n  field: meta.ucp-agent.profile\n  format: URI\n  applies_to: all 13 UCP tools\n  detail: >-\n    Not authentication and not authorization — the server does not issue or verify a secret — but it\n    IS a hard gate. Every tool declares meta and meta.ucp-agent.profile as required, and a call that\n    omits it is rejected before tool logic runs\
  \ with JSON-RPC error -32001 \"UCP discovery failed\",\n    data.code \"invalid_profile_url\", data.content \"Unable to fetch agent profile: Missing profile\n    uri\". Observed live on tools/call, prompts/list and resources/list.\n  evidence:\n    probed: '2026-09-12'\n    url: https://agilitas.com/api/ucp/mcp\n    http_status: 200\n\n- id: buyer-payment-instrument\n  surface: Agilitas Commerce MCP API — checkout\n  type: buyer-supplied credential\n  required: true for complete_checkout\n  detail: >-\n    Payment is carried per-call as a checkout payment instrument (handler_id + credential token),\n    not as a server credential the agent holds. Declared handlers in the UCP profile are\n    com.google.pay (gateway \"shopify\", gatewayMerchantId 99796025642) and dev.shopify.card accepting\n    visa, master, american_express, discover and diners_club. Apple Pay token shape is present in\n    the schema branch but no apple-pay handler is advertised in this store's UCP profile.\n  human_approval_required:\
  \ true\n  human_approval_source: >-\n    https://agilitas.com/llms.txt and https://agilitas.com/robots.txt both state that checkout,\n    payment and order placement must not be completed by an agent without an explicit,\n    contemporaneous human approval step.\n\n- id: oauth2-oidc-customer-account\n  surface: Shopify customer account (shopper sign-in), not the agent API\n  type: oauth2\n  flows:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  pkce: S256\n  issuer: https://shopify.com/authentication/99796025642\n  authorization_endpoint: https://shopify.com/authentication/99796025642/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/99796025642/oauth/token\n  jwks_uri: https://shopify.com/authentication/99796025642/.well-known/jwks.json\n  end_session_endpoint: https://shopify.com/authentication/99796025642/logout\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n\
  \  - RS256\n  scopes_supported:\n  - openid\n  - email\n  - customer-account-api:full\n  - customer-account-mcp-api:full\n  discovery: https://agilitas.com/.well-known/openid-configuration\n  protected_resource_metadata: https://agilitas.com/.well-known/oauth-protected-resource\n  rfc9728: true\n  detail: >-\n    Discovery documents are served on the Agilitas domain, but every endpoint they name lives on\n    shopify.com and the operator policy/terms URIs in the document are Shopify's\n    (op_policy_uri https://www.shopify.com/legal/privacy, op_tos_uri\n    https://www.shopify.com/legal/terms). This is Shopify's customer-account identity provider for\n    this shop, offered to shoppers, not a developer OAuth program Agilitas runs. No client\n    registration path is published, and there is no public client_id for third-party integrators.\n  note: >-\n    The customer-account-mcp-api:full scope indicates a Shopify-side authenticated customer MCP API\n    exists as a product; nothing on\
  \ an Agilitas host advertises or documents it and it was not\n    probed because it requires a customer token.\n\nnot_present:\n- api_keys\n- bearer_tokens_for_the_agent_surface\n- mutual_tls\n- hmac_request_signing\n- developer_client_registration\n- partner_or_sandbox_credentials\n\ncross_links:\n  scopes: scopes/agilitassports-scopes.yml\n  conventions: conventions/agilitassports-conventions.yml\n  well_known: well-known/agilitassports-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilitassports/refs/heads/main/authentication/agilitassports-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Commerce
- E-Commerce
- Retail
- Sportswear
- Footwear
- Athleisure
- Manufacturing
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- India
---
