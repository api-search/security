---
api_key_in:
- header
api_specs:
- filename: clevertap-campaigns-api-openapi.yml
  format: yaml
  label: CleverTap Campaigns API
  slug: clevertap-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-campaigns-api-openapi.yml
- filename: clevertap-events-api-openapi.yml
  format: yaml
  label: CleverTap Events API
  slug: clevertap-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-events-api-openapi.yml
- filename: clevertap-profiles-api-openapi.yml
  format: yaml
  label: CleverTap Profiles API
  slug: clevertap-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-profiles-api-openapi.yml
- filename: clevertap-reports-api-openapi.yml
  format: yaml
  label: CleverTap Reports API
  slug: clevertap-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/openapi/clevertap-reports-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: CleverTap's authentication model, derived from the OpenAPI security schemes and upgraded from the provider's own authentication and SCIM pages plus the MCP server's OAuth metadata. Three distinct models coexist on three different surfaces, and they do not share credentials.
kind: authentication
layout: security
method: searched
name: Clevertap Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: CleverTap secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: CleverTap
provider_slug: clevertap
scheme_count: 4
schemes:
- description: CleverTap Account ID (Project ID), found under Settings > Project > Overview.
  in: header
  name: AccountId
  parameter: X-CleverTap-Account-Id
  sources:
  - openapi/clevertap-campaigns-api-openapi.yml
  - openapi/clevertap-events-api-openapi.yml
  - openapi/clevertap-profiles-api-openapi.yml
  - openapi/clevertap-reports-api-openapi.yml
  - https://developer.clevertap.com/docs/authentication
  surface: rest
  type: apiKey
- description: CleverTap Account Passcode, paired with the Account ID on every REST request.
  in: header
  name: Passcode
  parameter: X-CleverTap-Passcode
  sources:
  - openapi/clevertap-campaigns-api-openapi.yml
  - openapi/clevertap-events-api-openapi.yml
  - openapi/clevertap-profiles-api-openapi.yml
  - openapi/clevertap-reports-api-openapi.yml
  - https://developer.clevertap.com/docs/authentication
  surface: rest
  type: apiKey
- description: Separate bearer token for the SCIM user-provisioning endpoints (/nx/v2/scim/v2/Users). Generated in the dashboard under Organization > SCIM Management. Exactly one token exists per account; it is valid for one year, and regenerating it immediately invalidates the previous token. SCIM and IdP tokens are not interchangeable.
  name: SCIM Token
  scheme: bearer
  sources:
  - https://developer.clevertap.com/docs/scim-user-provisioning-using-api
  surface: scim
  type: http
- description: The remote MCP server at mcp.clevertap.com is OAuth-protected with dynamic client registration and PKCE. This is the only CleverTap surface using OAuth.
  detail: scopes/clevertap-scopes.yml
  flows:
  - authorizationUrl: https://mcp.clevertap.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://mcp.clevertap.com/oauth/register
    scopes: 4
    tokenUrl: https://mcp.clevertap.com/oauth/token
  - flow: refreshToken
    tokenUrl: https://mcp.clevertap.com/oauth/token
  name: MCP OAuth 2.1
  sources:
  - well-known/clevertap-oauth-authorization-server.json
  - well-known/clevertap-oauth-protected-resource.json
  surface: mcp
  type: oauth2
slug: clevertap-authentication
source_filename: clevertap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/clevertap-campaigns-api-openapi.yml, openapi/clevertap-events-api-openapi.yml,\n  openapi/clevertap-profiles-api-openapi.yml, openapi/clevertap-reports-api-openapi.yml\ndocs: https://developer.clevertap.com/docs/authentication\ndescription: >-\n  CleverTap's authentication model, derived from the OpenAPI security schemes and\n  upgraded from the provider's own authentication and SCIM pages plus the MCP\n  server's OAuth metadata. Three distinct models coexist on three different\n  surfaces, and they do not share credentials.\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n    - refreshToken\n  surfaces: 3\nschemes:\n  - name: AccountId\n    type: apiKey\n    in: header\n    parameter: X-CleverTap-Account-Id\n    description: CleverTap Account ID (Project ID), found under Settings > Project > Overview.\n    surface: rest\n    sources:\n\
  \      - openapi/clevertap-campaigns-api-openapi.yml\n      - openapi/clevertap-events-api-openapi.yml\n      - openapi/clevertap-profiles-api-openapi.yml\n      - openapi/clevertap-reports-api-openapi.yml\n      - https://developer.clevertap.com/docs/authentication\n  - name: Passcode\n    type: apiKey\n    in: header\n    parameter: X-CleverTap-Passcode\n    description: CleverTap Account Passcode, paired with the Account ID on every REST request.\n    surface: rest\n    sources:\n      - openapi/clevertap-campaigns-api-openapi.yml\n      - openapi/clevertap-events-api-openapi.yml\n      - openapi/clevertap-profiles-api-openapi.yml\n      - openapi/clevertap-reports-api-openapi.yml\n      - https://developer.clevertap.com/docs/authentication\n  - name: SCIM Token\n    type: http\n    scheme: bearer\n    description: >-\n      Separate bearer token for the SCIM user-provisioning endpoints\n      (/nx/v2/scim/v2/Users). Generated in the dashboard under Organization >\n      SCIM Management.\
  \ Exactly one token exists per account; it is valid for one\n      year, and regenerating it immediately invalidates the previous token. SCIM\n      and IdP tokens are not interchangeable.\n    surface: scim\n    sources:\n      - https://developer.clevertap.com/docs/scim-user-provisioning-using-api\n  - name: MCP OAuth 2.1\n    type: oauth2\n    description: >-\n      The remote MCP server at mcp.clevertap.com is OAuth-protected with dynamic\n      client registration and PKCE. This is the only CleverTap surface using\n      OAuth.\n    surface: mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.clevertap.com/oauth/authorize\n        tokenUrl: https://mcp.clevertap.com/oauth/token\n        registrationUrl: https://mcp.clevertap.com/oauth/register\n        scopes: 4\n        pkce: S256\n      - flow: refreshToken\n        tokenUrl: https://mcp.clevertap.com/oauth/token\n    sources:\n      - well-known/clevertap-oauth-authorization-server.json\n   \
  \   - well-known/clevertap-oauth-protected-resource.json\n    detail: scopes/clevertap-scopes.yml\nposture:\n  rotation_documented: false\n  expiry:\n    rest: none\n    scim: 1 year\n    mcp: access token + refresh token\n  scoping:\n    rest: none\n    mcp: identity scopes only (openid, profile, email, offline_access)\n  mtls: false\n  ip_allowlisting: true\n  ip_allowlist_note: >-\n    CleverTap publishes its outbound IP ranges for customers allowlisting\n    CleverTap traffic, and offers \"restricted IP access\" as a dashboard security\n    control.\n  ip_ranges_doc: https://developer.clevertap.com/docs/clevertap-ip-ranges\n  payload_encryption:\n    supported: true\n    scheme: HPKE\n    doc: https://developer.clevertap.com/docs/api-encryption\n  regional_binding:\n    note: >-\n      Credentials are bound to the account's data-center region. Presenting valid\n      credentials to the wrong regional host returns HTTP 401 Unauthorized rather\n      than a redirect.\n    doc: https://developer.clevertap.com/docs/common-api-components\n\
  \  gap: >-\n    The REST API — the surface that carries all customer data — uses two static,\n    non-expiring, unscoped header credentials. There is no token exchange, no\n    least-privilege scope, no documented rotation procedure and no expiry. An\n    agent given these headers holds full account authority indefinitely.\nx-evidence:\n  fetched: '2026-08-13'\n  urls:\n    - url: https://developer.clevertap.com/docs/authentication\n      status: 200\n    - url: https://developer.clevertap.com/docs/common-api-components\n      status: 200\n    - url: https://developer.clevertap.com/docs/scim-user-provisioning-using-api\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clevertap/refs/heads/main/authentication/clevertap-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Audiences
- Customer Engagement
- Customer Retention
- Marketing Automation
- Mobile Engagement
- Push Notifications
- User Behavior
---
