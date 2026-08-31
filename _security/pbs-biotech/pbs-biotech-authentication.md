---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Pbs Biotech Authentication
name_suffix: Authentication
oauth_flows: []
overview: PBS Biotech declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PBS Biotech
provider_slug: pbs-biotech
scheme_count: 2
schemes:
- applies_to: https://shoppbsbiotech.com/api/ucp/mcp
  id: ucp-mcp-anonymous
  note: 'MCP tools/list requires no credentials and returned 200. tools/call requires no bearer token either, but does require an agent identity handle — meta.ucp-agent.profile, a resolvable agent profile URI. Omitting it returns HTTP 422 with JSON-RPC error -32001 (invalid_profile_url). This is agent identification, not authentication: nothing is issued to the caller.'
  type: none
- applies_to: https://account.shoppbsbiotech.com
  authorization_endpoint: https://account.shoppbsbiotech.com/authentication/oauth/authorize
  bearer_methods:
  - header
  end_session_endpoint: https://account.shoppbsbiotech.com/authentication/logout
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-account-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/71340753133
  jwks_uri: https://account.shoppbsbiotech.com/authentication/.well-known/jwks.json
  note: Platform-provided by Shopify for this merchant; the discovery documents are served from PBS Biotech's own store and account hosts. Used for buyer sign-in and customer-account/MCP access, not for any PBS Biotech product API.
  pkce:
    required_methods:
    - S256
  protected_resource: https://account.shoppbsbiotech.com
  response_types:
  - code
  scopes: scopes/pbs-biotech-scopes.yml
  token_endpoint: https://account.shoppbsbiotech.com/authentication/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
slug: pbs-biotech-authentication
source_filename: pbs-biotech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://shoppbsbiotech.com/.well-known/openid-configuration (200),\n  https://shoppbsbiotech.com/.well-known/oauth-authorization-server (200),\n  https://account.shoppbsbiotech.com/.well-known/oauth-protected-resource (200),\n  and an anonymous POST to https://shoppbsbiotech.com/api/ucp/mcp (tools/list 200, tools/call 422).\n  Probed 2026-08-26.\ndocs: https://shoppbsbiotech.com/llms.txt\nsummary: >-\n  PBS Biotech publishes no developer API of its own and therefore no first-party authentication model.\n  The only authenticated surface reachable on a host it controls is the Shopify customer-account OAuth\n  2.0 / OpenID Connect server behind its online store, plus the anonymous UCP/MCP commerce endpoint.\nschemes:\n- id: ucp-mcp-anonymous\n  type: none\n  applies_to: https://shoppbsbiotech.com/api/ucp/mcp\n  note: >-\n    MCP tools/list requires no credentials and returned 200. tools/call requires no bearer token either,\n\
  \    but does require an agent identity handle — meta.ucp-agent.profile, a resolvable agent profile URI.\n    Omitting it returns HTTP 422 with JSON-RPC error -32001 (invalid_profile_url). This is agent\n    identification, not authentication: nothing is issued to the caller.\n- id: shopify-customer-account-oidc\n  type: openIdConnect\n  applies_to: https://account.shoppbsbiotech.com\n  issuer: https://shopify.com/authentication/71340753133\n  authorization_endpoint: https://account.shoppbsbiotech.com/authentication/oauth/authorize\n  token_endpoint: https://account.shoppbsbiotech.com/authentication/oauth/token\n  end_session_endpoint: https://account.shoppbsbiotech.com/authentication/logout\n  jwks_uri: https://account.shoppbsbiotech.com/authentication/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n  response_types:\n  - code\n  pkce:\n    required_methods:\n    - S256\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg:\n  - RS256\n  bearer_methods:\n  - header\n  protected_resource: https://account.shoppbsbiotech.com\n  scopes: scopes/pbs-biotech-scopes.yml\n  note: >-\n    Platform-provided by Shopify for this merchant; the discovery documents are served from PBS Biotech's\n    own store and account hosts. Used for buyer sign-in and customer-account/MCP access, not for any PBS\n    Biotech product API.\nnot_found:\n- what: first-party API keys, bearer tokens or OAuth for bioreactor control software\n  note: >-\n    No developer portal, key issuance page, or authentication documentation exists on pbsbiotech.com.\n    The customer support portal and the Vertical-Wheel Scaling Calculator sign-in are human web logins\n    with no documented programmatic surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pbs-biotech/refs/heads/main/authentication/pbs-biotech-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Life Sciences
- Biotechnology
- Bioprocessing
- Cell Therapy
- Laboratory Equipment
- Manufacturing
- E-Commerce
- Agent Commerce
- MCP
---
