---
api_key_in: []
auth_types: []
description: 'Omaze publishes no API keys and no developer credentials. The only authentication surface it exposes is the Shopify Customer Accounts identity provider that sits behind its UK and German storefronts: a standards-compliant OpenID Connect 1.0 / OAuth 2.0 authorization server, discoverable anonymously, with PKCE required. This profile is derived entirely from the live discovery documents — no securityScheme was inferred from a spec, because there is no spec.'
kind: authentication
layout: security
method: probed
name: Omaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: Omaze declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Omaze
provider_slug: omaze
scheme_count: 2
schemes:
- claims:
  - iss
  - sub
  - aud
  - exp
  - iat
  - nonce
  - sid
  - email
  - email_verified
  endpoints:
    authorization: https://accounts.omaze.co.uk/authentication/oauth/authorize
    end_session: https://accounts.omaze.co.uk/authentication/logout
    jwks: https://accounts.omaze.co.uk/authentication/.well-known/jwks.json
    token: https://accounts.omaze.co.uk/authentication/oauth/token
  file: ../well-known/omaze-uk-openid-configuration.json
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: shopify-customer-accounts-uk
  id_token_signing_alg:
  - RS256
  issuer: https://shopify.com/authentication/27583905878
  market: United Kingdom
  openid_configuration: https://omaze.co.uk/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    required: true
  response_types:
  - code
  scopes: ../scopes/omaze-scopes.yml
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  type: openIdConnect
- endpoints:
    authorization: https://accounts.omaze.de/authentication/oauth/authorize
  file: ../well-known/omaze-de-openid-configuration.json
  id: shopify-customer-accounts-de
  issuer: https://shopify.com/authentication/69889196213
  market: Germany
  note: Same Shopify Customer Accounts profile as the UK store, distinct issuer and account host. Scope set is identical.
  openid_configuration: https://omaze.de/.well-known/openid-configuration
  type: openIdConnect
slug: omaze-authentication
source_filename: omaze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: >-\n  https://omaze.co.uk/.well-known/openid-configuration,\n  https://omaze.co.uk/.well-known/oauth-authorization-server,\n  https://omaze.co.uk/.well-known/oauth-protected-resource,\n  https://omaze.de/.well-known/openid-configuration — all fetched 2026-08-02.\ndescription: >-\n  Omaze publishes no API keys and no developer credentials. The only\n  authentication surface it exposes is the Shopify Customer Accounts identity\n  provider that sits behind its UK and German storefronts: a standards-compliant\n  OpenID Connect 1.0 / OAuth 2.0 authorization server, discoverable anonymously,\n  with PKCE required. This profile is derived entirely from the live discovery\n  documents — no securityScheme was inferred from a spec, because there is no\n  spec.\nschemes:\n  - id: shopify-customer-accounts-uk\n    type: openIdConnect\n    market: United Kingdom\n    issuer: https://shopify.com/authentication/27583905878\n    openid_configuration:\
  \ https://omaze.co.uk/.well-known/openid-configuration\n    file: ../well-known/omaze-uk-openid-configuration.json\n    endpoints:\n      authorization: https://accounts.omaze.co.uk/authentication/oauth/authorize\n      token: https://accounts.omaze.co.uk/authentication/oauth/token\n      end_session: https://accounts.omaze.co.uk/authentication/logout\n      jwks: https://accounts.omaze.co.uk/authentication/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    response_types:\n      - code\n    token_endpoint_auth_methods:\n      - client_secret_basic\n    pkce:\n      required: true\n      code_challenge_methods:\n        - S256\n    id_token_signing_alg:\n      - RS256\n    subject_types:\n      - public\n    claims:\n      - iss\n      - sub\n      - aud\n      - exp\n      - iat\n      - nonce\n      - sid\n      - email\n      - email_verified\n    scopes: ../scopes/omaze-scopes.yml\n\
  \  - id: shopify-customer-accounts-de\n    type: openIdConnect\n    market: Germany\n    issuer: https://shopify.com/authentication/69889196213\n    openid_configuration: https://omaze.de/.well-known/openid-configuration\n    file: ../well-known/omaze-de-openid-configuration.json\n    endpoints:\n      authorization: https://accounts.omaze.de/authentication/oauth/authorize\n    note: >-\n      Same Shopify Customer Accounts profile as the UK store, distinct issuer and\n      account host. Scope set is identical.\nprotected_resource:\n  spec: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n  url: https://omaze.co.uk/.well-known/oauth-protected-resource\n  file: ../well-known/omaze-uk-oauth-protected-resource.json\n  resource: https://omaze.co.uk\n  authorization_servers:\n    - https://accounts.omaze.co.uk\n    - https://shopify.com/authentication/27583905878\n  bearer_methods_supported:\n    - header\nanonymous_surfaces:\n  - surface: UCP Shopping MCP endpoint (https://omaze.co.uk/api/ucp/mcp)\n\
  \    auth: >-\n      No bearer token is required to reach the endpoint, but the server refuses\n      to negotiate without a resolvable UCP agent profile URI from the calling\n      agent (observed: JSON-RPC -32001 / invalid_profile_url, HTTP 422). Payment\n      completion additionally requires explicit buyer approval.\n  - surface: Storefront product/collection JSON (/products.json, /collections/{handle}/products.json)\n    auth: None. Read-only, anonymous, public.\nnot_published:\n  api_keys: No developer API keys, no key-issuance flow, no developer portal.\n  mtls: Not advertised.\n  http_basic: Not advertised.\n  service_accounts: None.\ndocs: https://omaze.co.uk/agents.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omaze/refs/heads/main/authentication/omaze-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Charity
- Fundraising
- Non-Profit
- Prize Draws
- Sweepstakes
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- United Kingdom
- Germany
---
