---
api_key_in: []
api_specs:
- filename: taboola-accounts-api-openapi.yml
  format: yaml
  label: Taboola Accounts API
  slug: taboola-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-accounts-api-openapi.yml
- filename: taboola-audience-targeting-api-openapi.yml
  format: yaml
  label: Taboola Audience Targeting API
  slug: taboola-audience-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-audience-targeting-api-openapi.yml
- filename: taboola-bulk-items-api-openapi.yml
  format: yaml
  label: Taboola Bulk Items API
  slug: taboola-bulk-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-items-api-openapi.yml
- filename: taboola-bulk-operations-api-openapi.yml
  format: yaml
  label: Taboola Bulk Operations API
  slug: taboola-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-bulk-operations-api-openapi.yml
- filename: taboola-campaign-items-api-openapi.yml
  format: yaml
  label: Taboola Campaign Items API
  slug: taboola-campaign-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaign-items-api-openapi.yml
- filename: taboola-campaigns-api-openapi.yml
  format: yaml
  label: Taboola Campaigns API
  slug: taboola-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-campaigns-api-openapi.yml
- filename: taboola-combined-audiences-api-openapi.yml
  format: yaml
  label: Taboola Combined Audiences API
  slug: taboola-combined-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-combined-audiences-api-openapi.yml
- filename: taboola-conversion-rules-api-openapi.yml
  format: yaml
  label: Taboola Conversion Rules API
  slug: taboola-conversion-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-conversion-rules-api-openapi.yml
- filename: taboola-custom-audiences-api-openapi.yml
  format: yaml
  label: Taboola Custom Audiences API
  slug: taboola-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-custom-audiences-api-openapi.yml
- filename: taboola-dictionary-api-openapi.yml
  format: yaml
  label: Taboola Dictionary API
  slug: taboola-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-dictionary-api-openapi.yml
- filename: taboola-first-party-audiences-api-openapi.yml
  format: yaml
  label: Taboola First Party Audiences API
  slug: taboola-first-party-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-first-party-audiences-api-openapi.yml
- filename: taboola-lookalike-audiences-api-openapi.yml
  format: yaml
  label: Taboola Lookalike Audiences API
  slug: taboola-lookalike-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-lookalike-audiences-api-openapi.yml
- filename: taboola-marketplace-audiences-api-openapi.yml
  format: yaml
  label: Taboola Marketplace Audiences API
  slug: taboola-marketplace-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-marketplace-audiences-api-openapi.yml
- filename: taboola-reach-estimator-api-openapi.yml
  format: yaml
  label: Taboola Reach Estimator API
  slug: taboola-reach-estimator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reach-estimator-api-openapi.yml
- filename: taboola-reports-api-openapi.yml
  format: yaml
  label: Taboola Reports API
  slug: taboola-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-reports-api-openapi.yml
- filename: taboola-video-items-api-openapi.yml
  format: yaml
  label: Taboola Video Items API
  slug: taboola-video-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/openapi/taboola-video-items-api-openapi.yml
auth_types:
- oauth2
- http
description: 'Two OAuth surfaces with very different maturity. The Backstage advertising API uses a

  plain OAuth 2.0 client credentials grant with manually issued credentials and no scopes,

  and the token is presented as a bearer on every call. The Realize MCP server, added

  later, runs OAuth 2.1 with PKCE, discovery metadata and dynamic client registration.

  A previous round derived only the bearer scheme from the OpenAPI; this round upgrades it

  from the provider''s own documentation and a live probe.'
kind: authentication
layout: security
method: searched
name: Taboola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Taboola secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Taboola
provider_slug: taboola
scheme_count: 3
schemes:
- bearerFormat: opaque
  format: 'Authorization: Bearer {access_token}'
  header: Authorization
  in: header
  name: bearerAuth
  note: The captured specs declare bearerFormat JWT. The docs do not claim JWT and the sample token in the client-credentials-flow page is an opaque base64-ish string with a "::" delimiter, not a three-segment JWT. Recorded as opaque here; treat the token as opaque and do not attempt to parse claims from it.
  scheme: bearer
  sources:
  - openapi/taboola-accounts-api-openapi.yml
  - openapi/taboola-campaigns-api-openapi.yml
  - openapi/taboola-campaign-items-api-openapi.yml
  - openapi/taboola-conversion-rules-api-openapi.yml
  - openapi/taboola-dictionary-api-openapi.yml
  - openapi/taboola-reports-api-openapi.yml
  surface: Backstage API
  type: http
- flow: clientCredentials
  name: backstageClientCredentials
  note: The docs page embeds a one-operation OpenAPI 3.1.0 fragment for this endpoint that declares scopes as an empty object for both clientCredentials and the deprecated password flow — the provider's own statement that there is no scope vocabulary. Permissions ride on the account the client_id identifies. Trailing slash on the token URL returns a 403 CSRF HTML page.
  parameters:
  - client_id
  - client_secret
  - grant_type=client_credentials
  refresh_token: false
  scopes: {}
  source: https://developers.taboola.com/backstage-api/reference/client-credentials-flow
  surface: Backstage API
  token_endpoint: https://backstage.taboola.com/backstage/oauth/token
  token_request_content_type: application/x-www-form-urlencoded
  token_ttl_human: 12 hours
  token_ttl_seconds: 43200
  type: oauth2
- authorization_endpoint: https://authentication.taboola.com/authentication/oauth2.1/authorize
  discovery:
    authorization_server_metadata: https://mcp.realize.com/.well-known/oauth-authorization-server
    protected_resource_metadata: https://mcp.realize.com/.well-known/oauth-protected-resource
  flows:
  - authorization_code
  - refresh_token
  - client_credentials
  http_status: 200
  introspection_endpoint: https://authentication.taboola.com/authentication/oauth2.1/introspect
  issuer: https://mcp.realize.com
  name: realizeMcpOAuth
  note: Full RFC 9728 challenge loop verified live — an unauthenticated tools/list returns 401 with WWW-Authenticate pointing at the protected-resource metadata document.
  pkce: S256
  probed: '2026-08-13'
  registration_endpoint: https://mcp.realize.com/register
  resource: https://mcp.realize.com/mcp
  resource_indicators_supported: true
  scopes:
    all: The single advertised scope. No read-only alternative.
  surface: Realize MCP
  token_endpoint: https://authentication.taboola.com/authentication/oauth2.1/token
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  version: OAuth 2.1
slug: taboola-authentication
source_filename: taboola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.taboola.com/backstage-api/reference/authentication-basics,\n  https://developers.taboola.com/backstage-api/reference/client-credentials-flow,\n  https://developers.taboola.com/backstage-api/reference/getting-an-access-token,\n  https://developers.taboola.com/backstage-api/reference/request-basics,\n  https://mcp.realize.com/.well-known/oauth-authorization-server (probed 2026-08-13),\n  openapi/*.yml\ndocs:\n  - https://developers.taboola.com/backstage-api/reference/authentication-basics\n  - https://developers.taboola.com/backstage-api/reference/client-credentials-flow\nprovider: Taboola\nproviderId: taboola\ndescription: |-\n  Two OAuth surfaces with very different maturity. The Backstage advertising API uses a\n  plain OAuth 2.0 client credentials grant with manually issued credentials and no scopes,\n  and the token is presented as a bearer on every call. The Realize MCP server, added\n  later, runs\
  \ OAuth 2.1 with PKCE, discovery metadata and dynamic client registration.\n  A previous round derived only the bearer scheme from the OpenAPI; this round upgrades it\n  from the provider's own documentation and a live probe.\n\nsummary:\n  types:\n    - oauth2\n    - http\n  surfaces: 2\n  scopes_published: 1\n  credential_issuance: manual (Backstage) / dynamic client registration (MCP)\n\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: opaque\n    surface: Backstage API\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer {access_token}'\n    sources:\n      - openapi/taboola-accounts-api-openapi.yml\n      - openapi/taboola-campaigns-api-openapi.yml\n      - openapi/taboola-campaign-items-api-openapi.yml\n      - openapi/taboola-conversion-rules-api-openapi.yml\n      - openapi/taboola-dictionary-api-openapi.yml\n      - openapi/taboola-reports-api-openapi.yml\n    note: >-\n      The captured specs declare bearerFormat\
  \ JWT. The docs do not claim JWT and the sample\n      token in the client-credentials-flow page is an opaque base64-ish string with a\n      \"::\" delimiter, not a three-segment JWT. Recorded as opaque here; treat the token as\n      opaque and do not attempt to parse claims from it.\n\n  - name: backstageClientCredentials\n    type: oauth2\n    surface: Backstage API\n    flow: clientCredentials\n    token_endpoint: https://backstage.taboola.com/backstage/oauth/token\n    token_request_content_type: application/x-www-form-urlencoded\n    parameters: [client_id, client_secret, grant_type=client_credentials]\n    scopes: {}\n    token_ttl_seconds: 43200\n    token_ttl_human: 12 hours\n    refresh_token: false\n    source: https://developers.taboola.com/backstage-api/reference/client-credentials-flow\n    note: >-\n      The docs page embeds a one-operation OpenAPI 3.1.0 fragment for this endpoint that\n      declares scopes as an empty object for both clientCredentials and the deprecated\n\
  \      password flow — the provider's own statement that there is no scope vocabulary.\n      Permissions ride on the account the client_id identifies. Trailing slash on the\n      token URL returns a 403 CSRF HTML page.\n\n  - name: realizeMcpOAuth\n    type: oauth2\n    surface: Realize MCP\n    resource: https://mcp.realize.com/mcp\n    issuer: https://mcp.realize.com\n    version: OAuth 2.1\n    flows: [authorization_code, refresh_token, client_credentials]\n    pkce: S256\n    authorization_endpoint: https://authentication.taboola.com/authentication/oauth2.1/authorize\n    token_endpoint: https://authentication.taboola.com/authentication/oauth2.1/token\n    introspection_endpoint: https://authentication.taboola.com/authentication/oauth2.1/introspect\n    registration_endpoint: https://mcp.realize.com/register\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    scopes:\n      all: The single advertised scope. No read-only alternative.\n    resource_indicators_supported:\
  \ true\n    discovery:\n      authorization_server_metadata: https://mcp.realize.com/.well-known/oauth-authorization-server\n      protected_resource_metadata: https://mcp.realize.com/.well-known/oauth-protected-resource\n    probed: '2026-08-13'\n    http_status: 200\n    note: >-\n      Full RFC 9728 challenge loop verified live — an unauthenticated tools/list returns\n      401 with WWW-Authenticate pointing at the protected-resource metadata document.\n\ncredentials:\n  backstage:\n    issuance: >-\n      \"Ask your Taboola Account Manager to provide you with a client_id and client_secret.\"\n      There is no self-service developer console for Backstage credentials.\n    self_service: false\n  mcp:\n    issuance: Dynamic client registration at https://mcp.realize.com/register, then Taboola SSO.\n    self_service: true\n\nfailure_modes:\n  detail: ../errors/taboola-problem-types.yml\n  modes:\n    - status: 401\n      cause: Missing Authorization header, or an invalid/expired access\
  \ token.\n    - status: 400\n      cause: Bad client credentials at the token endpoint (XML invalid_client fault).\n    - status: 403\n      cause: Trailing slash on the token endpoint URL (HTML CSRF error from Jetty).\n\ndeprecated:\n  - flow: password (resource owner credentials)\n    deprecated_on: '2024-06-30'\n    replacement: client_credentials\n    source: https://developers.taboola.com/backstage-api/changelog/password-credentials-deprecation-notice\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taboola/refs/heads/main/authentication/taboola-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Advertising
- Native Advertising
- Discovery
- Performance Marketing
- AdTech
- Realize
- Backstage
- Recommendation
- Publishers
- Programmatic
---
