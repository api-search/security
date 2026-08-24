---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Harmonya Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harmonya declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Harmonya
provider_slug: harmonya
scheme_count: 1
schemes:
- applies_to: The Harmonya tenant application backend at https://app.harmonya.com (VITE_SERVER_URL). Not a published API — no reference, no contract, no self-service key issuance.
  audience: https://app.harmonya.com
  flows:
    authorization_code:
      authorizationUrl: https://harmonya.us.auth0.com/authorize
      code_challenge_methods:
      - S256
      - plain
      note: The browser SPA uses auth0-spa-js with a public client (VITE_CLIENT_ID present in the bundle, no secret) — the standard Authorization Code + PKCE arrangement.
      pkce: true
      public_client: true
      tokenUrl: https://harmonya.us.auth0.com/oauth/token
    client_credentials:
      note: Advertised in grant_types_supported on the tenant. This is the machine-to-machine grant a customer integration would use, but Harmonya publishes no scope reference, no API reference, and no self-service path to a client_id/secret, so it cannot be exercised without an account and a sales conversation.
      tokenUrl: https://harmonya.us.auth0.com/oauth/token
  format: Bearer <JWT access token>
  header: Authorization
  id: auth0_oidc
  in: header
  openIdConnectUrl: https://harmonya.us.auth0.com/.well-known/openid-configuration
  scheme: oauth2
  type: openIdConnect
slug: harmonya-authentication
source_filename: harmonya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  https://harmonya.us.auth0.com/.well-known/openid-configuration (HTTP 200, 2026-08-22) and the\n  build-time environment block in https://app.harmonya.com/assets/fetchMock-VndaR4oo.js\n  (VITE_DOMAIN, VITE_AUDIENCE, VITE_SERVER_URL, VITE_CLIENT_ID).\nsummary: >-\n  Harmonya publishes no developer authentication documentation — there is no docs, developer or\n  api subdomain and no auth page on www.harmonya.com. What is recorded here was probed, not read\n  from a reference: the Harmonya tenant application at app.harmonya.com authenticates end users\n  against an Auth0 tenant (harmonya.us.auth0.com) using OAuth 2.0 / OpenID Connect with PKCE, and\n  presents the resulting access token to its own backend at https://app.harmonya.com. The tenant's\n  OIDC discovery document is anonymous and was saved verbatim to\n  well-known/harmonya-openid-configuration.json.\ndocumented_publicly: false\ndocs: null\nidentity_provider:\n  vendor:\
  \ Auth0 (Okta)\n  tenant: harmonya.us.auth0.com\n  issuer: https://harmonya.us.auth0.com/\n  discovery: https://harmonya.us.auth0.com/.well-known/openid-configuration\nschemes:\n- id: auth0_oidc\n  type: openIdConnect\n  scheme: oauth2\n  openIdConnectUrl: https://harmonya.us.auth0.com/.well-known/openid-configuration\n  in: header\n  header: Authorization\n  format: Bearer <JWT access token>\n  audience: https://app.harmonya.com\n  applies_to: >-\n    The Harmonya tenant application backend at https://app.harmonya.com (VITE_SERVER_URL). Not a\n    published API — no reference, no contract, no self-service key issuance.\n  flows:\n    authorization_code:\n      authorizationUrl: https://harmonya.us.auth0.com/authorize\n      tokenUrl: https://harmonya.us.auth0.com/oauth/token\n      pkce: true\n      code_challenge_methods: [S256, plain]\n      public_client: true\n      note: >-\n        The browser SPA uses auth0-spa-js with a public client (VITE_CLIENT_ID present in the\n        bundle,\
  \ no secret) — the standard Authorization Code + PKCE arrangement.\n    client_credentials:\n      tokenUrl: https://harmonya.us.auth0.com/oauth/token\n      note: >-\n        Advertised in grant_types_supported on the tenant. This is the machine-to-machine grant a\n        customer integration would use, but Harmonya publishes no scope reference, no API\n        reference, and no self-service path to a client_id/secret, so it cannot be exercised\n        without an account and a sales conversation.\ngrant_types_supported:\n- client_credentials\n- authorization_code\n- refresh_token\n- password\n- implicit\n- urn:ietf:params:oauth:grant-type:device_code\n- urn:ietf:params:oauth:grant-type:token-exchange\n- urn:ietf:params:oauth:grant-type:jwt-bearer\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n- none\nid_token_signing_alg_values_supported: [HS256, RS256, PS256]\nscopes_supported:\n- openid\n- profile\n- offline_access\n- email\n\
  - email_verified\n- name\n- given_name\n- family_name\n- nickname\n- picture\n- phone\n- address\n- created_at\n- identities\nscopes_note: >-\n  These are Auth0's default OIDC identity scopes on the tenant's discovery document, not Harmonya\n  API permission scopes. No product scope reference is published, so scopes/ is not written —\n  see the guidance that scopes/ is OAuth-only and must not be filled with an empty artifact.\nmfa:\n  endpoint: https://harmonya.us.auth0.com/mfa/challenge\n  note: Auth0 MFA challenge endpoint is present on the tenant; enrollment policy is not public.\ngaps:\n- No public authentication documentation of any kind.\n- No self-service credential issuance; the only published CTA is https://www.harmonya.com/get-a-demo.\n- No documented API scopes, no token lifetime statement, no rotation guidance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonya/refs/heads/main/authentication/harmonya-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Product Intelligence
- Product Data
- Data Enrichment
- Consumer Packaged Goods
- Retail
- Consumer Insights
- Retail Media
- Artificial Intelligence
---
