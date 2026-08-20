---
api_key_in:
- query
- header
api_specs:
- filename: ezoic-access-api-openapi.yml
  format: yaml
  label: ezoic Access API
  slug: ezoic-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-access-api-openapi.yml
- filename: ezoic-products-api-openapi.yml
  format: yaml
  label: ezoic Products API
  slug: ezoic-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-products-api-openapi.yml
- filename: ezoic-purchases-api-openapi.yml
  format: yaml
  label: ezoic Purchases API
  slug: ezoic-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-purchases-api-openapi.yml
- filename: ezoic-big-data-analytics-api-openapi.yml
  format: yaml
  label: ezoic Big Data Analytics API
  slug: ezoic-big-data-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-big-data-analytics-api-openapi.yml
- filename: ezoic-cdn-api-openapi.yml
  format: yaml
  label: ezoic CDN API
  slug: ezoic-cdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/openapi/ezoic-cdn-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ezoic Authentication
name_suffix: Authentication
oauth_flows: []
overview: ezoic secures its APIs with apiKey and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ezoic
provider_slug: ezoic
scheme_count: 6
schemes:
- description: Your Ezoic API key, copied from Settings -> API Access. One key for every enabled gateway service; regenerate it from the same page.
  in: query
  name: developerKey
  parameter: developerKey
  regime: API gateway (REST)
  risk: A long-lived bearer credential in the query string is logged by proxies, CDNs, browser history and server access logs by default. Ezoic keeps reader identity out of the URL for exactly this reason, but places the account credential there.
  sources:
  - https://docs.ezoic.com/docs/api/
  - openapi/ezoic-big-data-analytics-api-openapi.yml
  - openapi/ezoic-cdn-api-openapi.yml
  - openapi/ezoic-access-api-openapi.yml
  type: apiKey
- description: The domain being queried. Not a credential, but authorization-bearing — the gateway rejects any domain not on the key's account.
  in: query
  name: domain
  parameter: domain
  regime: API gateway (REST)
  sources:
  - https://docs.ezoic.com/docs/subscriptions/rest-api/
  type: scoping-parameter
- applies_to:
  - Subscriptions
  description: Reader identity — the reader's email address. The common case, including sites that bring their own login. Supply exactly one reader identity header; neither or both is rejected.
  in: header
  name: X-Ezoic-Reader-Email
  parameter: X-Ezoic-Reader-Email
  regime: API gateway (REST)
  sources:
  - https://docs.ezoic.com/docs/subscriptions/rest-api/
  type: apiKey
- applies_to:
  - Subscriptions
  description: Reader identity — the reader's Ezoic Subscriptions session JWT, for Ezoic visitor-account sites where the server never sees the reader's email. Read it in the browser with getSessionToken() and relay it. Short-lived and scoped to the current domain; the API validates it against the requested domain, so a token from one site cannot be replayed against another. Read per request rather than storing it — getSessionToken() returns null for a signed-out visitor.
  in: header
  name: X-Ezoic-Reader-Token
  parameter: X-Ezoic-Reader-Token
  regime: API gateway (REST)
  sources:
  - https://docs.ezoic.com/docs/subscriptions/rest-api/
  type: apiKey
- applies_to:
  - Analytics MCP
  bearer_methods_supported:
  - header
  description: The assistant redirects the user to Ezoic login, the user authorizes, and the assistant receives a scoped access token. Read-only — no MCP tool can modify, create or delete anything on the account.
  dpop: supported (ES256)
  dynamic_client_registration: https://token.ezoic.com/register
  flows:
    authorization_code:
      authorization_url: https://token.ezoic.com/authorize
      pkce: required (S256 only)
      scopes: {}
      token_url: https://token.ezoic.com/token
    client_credentials:
      token_url: https://token.ezoic.com/token
    device_code:
      device_authorization_url: https://token.ezoic.com/device_authorization
      token_url: https://token.ezoic.com/token
  issuer: https://token.ezoic.com
  jwks_uri: https://token.ezoic.com/.well-known/jwks.json
  metadata: https://token.ezoic.com/.well-known/oauth-authorization-server
  name: Ezoic OAuth 2.0
  regime: Agent surface (OAuth)
  revocation: https://token.ezoic.com/token/revoke
  sources:
  - https://docs.ezoic.com/docs/analytics-mcp/
  - https://token.ezoic.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - private_key_jwt
  type: oauth2
- applies_to:
  - Setup Assistant MCP
  description: No account and no key. Verified by a successful unauthenticated initialize + tools/list on 2026-08-13.
  endpoint: https://setup-agent.ezoic.com/mcp
  name: anonymous
  regime: Agent surface
  sources:
  - https://github.com/ezoic/ezoic-setup-mcp
  type: none
slug: ezoic-authentication
source_filename: ezoic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.ezoic.com/docs/api/ , https://docs.ezoic.com/docs/subscriptions/rest-api/ ,\n  https://docs.ezoic.com/docs/analytics-mcp/ , and live probes of\n  https://token.ezoic.com/.well-known/oauth-authorization-server and\n  https://analytics-mcp.ezoic.com/.well-known/oauth-protected-resource\ndocs: https://docs.ezoic.com/docs/api/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [query, header]\n  note: >-\n    Ezoic runs two authentication regimes with nothing in common. The REST gateway uses one\n    long-lived API key in the QUERY STRING for all three services. The agent surface uses a\n    modern OAuth 2.0 authorization server with PKCE, DPoP, dynamic client registration and\n    RFC 9728 resource metadata. The newer surface is materially better secured than the\n    older one.\nregimes:\n- name: API gateway (REST)\n  applies_to: [Big Data Analytics, CDN, Subscriptions]\n  host: https://api-gateway.ezoic.com\n\
  \  enablement: >-\n    Each service is off until enabled under Settings -> API Access in the Ezoic dashboard.\n    The key is shared across every enabled service and is rotatable from that page.\n  authorization: >-\n    The gateway authenticates the key, confirms it is enabled for the requested service,\n    and confirms any `domain` passed belongs to the account, before the request reaches the\n    service. A key can only ever act on its own domains.\n  unauthenticated_response: 503 \"Developer key is empty.\"\n- name: Agent surface (OAuth)\n  applies_to: [Analytics MCP]\n  authorization_server: https://token.ezoic.com\n  enablement: The connecting Ezoic role must include the Analytics permission.\n  see_also: scopes/ezoic-scopes.yml\nschemes:\n- name: developerKey\n  type: apiKey\n  in: query\n  parameter: developerKey\n  regime: API gateway (REST)\n  description: >-\n    Your Ezoic API key, copied from Settings -> API Access. One key for every enabled\n    gateway service; regenerate\
  \ it from the same page.\n  sources:\n  - https://docs.ezoic.com/docs/api/\n  - openapi/ezoic-big-data-analytics-api-openapi.yml\n  - openapi/ezoic-cdn-api-openapi.yml\n  - openapi/ezoic-access-api-openapi.yml\n  risk: >-\n    A long-lived bearer credential in the query string is logged by proxies, CDNs, browser\n    history and server access logs by default. Ezoic keeps reader identity out of the URL\n    for exactly this reason, but places the account credential there.\n- name: domain\n  type: scoping-parameter\n  in: query\n  parameter: domain\n  regime: API gateway (REST)\n  description: >-\n    The domain being queried. Not a credential, but authorization-bearing — the gateway\n    rejects any domain not on the key's account.\n  sources: [https://docs.ezoic.com/docs/subscriptions/rest-api/]\n- name: X-Ezoic-Reader-Email\n  type: apiKey\n  in: header\n  parameter: X-Ezoic-Reader-Email\n  regime: API gateway (REST)\n  applies_to: [Subscriptions]\n  description: >-\n    Reader identity\
  \ — the reader's email address. The common case, including sites that\n    bring their own login. Supply exactly one reader identity header; neither or both is\n    rejected.\n  sources: [https://docs.ezoic.com/docs/subscriptions/rest-api/]\n- name: X-Ezoic-Reader-Token\n  type: apiKey\n  in: header\n  parameter: X-Ezoic-Reader-Token\n  regime: API gateway (REST)\n  applies_to: [Subscriptions]\n  description: >-\n    Reader identity — the reader's Ezoic Subscriptions session JWT, for Ezoic\n    visitor-account sites where the server never sees the reader's email. Read it in the\n    browser with getSessionToken() and relay it. Short-lived and scoped to the current\n    domain; the API validates it against the requested domain, so a token from one site\n    cannot be replayed against another. Read per request rather than storing it —\n    getSessionToken() returns null for a signed-out visitor.\n  sources: [https://docs.ezoic.com/docs/subscriptions/rest-api/]\n- name: Ezoic OAuth 2.0\n\
  \  type: oauth2\n  regime: Agent surface (OAuth)\n  applies_to: [Analytics MCP]\n  issuer: https://token.ezoic.com\n  metadata: https://token.ezoic.com/.well-known/oauth-authorization-server\n  flows:\n    authorization_code:\n      authorization_url: https://token.ezoic.com/authorize\n      token_url: https://token.ezoic.com/token\n      pkce: required (S256 only)\n      scopes: {}\n    client_credentials:\n      token_url: https://token.ezoic.com/token\n    device_code:\n      device_authorization_url: https://token.ezoic.com/device_authorization\n      token_url: https://token.ezoic.com/token\n  bearer_methods_supported: [header]\n  dpop: supported (ES256)\n  dynamic_client_registration: https://token.ezoic.com/register\n  revocation: https://token.ezoic.com/token/revoke\n  jwks_uri: https://token.ezoic.com/.well-known/jwks.json\n  token_endpoint_auth_methods: [none, private_key_jwt]\n  description: >-\n    The assistant redirects the user to Ezoic login, the user authorizes, and the\
  \ assistant\n    receives a scoped access token. Read-only — no MCP tool can modify, create or delete\n    anything on the account.\n  sources:\n  - https://docs.ezoic.com/docs/analytics-mcp/\n  - https://token.ezoic.com/.well-known/oauth-authorization-server\n- name: anonymous\n  type: none\n  regime: Agent surface\n  applies_to: [Setup Assistant MCP]\n  endpoint: https://setup-agent.ezoic.com/mcp\n  description: >-\n    No account and no key. Verified by a successful unauthenticated initialize +\n    tools/list on 2026-08-13.\n  sources: [https://github.com/ezoic/ezoic-setup-mcp]\nmfa_or_signing:\n  request_signing: false\n  mutual_tls: false\n  note: No request signing or mTLS is published for the REST gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ezoic/refs/heads/main/authentication/ezoic-authentication.yml
summary_line: apiKey/oauth2 · 6 schemes
tags:
- Company
- Advertising
- AdTech
- Publisher Monetization
- Analytics
- Reporting
- Subscription
- Paywalls
- Identity
- CDN
- Caching
- MCP
- Authentication
- Agents
---
