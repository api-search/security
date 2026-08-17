---
api_key_in:
- query
api_specs:
- filename: antavo-events-openapi.yml
  format: yaml
  label: Antavo Events API
  slug: antavo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-events-openapi.yml
- filename: antavo-async-events-openapi.yml
  format: yaml
  label: Antavo Async Events API
  slug: antavo-async-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-async-events-openapi.yml
- filename: antavo-customer-openapi.yml
  format: yaml
  label: Antavo Customer API
  slug: antavo-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-customer-openapi.yml
- filename: antavo-display-openapi.yml
  format: yaml
  label: Antavo Display API
  slug: antavo-display-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-display-openapi.yml
- filename: antavo-entities-openapi.yml
  format: yaml
  label: Antavo Entities API
  slug: antavo-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-entities-openapi.yml
- filename: antavo-rewards-openapi.yml
  format: yaml
  label: Antavo Rewards API
  slug: antavo-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-rewards-openapi.yml
- filename: antavo-coupons-openapi.yml
  format: yaml
  label: Antavo Coupons and Coupon Pools API
  slug: antavo-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-coupons-openapi.yml
- filename: antavo-offers-openapi.yml
  format: yaml
  label: Antavo Offers API
  slug: antavo-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-offers-openapi.yml
- filename: antavo-points-preview-openapi.yml
  format: yaml
  label: Antavo Points Preview API
  slug: antavo-points-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-points-preview-openapi.yml
- filename: antavo-leaderboard-openapi.yml
  format: yaml
  label: Antavo Leaderboard API
  slug: antavo-leaderboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-leaderboard-openapi.yml
- filename: antavo-bulk-operations-openapi.yml
  format: yaml
  label: Antavo Bulk Operations API
  slug: antavo-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-bulk-operations-openapi.yml
- filename: antavo-clubs-openapi.yml
  format: yaml
  label: Antavo Clubs API
  slug: antavo-clubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-clubs-openapi.yml
- filename: antavo-promotion-engine-openapi.yml
  format: yaml
  label: Antavo Promotion Engine API
  slug: antavo-promotion-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-promotion-engine-openapi.yml
- filename: antavo-authentication-openapi.yml
  format: yaml
  label: Antavo Authentication API
  slug: antavo-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-authentication-openapi.yml
- filename: antavo-faq-openapi.yml
  format: yaml
  label: Antavo FAQ API
  slug: antavo-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-faq-openapi.yml
- filename: antavo-loyalty-read-openapi.yml
  format: yaml
  label: Antavo Loyalty Read API
  slug: antavo-loyalty-read-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-loyalty-read-openapi.yml
- filename: antavo-social-share-campaigns-openapi.yml
  format: yaml
  label: Antavo Social Share Campaigns API
  slug: antavo-social-share-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/openapi/antavo-social-share-campaigns-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: Antavo runs three distinct authentication models side by side, split by API rather than negotiated per request. The spec-derived scheme list below was produced mechanically from the harvested OpenAPI, then upgraded from Antavo's own API security and API signing documentation - the specs alone materially understate the model, because the Escher request signature that actually authenticates most calls is invisible to OpenAPI (it is a computed `Authorization` header, not a declared securityScheme).
kind: authentication
layout: security
method: searched
name: Antavo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Antavo secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Antavo
provider_slug: antavo
scheme_count: 5
schemes:
- applies_to:
  - Events, Async (submission side), Display, Customer, Entities, Rewards
  - Coupons, Coupon Pools, Offers, FAQ, Leaderboard, Clubs, Bulk Operations
  - Points Preview, Social Share Campaigns
  description: Workspace API key, passed as a query parameter. Generated in Management UI > API settings. The paired API SECRET is displayed only once at generation and is never retrievable afterwards; it is used to compute the Escher signature, not sent on the wire.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/antavo-bulk-operations-openapi.yml
  - openapi/antavo-clubs-openapi.yml
  - openapi/antavo-coupon-pools-openapi.yml
  - openapi/antavo-coupons-openapi.yml
  - openapi/antavo-customer-openapi.yml
  - openapi/antavo-display-openapi.yml
  - openapi/antavo-entities-openapi.yml
  - openapi/antavo-events-openapi.yml
  - openapi/antavo-faq-openapi.yml
  - openapi/antavo-leaderboard-openapi.yml
  - openapi/antavo-offers-openapi.yml
  - openapi/antavo-rewards-openapi.yml
  - openapi/antavo-social-share-campaigns-openapi.yml
  spec_names_observed:
  - api_key
  - ApiKeyAuth
  type: apiKey
  warning: The key travels in the QUERY STRING on every one of these APIs. Query parameters are routinely written to proxy, CDN and web-server access logs, so the key must be treated as observable in transit infrastructure. It is the signature, not the key, that provides authentication integrity.
- constraint: '"API signatures should not be generated on front-end implementations as this could potentially expose API keys and secrets." Signing must happen server-side, which is the central design constraint on any Antavo client, MCP server or agent integration.'
  declared_in_openapi: false
  derived_from: AWS Signature Version 4
  description: '"Antavo enhances HTTPS security by requiring every request to be signed with an API signature ... The Antavo Loyalty Cloud uses Escher, a stateless HTTP request signing specification based on an enhanced version of the AWS Signature Version 4 protocol." Antavo recomputes the signature server-side and rejects the request when the two do not match.'
  encoding: RFC 3986; spaces as %20 never +; commas as %2C; '+' and %2B rewritten to %20 outside the PHP SDK
  enforcement:
    all_environments: required from 2026-12-31
    per_endpoint_toggle: Management UI > API settings > Signature enforcement, available when the API signature check module is enabled. Toggleable per API - Challenges (legacy), Clubs, Coupons, Customer, Display, Entities, Events, FAQ, Offers, Rewards, Points preview. With enforcement on, a plain-key request is rejected with an authentication error.
    production: required today
    source: https://developers.antavo.com/changelog/discontinuing-unsigned-api-requests
  guarantees:
  - the request originates from an authorized client
  - the transmitted data was not modified in transit
  - the request is accepted only once within a defined time window
  header: Authorization
  libraries:
  - first_party: true
    language: php
    name: antavo/escher-php
    url: https://github.com/antavo/escher-php
  - first_party: true
    language: javascript
    name: '@antavo/api-signature-node'
    url: https://www.npmjs.com/package/@antavo/api-signature-node
  - first_party: false
    language: java
    name: escher-java
    url: https://github.com/emartech/escher-java
  - first_party: false
    language: csharp
    name: escher-csharp
    url: https://github.com/emartech/escher-csharp
  - first_party: false
    language: go
    name: EscherAuth/escher
    url: https://github.com/EscherAuth/escher
  - first_party: false
    language: other
    name: Escher implementations index
    url: https://escherauth.io/implementations.html
  name: escher-signature
  procedure:
  - Build the Canonical Request (HTTPRequestMethod, CanonicalURI, CanonicalQueryString, CanonicalHeaders, blank line, SignedHeaders, HashedRequestPayload) joined by LF.
  - Build the String to Sign from the hashed Canonical Request plus metadata.
  - Sign it with a Signing Key derived from the Antavo API secret.
  - Place the resulting signature in the Authorization header.
  required_headers:
  - Host
  - Date
  specification: https://escherauth.io/
  type: http-signature
- applies_to: POST /v1/auth/token
  description: HTTP Basic with the Authentication Manager client_id as username and client_secret as password. Used ONLY to authenticate the OAuth token request itself (client_secret_basic).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/antavo-authentication-openapi.yml
  type: http
- applies_to: Async Events API; also declared in the Promotion Engine spec
  bearerFormat: JWT
  description: 'Bearer presentation of the access token issued by POST /v1/auth/token. ''Authorization: Bearer <access_token>''.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/antavo-async-events-openapi.yml
  - openapi/antavo-promotion-engine-openapi.yml
  token_lifetime_seconds:
    maximum: 3600
    minimum: 300
  type: http
- declared_in_openapi: false
  description: '"Access tokens are issued via an OAuth 2.0 token endpoint using the Client Credentials grant type." Clients are created in Management UI > API settings > Authentication Manager with a name, purpose, expiration date, scope and token audience.'
  flow: clientCredentials
  name: oauth2-client-credentials
  note: Antavo does not model this as an OpenAPI oauth2 securityScheme, so a spec-only reader sees only basicAuth + bearerAuth and cannot discover the flow, the token URL or the scope. This is why derive-oauth-scopes.py returned nothing for this provider.
  parameters:
  - grant_type=client_credentials
  - scope
  request_content_type: application/x-www-form-urlencoded
  scopes:
  - loyalty.async_events
  see: scopes/antavo-scopes.yml
  token_endpoint_auth_method: client_secret_basic
  token_url: /v1/auth/token
  type: oauth2
slug: antavo-authentication
source_filename: antavo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/ (18 harvested OpenAPI documents)\ndocs: https://developers.antavo.com/docs/api-security\ndocs_signing: https://developers.antavo.com/docs/api-signing\ndocs_credentials: https://docs.antavo.com/docs/api-settings\ndocs_postman: https://developers.antavo.com/docs/signing-api-requests-in-postman\ndescription: >-\n  Antavo runs three distinct authentication models side by side, split by API\n  rather than negotiated per request. The spec-derived scheme list below was\n  produced mechanically from the harvested OpenAPI, then upgraded from Antavo's\n  own API security and API signing documentation - the specs alone materially\n  understate the model, because the Escher request signature that actually\n  authenticates most calls is invisible to OpenAPI (it is a computed\n  `Authorization` header, not a declared securityScheme).\n\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [query]\n  http_schemes: [basic, bearer]\n\
  \  oauth2_flows: [clientCredentials]\n  signing: escher\n  credential_scope: one workspace, one environment\n\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: >-\n    Workspace API key, passed as a query parameter. Generated in Management UI >\n    API settings. The paired API SECRET is displayed only once at generation and\n    is never retrievable afterwards; it is used to compute the Escher signature,\n    not sent on the wire.\n  applies_to:\n  - Events, Async (submission side), Display, Customer, Entities, Rewards\n  - Coupons, Coupon Pools, Offers, FAQ, Leaderboard, Clubs, Bulk Operations\n  - Points Preview, Social Share Campaigns\n  sources:\n  - openapi/antavo-bulk-operations-openapi.yml\n  - openapi/antavo-clubs-openapi.yml\n  - openapi/antavo-coupon-pools-openapi.yml\n  - openapi/antavo-coupons-openapi.yml\n  - openapi/antavo-customer-openapi.yml\n  - openapi/antavo-display-openapi.yml\n  - openapi/antavo-entities-openapi.yml\n  -\
  \ openapi/antavo-events-openapi.yml\n  - openapi/antavo-faq-openapi.yml\n  - openapi/antavo-leaderboard-openapi.yml\n  - openapi/antavo-offers-openapi.yml\n  - openapi/antavo-rewards-openapi.yml\n  - openapi/antavo-social-share-campaigns-openapi.yml\n  spec_names_observed: [api_key, ApiKeyAuth]\n  warning: >-\n    The key travels in the QUERY STRING on every one of these APIs. Query\n    parameters are routinely written to proxy, CDN and web-server access logs, so\n    the key must be treated as observable in transit infrastructure. It is the\n    signature, not the key, that provides authentication integrity.\n- name: escher-signature\n  type: http-signature\n  header: Authorization\n  specification: https://escherauth.io/\n  derived_from: AWS Signature Version 4\n  declared_in_openapi: false\n  description: >-\n    \"Antavo enhances HTTPS security by requiring every request to be signed with\n    an API signature ... The Antavo Loyalty Cloud uses Escher, a stateless HTTP\n    request\
  \ signing specification based on an enhanced version of the AWS\n    Signature Version 4 protocol.\" Antavo recomputes the signature server-side\n    and rejects the request when the two do not match.\n  procedure:\n  - Build the Canonical Request (HTTPRequestMethod, CanonicalURI, CanonicalQueryString, CanonicalHeaders, blank line, SignedHeaders, HashedRequestPayload) joined by LF.\n  - Build the String to Sign from the hashed Canonical Request plus metadata.\n  - Sign it with a Signing Key derived from the Antavo API secret.\n  - Place the resulting signature in the Authorization header.\n  required_headers: [Host, Date]\n  encoding: RFC 3986; spaces as %20 never +; commas as %2C; '+' and %2B rewritten to %20 outside the PHP SDK\n  guarantees:\n  - the request originates from an authorized client\n  - the transmitted data was not modified in transit\n  - the request is accepted only once within a defined time window\n  enforcement:\n    production: required today\n    all_environments:\
  \ required from 2026-12-31\n    source: https://developers.antavo.com/changelog/discontinuing-unsigned-api-requests\n    per_endpoint_toggle: >-\n      Management UI > API settings > Signature enforcement, available when the\n      API signature check module is enabled. Toggleable per API - Challenges\n      (legacy), Clubs, Coupons, Customer, Display, Entities, Events, FAQ, Offers,\n      Rewards, Points preview. With enforcement on, a plain-key request is\n      rejected with an authentication error.\n  libraries:\n  - {language: php, name: antavo/escher-php, url: https://github.com/antavo/escher-php, first_party: true}\n  - {language: javascript, name: '@antavo/api-signature-node', url: https://www.npmjs.com/package/@antavo/api-signature-node, first_party: true}\n  - {language: java, name: escher-java, url: https://github.com/emartech/escher-java, first_party: false}\n  - {language: csharp, name: escher-csharp, url: https://github.com/emartech/escher-csharp, first_party: false}\n  -\
  \ {language: go, name: EscherAuth/escher, url: https://github.com/EscherAuth/escher, first_party: false}\n  - {language: other, name: Escher implementations index, url: https://escherauth.io/implementations.html, first_party: false}\n  constraint: >-\n    \"API signatures should not be generated on front-end implementations as this\n    could potentially expose API keys and secrets.\" Signing must happen\n    server-side, which is the central design constraint on any Antavo client,\n    MCP server or agent integration.\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic with the Authentication Manager client_id as username and\n    client_secret as password. Used ONLY to authenticate the OAuth token request\n    itself (client_secret_basic).\n  applies_to: POST /v1/auth/token\n  sources: [openapi/antavo-authentication-openapi.yml]\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Bearer presentation of the\
  \ access token issued by POST /v1/auth/token.\n    'Authorization: Bearer <access_token>'.\n  applies_to: Async Events API; also declared in the Promotion Engine spec\n  token_lifetime_seconds: {minimum: 300, maximum: 3600}\n  sources:\n  - openapi/antavo-async-events-openapi.yml\n  - openapi/antavo-promotion-engine-openapi.yml\n- name: oauth2-client-credentials\n  type: oauth2\n  declared_in_openapi: false\n  flow: clientCredentials\n  token_url: /v1/auth/token\n  token_endpoint_auth_method: client_secret_basic\n  request_content_type: application/x-www-form-urlencoded\n  parameters: [grant_type=client_credentials, scope]\n  scopes: [loyalty.async_events]\n  description: >-\n    \"Access tokens are issued via an OAuth 2.0 token endpoint using the Client\n    Credentials grant type.\" Clients are created in Management UI > API settings\n    > Authentication Manager with a name, purpose, expiration date, scope and\n    token audience.\n  note: >-\n    Antavo does not model this as an OpenAPI\
  \ oauth2 securityScheme, so a\n    spec-only reader sees only basicAuth + bearerAuth and cannot discover the\n    flow, the token URL or the scope. This is why derive-oauth-scopes.py returned\n    nothing for this provider.\n  see: scopes/antavo-scopes.yml\n\ncredential_management:\n  location: Management UI > API settings\n  api_key: visible on the settings page at any time\n  api_secret: displayed once at generation, never retrievable\n  rotation_warning: >-\n    \"Generating new API credentials will deactivate all existing connections\n    until the new credentials are entered.\" There is no overlap window and no\n    multi-key rotation - key rotation is a hard cutover with downtime.\n  oauth_client_secret: displayed once at creation, never retrievable\n  oauth_client_statuses: [active, revoked, expired]\n  oauth_revocation: irreversible\n  audit_log: >-\n    The Authentication Manager audit log records client creation, revocation, and\n    every access token issued or rejected by the\
  \ token endpoint.\n\nnetwork_authorization:\n  ip_filter:\n    supported: true\n    notation: CIDR\n    granularity: per API endpoint\n    module_gated: true\n    on_violation: forbidden exception (HTTP 403)\n    source: https://docs.antavo.com/docs/api-settings\n    note: >-\n      Requires the IP filter module to be enabled by the Antavo Service Desk. The\n      allow-list is per endpoint, not per key, so an agent or server calling from\n      dynamic egress addresses must be allow-listed before any call succeeds.\n\ntransport:\n  https_required: true\n  http_behaviour: redirected to HTTPS, but relying on the redirect is discouraged\n  tls_minimum: TLS 1.2\n  observed_tls: TLSv1.3 on antavo.com, developers.antavo.com and api.antavo.com (2026-08-13)\n  see: security/antavo-domain-security.yml\n\nauthorization_model:\n  scopes: >-\n    Only the OAuth surface has scopes, and only one exists\n    (loyalty.async_events). Key-authenticated APIs have no scope dimension at\n    all - a workspace\
  \ key is authorised for every enabled endpoint in that\n    workspace, constrained only by the per-endpoint IP filter and signature\n    enforcement toggles.\n  least_privilege: >-\n    There is no read-only key, no per-resource key and no delegation model. This\n    is the most significant authorisation gap on the platform: any integration\n    holding a workspace key can write loyalty events, claim rewards and read\n    every member profile.\n  end_user_auth:\n    note: >-\n      Separate from API-client auth. Loyalty members authenticate through the\n      Custom login module - POST /customers/-/login, POST /customers/{id}/opt-in,\n      POST /customers/-/password/request, POST /customers/-/password/reset,\n      GET /customers/-/verify/ - which returns the customer object and its\n      Antavo ID for subsequent Display API calls. A successful login also writes\n      a daily_login event, once per calendar day.\n    module_gated: true\n\ncross_links:\n  scopes: scopes/antavo-scopes.yml\n\
  \  conventions: conventions/antavo-conventions.yml\n  errors: errors/antavo-problem-types.yml\n  sandbox: sandbox/antavo-sandbox.yml\n  domain_security: security/antavo-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/authentication/antavo-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Loyalty
- Customer Loyalty
- Rewards
- Enterprise
- Headless
- Retail
- Marketing
- Engagement
- Promotions
- Gamification
- Events
- eCommerce
- Coupons
- Points
- Membership
---
