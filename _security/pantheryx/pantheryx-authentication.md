---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Pantheryx Authentication
name_suffix: Authentication
oauth_flows: []
overview: PanTheryx declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: PanTheryx
provider_slug: pantheryx
scheme_count: 3
schemes:
- applies_to: relesium.com
  authorization_endpoint: https://account.relesium.com/authentication/oauth/authorize
  discovery:
  - /.well-known/openid-configuration
  - /.well-known/oauth-authorization-server
  - /.well-known/oauth-protected-resource
  end_session_endpoint: https://account.relesium.com/authentication/logout
  id: shopify_customer_account_oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/60191506528
  jwks_uri: https://account.relesium.com/authentication/.well-known/jwks.json
  note: A customer-account identity provider, not a partner/developer API program. It authenticates shoppers, not integrators.
  response_types_supported:
  - code
  token_endpoint: https://account.relesium.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to: www.lifesfirstnaturals.com
  authorization_endpoint: https://shopify.com/authentication/27073282091/oauth/authorize
  id: shopify_customer_account_oidc_lfn
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/27073282091
  jwks_uri: https://shopify.com/authentication/27073282091/.well-known/jwks.json
  response_types_supported:
  - code
  token_endpoint: https://shopify.com/authentication/27073282091/oauth/token
  type: openIdConnect
- applies_to: checkout completion
  handlers:
  - com.google.pay
  - dev.shopify.card
  - dev.shopify.shop_pay
  id: ucp_payment_instrument
  note: complete_checkout is not authenticated with an API key; it carries a payment instrument and, per each store's published llms.txt, requires contemporaneous buyer approval.
  type: payment-credential
slug: pantheryx-authentication
source_filename: pantheryx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://relesium.com/.well-known/oauth-authorization-server (200),\n  https://relesium.com/.well-known/oauth-protected-resource (200),\n  https://www.lifesfirstnaturals.com/.well-known/openid-configuration (200), and an anonymous\n  JSON-RPC tools/list POST to each store's /api/ucp/mcp endpoint (200, no credential sent).\nsummary: >-\n  PanTheryx publishes no API keys, no developer signup and no authentication documentation of its\n  own. The only authenticated surface on any PanTheryx-controlled host is the Shopify customer\n  account OAuth 2.0 / OpenID Connect provider that fronts the two brand storefronts. Agent\n  discovery on those storefronts is fully anonymous: tools/list, the UCP merchant profile, the\n  catalog JSON endpoints and llms.txt all answer with no token.\nanonymous_surface:\n- surface: MCP tools/list\n  endpoints:\n  - https://relesium.com/api/ucp/mcp\n  - https://www.lifesfirstnaturals.com/api/ucp/mcp\n\
  \  credential_required: false\n  observed_status: 200\n- surface: UCP merchant profile\n  endpoints:\n  - https://relesium.com/.well-known/ucp\n  - https://www.lifesfirstnaturals.com/.well-known/ucp\n  credential_required: false\n  observed_status: 200\nschemes:\n- id: shopify_customer_account_oidc\n  type: openIdConnect\n  applies_to: relesium.com\n  issuer: https://shopify.com/authentication/60191506528\n  authorization_endpoint: https://account.relesium.com/authentication/oauth/authorize\n  token_endpoint: https://account.relesium.com/authentication/oauth/token\n  jwks_uri: https://account.relesium.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.relesium.com/authentication/logout\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  discovery:\n  - /.well-known/openid-configuration\n  - /.well-known/oauth-authorization-server\n\
  \  - /.well-known/oauth-protected-resource\n  note: >-\n    A customer-account identity provider, not a partner/developer API program. It authenticates\n    shoppers, not integrators.\n- id: shopify_customer_account_oidc_lfn\n  type: openIdConnect\n  applies_to: www.lifesfirstnaturals.com\n  issuer: https://shopify.com/authentication/27073282091\n  authorization_endpoint: https://shopify.com/authentication/27073282091/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/27073282091/oauth/token\n  jwks_uri: https://shopify.com/authentication/27073282091/.well-known/jwks.json\n  response_types_supported:\n  - code\n  id_token_signing_alg_values_supported:\n  - RS256\n- id: ucp_payment_instrument\n  type: payment-credential\n  applies_to: checkout completion\n  handlers:\n  - com.google.pay\n  - dev.shopify.card\n  - dev.shopify.shop_pay\n  note: >-\n    complete_checkout is not authenticated with an API key; it carries a payment instrument and,\n    per each store's published\
  \ llms.txt, requires contemporaneous buyer approval.\nbearer_methods_supported:\n- header\ngaps:\n- No API key issuance, no developer console, no partner authentication documentation.\n- No first-party authentication page exists on pantheryx.com; every document above is Shopify-served.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pantheryx/refs/heads/main/authentication/pantheryx-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Nutrition
- Biotechnology
- Life Sciences
- Consumer Health
- Dietary Supplements
- Colostrum
- Animal Health
- E-Commerce
- Agentic Commerce
---
