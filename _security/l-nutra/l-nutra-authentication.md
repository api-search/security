---
api_key_in: []
auth_types: []
description: L-Nutra has two distinct authentication postures and they are not the same. The agentic-commerce MCP surface is completely anonymous — a tools/list POST to /api/ucp/mcp and /api/mcp on all three storefronts returned HTTP 200 with a full tool set and no OAuth challenge, and there is no /.well-known/oauth-protected-resource on any host. Separately, each storefront serves Shopify customer-account OIDC discovery, an authorization-code + PKCE flow used by shoppers to sign into their own account — that is a human login, not an API credential the store issues to developers. L-Nutra publishes no API keys, no developer registration, and no client-credentials flow.
kind: authentication
layout: security
method: probed
name: L Nutra Authentication
name_suffix: Authentication
oauth_flows: []
overview: L-Nutra declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: L-Nutra
provider_slug: l-nutra
scheme_count: 2
schemes:
- applies_to:
  - https://prolonlife.com/api/ucp/mcp
  - https://prolonlife.com/api/mcp
  - https://l-nutrahealth.com/api/ucp/mcp
  - https://l-nutrahealth.com/api/mcp
  - https://l-nutraprofessional.com/api/ucp/mcp
  - https://l-nutraprofessional.com/api/mcp
  evidence: tools/list returned HTTP 200 with a populated result on every endpoint, 2026-08-23.
  name: anonymous-mcp
  note: The only thing standing between an agent and a completed purchase is store policy, not a credential — payment completion requires contemporaneous human approval per robots.txt and llms.txt. UCP does require a meta['ucp-agent'].profile URI on every call, but that is an agent self-description, not an authenticated identity.
  type: none
- applies_to:
  - https://prolonlife.com
  - https://l-nutrahealth.com
  - https://l-nutraprofessional.com
  authorization_endpoint: https://account.<storefront-domain>/authentication/oauth/authorize
  claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  code_challenge_methods_supported:
  - S256
  discovery: /.well-known/openid-configuration
  end_session_endpoint: https://account.<storefront-domain>/authentication/logout
  grant_types_supported:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/<shop-id>
  jwks_uri: https://account.<storefront-domain>/authentication/.well-known/jwks.json
  name: shopify-customer-accounts-oidc
  note: Shopify-operated identity for the merchant's own customer accounts. The issuer is shopify.com; only the OAuth endpoints are on an L-Nutra subdomain. No public client registration is offered, so a third-party developer cannot obtain a client_id here.
  response_types_supported:
  - code
  scopes: see scopes/l-nutra-scopes.yml
  subject_types_supported:
  - public
  token_endpoint: https://account.<storefront-domain>/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: l-nutra-authentication
source_filename: l-nutra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: >-\n  https://prolonlife.com/.well-known/openid-configuration,\n  https://prolonlife.com/.well-known/oauth-authorization-server, and live tools/list probes of\n  https://prolonlife.com/api/ucp/mcp and https://prolonlife.com/api/mcp\ndescription: >-\n  L-Nutra has two distinct authentication postures and they are not the same. The agentic-commerce\n  MCP surface is completely anonymous — a tools/list POST to /api/ucp/mcp and /api/mcp on all three\n  storefronts returned HTTP 200 with a full tool set and no OAuth challenge, and there is no\n  /.well-known/oauth-protected-resource on any host. Separately, each storefront serves Shopify\n  customer-account OIDC discovery, an authorization-code + PKCE flow used by shoppers to sign into\n  their own account — that is a human login, not an API credential the store issues to developers.\n  L-Nutra publishes no API keys, no developer registration, and no client-credentials flow.\nschemes:\n\
  - name: anonymous-mcp\n  type: none\n  applies_to:\n  - https://prolonlife.com/api/ucp/mcp\n  - https://prolonlife.com/api/mcp\n  - https://l-nutrahealth.com/api/ucp/mcp\n  - https://l-nutrahealth.com/api/mcp\n  - https://l-nutraprofessional.com/api/ucp/mcp\n  - https://l-nutraprofessional.com/api/mcp\n  evidence: tools/list returned HTTP 200 with a populated result on every endpoint, 2026-08-23.\n  note: >-\n    The only thing standing between an agent and a completed purchase is store policy, not a\n    credential — payment completion requires contemporaneous human approval per robots.txt and\n    llms.txt. UCP does require a meta['ucp-agent'].profile URI on every call, but that is an agent\n    self-description, not an authenticated identity.\n- name: shopify-customer-accounts-oidc\n  type: openIdConnect\n  applies_to:\n  - https://prolonlife.com\n  - https://l-nutrahealth.com\n  - https://l-nutraprofessional.com\n  issuer: https://shopify.com/authentication/<shop-id>\n  discovery:\
  \ /.well-known/openid-configuration\n  authorization_endpoint: https://account.<storefront-domain>/authentication/oauth/authorize\n  token_endpoint: https://account.<storefront-domain>/authentication/oauth/token\n  end_session_endpoint: https://account.<storefront-domain>/authentication/logout\n  jwks_uri: https://account.<storefront-domain>/authentication/.well-known/jwks.json\n  response_types_supported: [code]\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [public]\n  claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n  scopes: see scopes/l-nutra-scopes.yml\n  note: >-\n    Shopify-operated identity for the merchant's own customer accounts. The issuer is\n    shopify.com; only the\
  \ OAuth endpoints are on an L-Nutra subdomain. No public client\n    registration is offered, so a third-party developer cannot obtain a client_id here.\ngaps:\n- No /.well-known/oauth-protected-resource on any host (RFC 9728), so the MCP endpoints declare no\n  protected-resource metadata — consistent with them being unauthenticated.\n- No API keys, no developer account, no documented credential issuance of any kind.\n- No documented auth page — the only auth surface described in prose is the shopper login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/l-nutra/refs/heads/main/authentication/l-nutra-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Nutrition
- Health
- Longevity
- Consumer Products
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
---
