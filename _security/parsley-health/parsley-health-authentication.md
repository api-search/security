---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Parsley Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Parsley Health declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Parsley Health
provider_slug: parsley-health
scheme_count: 4
schemes:
- applies_to:
  - https://store.parsleyhealth.com/api/ucp/mcp (tools/list, initialize)
  - https://store.parsleyhealth.com/api/2026-01/graphql.json (introspection + public storefront reads)
  - https://store.parsleyhealth.com/products.json and the other storefront JSON endpoints
  evidence: All returned HTTP 200 with no Authorization header on 2026-08-15.
  id: none-anonymous
  type: none
- applies_to:
  - https://store.parsleyhealth.com/api/ucp/mcp
  description: Not authentication in the credential sense — every UCP tool call must carry meta.ucp-agent.profile, a resolvable agent profile URI identifying the calling agent. Omitting it returns JSON-RPC error -32001 "UCP discovery failed" with data.code invalid_profile_url.
  evidence: Observed on resources/list and prompts/list probes, 2026-08-15.
  id: ucp-agent-profile
  type: agent-identity
- applies_to:
  - Parsley Health store customer accounts
  authorization_endpoint: https://shopify.com/authentication/24996151350/oauth/authorize
  discovery:
  - https://store.parsleyhealth.com/.well-known/openid-configuration
  - https://store.parsleyhealth.com/.well-known/oauth-authorization-server
  end_session_endpoint: https://shopify.com/authentication/24996151350/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: oauth2-oidc-shopify
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/24996151350
  jwks_uri: https://shopify.com/authentication/24996151350/.well-known/jwks.json
  note: The discovery documents are served from Parsley Health's hostname but the issuer is Shopify's per-shop authorization server for shop 24996151350. Parsley Health does not operate this authorization server; it is inherited from the commerce platform.
  pkce:
  - S256
  response_types:
  - code
  scopes:
  - openid
  - email
  - customer-account-api:full
  - customer-account-mcp-api:full
  scopes_artifact: scopes/parsley-health-scopes.yml
  token_endpoint: https://shopify.com/authentication/24996151350/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- applies_to:
  - https://my.parsleyhealth.com
  - https://app.parsleyhealth.com
  description: Authenticated member application for clinical care. Single-page app behind a catch-all that returns HTTP 200 text/html for every path, including /.well-known/* and /openapi.json. No auth metadata, no token endpoint, no machine-readable contract is discoverable.
  evidence: Probed 2026-08-15 and 2026-08-02; all responses are the app shell.
  id: member-app-login
  type: opaque
slug: parsley-health-authentication
source_filename: parsley-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  https://store.parsleyhealth.com/.well-known/openid-configuration (HTTP 200),\n  https://store.parsleyhealth.com/.well-known/oauth-authorization-server (HTTP 200),\n  live anonymous probes of https://store.parsleyhealth.com/api/ucp/mcp and\n  https://store.parsleyhealth.com/api/2026-01/graphql.json (2026-08-15)\nnote: >-\n  Parsley Health publishes no developer authentication documentation and issues no API\n  keys. The auth model recorded here is the one that is actually observable on its public\n  hosts: an OAuth 2.0 / OpenID Connect authorization server delegated to Shopify for the\n  supplement store's customer accounts, plus two surfaces that need no credential at all.\n  The medical practice's member application (my.parsleyhealth.com) is a separate,\n  authenticated single-page app with no documented or discoverable auth contract — its\n  login is a human flow, not an API.\nschemes:\n- id: none-anonymous\n  type: none\n\
  \  applies_to:\n  - https://store.parsleyhealth.com/api/ucp/mcp (tools/list, initialize)\n  - https://store.parsleyhealth.com/api/2026-01/graphql.json (introspection + public storefront reads)\n  - https://store.parsleyhealth.com/products.json and the other storefront JSON endpoints\n  evidence: All returned HTTP 200 with no Authorization header on 2026-08-15.\n- id: ucp-agent-profile\n  type: agent-identity\n  applies_to: [https://store.parsleyhealth.com/api/ucp/mcp]\n  description: >-\n    Not authentication in the credential sense — every UCP tool call must carry\n    meta.ucp-agent.profile, a resolvable agent profile URI identifying the calling agent.\n    Omitting it returns JSON-RPC error -32001 \"UCP discovery failed\" with\n    data.code invalid_profile_url.\n  evidence: Observed on resources/list and prompts/list probes, 2026-08-15.\n- id: oauth2-oidc-shopify\n  type: openIdConnect\n  applies_to: [Parsley Health store customer accounts]\n  issuer: https://shopify.com/authentication/24996151350\n\
  \  authorization_endpoint: https://shopify.com/authentication/24996151350/oauth/authorize\n  token_endpoint: https://shopify.com/authentication/24996151350/oauth/token\n  end_session_endpoint: https://shopify.com/authentication/24996151350/logout\n  jwks_uri: https://shopify.com/authentication/24996151350/.well-known/jwks.json\n  discovery:\n  - https://store.parsleyhealth.com/.well-known/openid-configuration\n  - https://store.parsleyhealth.com/.well-known/oauth-authorization-server\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:jwt-bearer']\n  response_types: [code]\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, email, 'customer-account-api:full', 'customer-account-mcp-api:full']\n  scopes_artifact: scopes/parsley-health-scopes.yml\n  note: >-\n    The discovery documents are served from Parsley Health's hostname but the issuer is\n    Shopify's per-shop authorization server\
  \ for shop 24996151350. Parsley Health does not\n    operate this authorization server; it is inherited from the commerce platform.\n- id: member-app-login\n  type: opaque\n  applies_to: [https://my.parsleyhealth.com, https://app.parsleyhealth.com]\n  description: >-\n    Authenticated member application for clinical care. Single-page app behind a\n    catch-all that returns HTTP 200 text/html for every path, including\n    /.well-known/* and /openapi.json. No auth metadata, no token endpoint, no\n    machine-readable contract is discoverable.\n  evidence: Probed 2026-08-15 and 2026-08-02; all responses are the app shell.\napi_keys:\n  published: false\n  note: No developer program, no API key issuance, no key-prefix convention published.\nmtls:\n  published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parsley-health/refs/heads/main/authentication/parsley-health-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Health
- Healthcare
- Telehealth
- Telemedicine
- Functional Medicine
- Primary Care
- Wellness
- Nutrition
- Diagnostics
- Lab Testing
- Membership
- Digital Health
- Consumer Health
- Ecommerce
- Agentic Commerce
- MCP
- Supplements
---
