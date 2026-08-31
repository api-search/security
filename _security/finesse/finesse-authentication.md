---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Finesse Authentication
name_suffix: Authentication
oauth_flows: []
overview: FINESSE declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: FINESSE
provider_slug: finesse
scheme_count: 0
schemes: []
slug: finesse-authentication
source_filename: finesse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://finesse.us/.well-known/openid-configuration,\n  https://finesse.us/.well-known/oauth-authorization-server,\n  https://finesse.us/.well-known/oauth-protected-resource,\n  https://finesse.us/agents.md, live POST to https://finesse.us/api/ucp/mcp\nnote: >-\n  FINESSE publishes no developer API keys and no partner credential program. There are two distinct\n  auth postures on the surface: the agent commerce endpoint, which is anonymous-but-profiled, and\n  the customer account identity provider, which is a full OIDC/OAuth 2.0 authorization server\n  scoped to this merchant.\nsurfaces:\n  - name: FINESSE UCP Commerce MCP\n    url: https://finesse.us/api/ucp/mcp\n    scheme: none (agent-profile assertion)\n    credentials_required: false\n    detail: >-\n      tools/list is fully anonymous — HTTP 200 with complete inputSchemas on 2026-08-12 with no\n      Authorization header. Tool CALLS require a `meta.ucp-agent.profile`\
  \ URI identifying the calling\n      agent; a call without it fails with JSON-RPC -32001 / invalid_profile_url. This is an agent\n      identity assertion, not a secret: there is no key to issue, rotate or revoke, and there is no\n      published registration step. Authorization for the sensitive step (payment) is enforced out of\n      band by requiring contemporaneous human buyer approval rather than by a token scope.\n    evidence:\n      http_status: 200\n      observed: '2026-08-12'\n  - name: FINESSE Customer Accounts (Shopify-hosted OIDC)\n    url: https://account.finesse.us/\n    scheme: openIdConnect\n    credentials_required: true\n    detail: >-\n      A full OIDC provider for FINESSE shoppers, discoverable at both\n      /.well-known/openid-configuration and /.well-known/oauth-authorization-server (RFC 8414) on\n      finesse.us, and again on account.finesse.us. Endpoints are on account.finesse.us; the issuer\n      is a per-merchant Shopify identity (https://shopify.com/authentication/23733469261).\
  \ This is\n      end-user login, not developer access.\n    oidc:\n      issuer: https://shopify.com/authentication/23733469261\n      authorization_endpoint: https://account.finesse.us/authentication/oauth/authorize\n      token_endpoint: https://account.finesse.us/authentication/oauth/token\n      end_session_endpoint: https://account.finesse.us/authentication/logout\n      jwks_uri: https://account.finesse.us/authentication/.well-known/jwks.json\n      response_types_supported: [code]\n      grant_types_supported:\n        - authorization_code\n        - refresh_token\n        - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n      token_endpoint_auth_methods_supported: [client_secret_basic]\n      code_challenge_methods_supported: [S256]\n      id_token_signing_alg_values_supported: [RS256]\n      subject_types_supported: [public]\n      claims_supported: [iss, sub, aud, exp, iat, nonce, sid, email, email_verified]\n      scopes_supported:\n        - openid\n        - email\n      \
  \  - 'customer-account-api:full'\n        - 'customer-account-mcp-api:full'\n    protected_resource:\n      resource: https://finesse.us\n      authorization_servers:\n        - https://account.finesse.us\n        - https://shopify.com/authentication/23733469261\n      bearer_methods_supported: [header]\n      spec: RFC 9728\nsecurity_schemes_summary:\n  apiKey: false\n  http_bearer: true          # via the OIDC access token on the customer-account surface\n  oauth2: true\n  openIdConnect: true\n  mutualTLS: false\n  none: true                 # anonymous tools/list on the MCP endpoint\ngaps:\n  - No security.txt and no documented credential-rotation or revocation guidance for agents.\n  - >-\n    No published developer registration: an agent profile URI is self-asserted, so the MCP surface\n    has identification without authentication. That is by design in UCP 2026-04-08, but it means\n    rate limiting is per IP rather than per credential.\n  - >-\n    The customer-account MCP API implied\
  \ by the `customer-account-mcp-api:full` scope is not\n    documented on any FINESSE-controlled page; it is discoverable only from the OAuth metadata.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finesse/refs/heads/main/authentication/finesse-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Retail
- E-Commerce
- fashion
- apparel
- direct-to-consumer
- agentic-commerce
- UCP
- MCP
- agent-native
- shopify
- consumer
---
