---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: Tracxn API
  slug: tracxn-api
  spec_type: Postman
  url: https://www.postman.com/tracxnapi/tracxn-api/overview
auth_types:
- apiKey
- oauth2
description: 'Tracxn runs TWO independent authentication models, one per surface, and they share no credential. The REST API takes a long-lived, account-scoped API token in an `accessToken` request header — no OAuth, no scopes, no expiry for active accounts. The MCP server takes OAuth 2.1 with PKCE and dynamic client registration, browser-based, with a single `read` scope. Tokens are additionally ENVIRONMENT-specific on REST: the Playground token and the Production token are separate credentials issued from separate pages and Tracxn explicitly warns against reusing one for the other.'
kind: authentication
layout: security
method: searched
name: Tracxn Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: Tracxn secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: Tracxn
provider_slug: tracxn
scheme_count: 2
schemes:
- environments:
  - base_url: https://platform.tracxn.com/api/3.0
    environment: production
    legacy_base_url: https://platform.tracxn.com/api/2.2
    token_page: https://platform.tracxn.com/a/api/productionenvironment/apitoken
  - base_url: https://platform.tracxn.com/api/2.2/playground
    environment: playground
    note: Separate token; commercial use prohibited. See sandbox/tracxn-sandbox.yml.
    token_page: https://platform.tracxn.com/a/api/playground/about
  expiry:
    active_accounts: Tokens are generally configured NOT to expire for active accounts.
    notice: An alert notification is sent 30 days before an API access token expires.
    rotation: Self-serve — generate a new token from the API Token page at any time.
    trial_accounts: Automatically revoked when the trial period ends.
  in: header
  issuance: Tracxn platform > Data Solutions > API & Developer Tools > (Production Environment | Playground) > API Token > "Generate a new token"
  issuance_url: https://platform.tracxn.com/a/api/apitoken
  name: accessToken
  parameter: accessToken
  parameter_note: Published in the Postman collection as `accessToken` (camelCase) and observed working as `accesstoken` (lowercase) — HTTP header names are case-insensitive, so both are correct. Documentation is inconsistent between the two; either is safe to send.
  scopes: none
  surface: rest
  token_isolation: 'Tokens are environment-specific. Tracxn''s guide states: "Do not reuse between Playground and Production."'
  type: apiKey
  value_format: Opaque account-scoped token issued by Tracxn
- api_token_alternative:
    note: Tracxn documents a forthcoming MCP API-token method for in-house AI platforms and Microsoft Copilot Studio. Not available at this pass — OAuth is the only working method.
    status: coming-soon
  authorization_endpoint: https://platform.tracxn.com/auth/2.0/mcp/authorize
  client_type: public
  detail: scopes/tracxn-scopes.yml
  dynamic_client_registration: true
  flow: authorization_code
  issuer: https://platform.tracxn.com/mcp
  metadata:
    authorization_server: well-known/tracxn-oauth-authorization-server-mcp.json
    protected_resource: well-known/tracxn-oauth-protected-resource-mcp.json
  name: mcp-oauth
  pkce: S256
  pkce_required: true
  registration_endpoint: https://platform.tracxn.com/auth/2.0/mcp/register
  scopes:
  - read
  surface: mcp
  token_endpoint: https://platform.tracxn.com/auth/2.0/mcp/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
  user_experience: Browser-based login on first connect. Tracxn never sees the AI client's credentials and the AI client never sees the user's Tracxn password. The user revokes by disconnecting the integration in their AI client.
slug: tracxn-authentication
source_filename: tracxn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  Tracxn API Guide published in the official public Postman workspace\n  (https://www.postman.com/tracxnapi/tracxn-api), saved at\n  postman/tracxn-api-production.postman.json — request headers and the \"Generating API\n  Tokens\" section ;\n  https://help.tracxn.com/en/articles/8512359-getting-started-with-tracxn-apis ;\n  https://help.tracxn.com/en/articles/14686877-what-is-tracxn-mcp ;\n  live probes 2026-08-14 of https://platform.tracxn.com/api/2.2/companies (403 without token)\n  and https://platform.tracxn.com/mcp (401 + RFC 9728 challenge) ;\n  https://platform.tracxn.com/.well-known/oauth-authorization-server/mcp (HTTP 200)\ndocs: https://platform.tracxn.com/a/api/gettingstarted/apibasics\ndescription: >-\n  Tracxn runs TWO independent authentication models, one per surface, and they share no\n  credential. The REST API takes a long-lived, account-scoped API token in an `accessToken`\n  request header — no OAuth,\
  \ no scopes, no expiry for active accounts. The MCP server takes\n  OAuth 2.1 with PKCE and dynamic client registration, browser-based, with a single `read`\n  scope. Tokens are additionally ENVIRONMENT-specific on REST: the Playground token and the\n  Production token are separate credentials issued from separate pages and Tracxn explicitly\n  warns against reusing one for the other.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorization_code\n  scopes_defined: 1\nschemes:\n  - name: accessToken\n    surface: rest\n    type: apiKey\n    in: header\n    parameter: accessToken\n    parameter_note: >-\n      Published in the Postman collection as `accessToken` (camelCase) and observed working as\n      `accesstoken` (lowercase) — HTTP header names are case-insensitive, so both are correct.\n      Documentation is inconsistent between the two; either is safe to send.\n    value_format: Opaque account-scoped token issued by Tracxn\n\
  \    issuance: >-\n      Tracxn platform > Data Solutions > API & Developer Tools > (Production Environment |\n      Playground) > API Token > \"Generate a new token\"\n    issuance_url: https://platform.tracxn.com/a/api/apitoken\n    scopes: none\n    environments:\n      - environment: production\n        base_url: https://platform.tracxn.com/api/3.0\n        legacy_base_url: https://platform.tracxn.com/api/2.2\n        token_page: https://platform.tracxn.com/a/api/productionenvironment/apitoken\n      - environment: playground\n        base_url: https://platform.tracxn.com/api/2.2/playground\n        token_page: https://platform.tracxn.com/a/api/playground/about\n        note: Separate token; commercial use prohibited. See sandbox/tracxn-sandbox.yml.\n    token_isolation: >-\n      Tokens are environment-specific. Tracxn's guide states: \"Do not reuse between Playground\n      and Production.\"\n    expiry:\n      active_accounts: >-\n        Tokens are generally configured NOT to expire\
  \ for active accounts.\n      trial_accounts: Automatically revoked when the trial period ends.\n      notice: An alert notification is sent 30 days before an API access token expires.\n      rotation: Self-serve — generate a new token from the API Token page at any time.\n  - name: mcp-oauth\n    surface: mcp\n    type: oauth2\n    flow: authorization_code\n    pkce: S256\n    pkce_required: true\n    dynamic_client_registration: true\n    client_type: public\n    token_endpoint_auth_methods_supported: [none]\n    issuer: https://platform.tracxn.com/mcp\n    authorization_endpoint: https://platform.tracxn.com/auth/2.0/mcp/authorize\n    token_endpoint: https://platform.tracxn.com/auth/2.0/mcp/token\n    registration_endpoint: https://platform.tracxn.com/auth/2.0/mcp/register\n    scopes: [read]\n    detail: scopes/tracxn-scopes.yml\n    metadata:\n      protected_resource: well-known/tracxn-oauth-protected-resource-mcp.json\n      authorization_server: well-known/tracxn-oauth-authorization-server-mcp.json\n\
  \    user_experience: >-\n      Browser-based login on first connect. Tracxn never sees the AI client's credentials and\n      the AI client never sees the user's Tracxn password. The user revokes by disconnecting\n      the integration in their AI client.\n    api_token_alternative:\n      status: coming-soon\n      note: >-\n        Tracxn documents a forthcoming MCP API-token method for in-house AI platforms and\n        Microsoft Copilot Studio. Not available at this pass — OAuth is the only working method.\nentitlement_note: >-\n  Authentication is not authorization here. A valid credential on either surface still resolves\n  against the customer's subscription entitlements and credit balance: Tracxn's own\n  troubleshooting guidance covers tools that authenticate fine but return errors because \"your\n  subscription covers the data you're querying (e.g. financials may require a higher tier)\",\n  and a fully-authenticated REST call fails with 403 / code 900 once credits are exhausted.\n\
  unauthenticated_response:\n  rest:\n    status: 403\n    body:\n      errorCode: 403000000\n      message: Invalid web session access. No user.\n    observed: live probe 2026-08-14 (unchanged from 2026-07-21)\n    note: >-\n      The same envelope is returned for ANY unmatched path under /api/ — it is a catch-all, so\n      a 403 here does not prove an endpoint exists.\n  mcp:\n    status: 401\n    www_authenticate: >-\n      Bearer realm=\"mcp\",\n      resource_metadata=\"https://platform.tracxn.com/.well-known/oauth-protected-resource/mcp\"\n    body:\n      error: Unauthorized\n      message: Authorization required\n    observed: live probe 2026-08-14\n    note: Spec-compliant RFC 9728 challenge — this is what makes the server discoverable to a generic MCP client.\ndocumented_status_codes:\n  401: Authentication Issue — Token missing or invalid\n  403: Unauthorized — Token expired or access denied\n  detail: errors/tracxn-problem-types.yml\ntransport_security:\n  https_only: true\n\
  \  detail: security/tracxn-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracxn/refs/heads/main/authentication/tracxn-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Cloud Saas
- Market Intelligence
- Private Markets
- Venture Capital
- Startups
- Company Data
- Investors
- Funding
---
