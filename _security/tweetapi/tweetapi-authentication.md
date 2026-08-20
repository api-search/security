---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tweetapi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TweetAPI secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TweetAPI
provider_slug: tweetapi
scheme_count: 2
schemes:
- applies_to: TweetAPI tw-v2 REST API (all 76 documented endpoints)
  in: header
  name: XApiKey
  note: Single key, no scopes, no key-level permission model. The key identifies the billing account and its rate ceiling; it does not restrict which endpoint categories may be called.
  obtained_from: https://tweetapi.com/dashboard (account required, free trial without a card)
  parameter_name: X-API-Key
  source: https://tweetapi.com/docs/getting-started/overview
  type: apiKey
- applies_to: TweetAPI Hosted MCP Server (https://mcp.tweetapi.com/mcp)
  bearer_methods:
  - header
  flows:
  - authorizationUrl: https://tweetapi.com/dashboard/mcp/authorize
    flow: authorizationCode
    registrationUrl: https://tweetapi.com/api/oauth/register
    revocationUrl: https://tweetapi.com/api/oauth/revoke
    scopes:
    - tweetapi:read
    - offline_access
    tokenUrl: https://tweetapi.com/api/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://tweetapi.com
  name: TweetAPIOAuth
  note: RFC 8414 authorization-server metadata plus RFC 9728 protected-resource metadata, with dynamic client registration (RFC 7591) and RFC 8707 resource indicators. This is a materially stronger auth posture than the REST surface, and it exists so the API key stays behind the OAuth boundary instead of being pasted into an agent client.
  pkce:
    methods:
    - S256
    required_hint: only S256 advertised
    supported: true
  resource_indicators: true
  source: https://tweetapi.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: tweetapi-authentication
source_filename: tweetapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: searched\nsource: https://tweetapi.com/docs/getting-started/overview\ncorroborating_sources:\n  - https://tweetapi.com/.well-known/oauth-authorization-server\n  - https://mcp.tweetapi.com/.well-known/oauth-protected-resource/mcp\n  - https://tweetapi.com/llms.txt\ndocs: https://tweetapi.com/docs/getting-started/overview\nnote: >-\n  Derived by hand rather than by derive-authentication.py: TweetAPI publishes no OpenAPI, so there\n  are no securitySchemes to aggregate. Everything below was read from the provider's own docs and\n  live OAuth discovery documents.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  surfaces: 2\nschemes:\n  - name: XApiKey\n    type: apiKey\n    in: header\n    parameter_name: X-API-Key\n    applies_to: TweetAPI tw-v2 REST API (all 76 documented endpoints)\n    source: https://tweetapi.com/docs/getting-started/overview\n    obtained_from: https://tweetapi.com/dashboard\
  \ (account required, free trial without a card)\n    note: >-\n      Single key, no scopes, no key-level permission model. The key identifies the billing account\n      and its rate ceiling; it does not restrict which endpoint categories may be called.\n  - name: TweetAPIOAuth\n    type: oauth2\n    applies_to: TweetAPI Hosted MCP Server (https://mcp.tweetapi.com/mcp)\n    source: https://tweetapi.com/.well-known/oauth-authorization-server\n    issuer: https://tweetapi.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://tweetapi.com/dashboard/mcp/authorize\n        tokenUrl: https://tweetapi.com/api/oauth/token\n        revocationUrl: https://tweetapi.com/api/oauth/revoke\n        registrationUrl: https://tweetapi.com/api/oauth/register\n        scopes: [tweetapi:read, offline_access]\n    pkce: {supported: true, methods: [S256], required_hint: only S256 advertised}\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none]\n\
  \    resource_indicators: true\n    bearer_methods: [header]\n    note: >-\n      RFC 8414 authorization-server metadata plus RFC 9728 protected-resource metadata, with dynamic\n      client registration (RFC 7591) and RFC 8707 resource indicators. This is a materially stronger\n      auth posture than the REST surface, and it exists so the API key stays behind the OAuth\n      boundary instead of being pasted into an agent client.\naccount_credentials:\n  note: >-\n    A distinct third credential class, and the one a governance reader should look at hardest. The\n    account-authorized endpoints (posting, engagement, lists, profile, X Chat, legacy DM — 43 of 76\n    documented endpoints) require the caller to pass end-user Twitter/X session material as ordinary\n    request parameters: authToken (the auth_token cookie), ct0 (the CSRF token), an optional\n    upstream proxy string of the form host:port@user:pass, and for POST /tw-v2/auth/login a username,\n    password and twoFactorSecret.\
  \ These are not TweetAPI credentials and there is no delegated\n    authorization (no OAuth to X, no token exchange) in front of them.\n  fields: [authToken, ct0, proxy, password, twoFactorSecret]\n  transport_concern: >-\n    Several of these appear as query-string parameters in the provider's own published curl examples\n    (for example GET /tw-v2/interaction/inbox-timeline-trusted?authToken=...), which puts long-lived\n    session cookies into URLs and therefore into logs and referrers. Moving them to the request body\n    or a header would be a meaningful hardening step.\n  provider_guidance: >-\n    TweetAPI's own agent skill forbids agents from requesting, storing or forwarding any of these\n    values, and the hosted MCP server deliberately does not expose the endpoints that need them.\ngaps:\n  - No scopes or per-key permissions on the REST surface\n  - No key rotation or expiry policy published\n  - No mTLS, no signed requests, no OpenID Connect\n  - No documented 403 behaviour\
  \ distinguishing key-level from account-level authorization failure\nsee_also:\n  - scopes/tweetapi-scopes.yml\n  - conventions/tweetapi-conventions.yml\n  - well-known/tweetapi-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tweetapi/refs/heads/main/authentication/tweetapi-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Twitter
- X
- Social-Media
- Social Data
- Search
- Analytics
- Research
- Developer Tools
- MCP
- agent-native
- llms-txt
- REST API
---
