---
api_key_in:
- header
api_specs:
- filename: sumble-contact-lists-api-openapi.yml
  format: yaml
  label: Sumble contact-lists API
  slug: sumble-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-contact-lists-api-openapi.yml
- filename: sumble-jobs-api-openapi.yml
  format: yaml
  label: Sumble jobs API
  slug: sumble-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-jobs-api-openapi.yml
- filename: sumble-organization-lists-api-openapi.yml
  format: yaml
  label: Sumble organization-lists API
  slug: sumble-organization-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organization-lists-api-openapi.yml
- filename: sumble-organizations-api-openapi.yml
  format: yaml
  label: Sumble organizations API
  slug: sumble-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-organizations-api-openapi.yml
- filename: sumble-people-api-openapi.yml
  format: yaml
  label: Sumble people API
  slug: sumble-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-people-api-openapi.yml
- filename: sumble-projects-api-openapi.yml
  format: yaml
  label: Sumble projects API
  slug: sumble-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-projects-api-openapi.yml
- filename: sumble-signals-api-openapi.yml
  format: yaml
  label: Sumble signals API
  slug: sumble-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-signals-api-openapi.yml
- filename: sumble-support-api-openapi.yml
  format: yaml
  label: Sumble support API
  slug: sumble-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-support-api-openapi.yml
- filename: sumble-teams-api-openapi.yml
  format: yaml
  label: Sumble teams API
  slug: sumble-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-teams-api-openapi.yml
- filename: sumble-technologies-api-openapi.yml
  format: yaml
  label: Sumble technologies API
  slug: sumble-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/openapi/sumble-technologies-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Sumble Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Sumble secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Sumble
provider_slug: sumble
scheme_count: 2
schemes:
- applied_to: 'all 26 operations (declared per-operation as security[{api_token: []}])'
  failure_status: 401
  header: 'Authorization: Bearer YOUR_API_KEY'
  in: header
  key_management:
    availability: API keys can be generated on all plans
    display: shown in full only once at creation
    issuance: Account > API Keys > Create Key; name the key, copy the token immediately
    rotation: keys can be revoked at any time; lost keys are deleted and regenerated
    url: https://sumble.com/account/api-keys
  name: api_token
  scheme: bearer
  sources:
  - openapi/_original/sumble-openapi-original.json
  surface: REST API
  type: http
- bearer_methods_supported:
  - header
  challenge: 'WWW-Authenticate: Bearer error="invalid_token", error_description="Authentication required", resource_metadata="https://mcp.sumble.com/.well-known/oauth-protected-resource"'
  discovery:
  - file: ../well-known/sumble-mcp-oauth-authorization-server.json
    spec: RFC 8414 (Authorization Server Metadata)
    status: 200
    url: https://mcp.sumble.com/.well-known/oauth-authorization-server
  - file: ../well-known/sumble-mcp-oauth-protected-resource.json
    spec: RFC 9728 (Protected Resource Metadata)
    status: 200
    url: https://mcp.sumble.com/.well-known/oauth-protected-resource
  dynamic_client_registration: true
  failure_status: 401
  flows:
  - authorizationUrl: https://mcp.sumble.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    registrationUrl: https://mcp.sumble.com/register
    scopes: {}
    tokenUrl: https://mcp.sumble.com/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: mcp_oauth
  note: scopes_supported is absent from the authorization-server metadata and no scope/permission reference is published, so there is no scope surface to capture; scopes/ is intentionally not emitted.
  scopes_published: false
  surface: MCP server (https://mcp.sumble.com)
  type: oauth2
slug: sumble-authentication
source_filename: sumble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  openapi/_original/sumble-openapi-original.json (derived) upgraded from\n  https://docs.sumble.com/api/api,\n  https://docs.sumble.com/trust-and-security/trust-and-security, and live\n  probes of the MCP OAuth discovery documents.\ndocs: https://docs.sumble.com/api/api\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\n  api_key_in: [header]\n  note: >-\n    Two distinct auth surfaces. The REST API takes a long-lived account API\n    key as an HTTP bearer token. The hosted MCP server takes OAuth 2.0 with\n    PKCE and dynamic client registration — a different credential entirely,\n    and the reason an MCP client can be connected without ever handling the\n    API key.\nschemes:\n  - name: api_token\n    surface: REST API\n    type: http\n    scheme: bearer\n    in: header\n    header: 'Authorization: Bearer YOUR_API_KEY'\n    sources: [openapi/_original/sumble-openapi-original.json]\n\
  \    applied_to: 'all 26 operations (declared per-operation as security[{api_token: []}])'\n    key_management:\n      url: https://sumble.com/account/api-keys\n      issuance: 'Account > API Keys > Create Key; name the key, copy the token immediately'\n      display: shown in full only once at creation\n      rotation: keys can be revoked at any time; lost keys are deleted and regenerated\n      availability: API keys can be generated on all plans\n    failure_status: 401\n  - name: mcp_oauth\n    surface: MCP server (https://mcp.sumble.com)\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.sumble.com/authorize\n        tokenUrl: https://mcp.sumble.com/token\n        registrationUrl: https://mcp.sumble.com/register\n        code_challenge_methods: [S256]\n        grant_types: [authorization_code, refresh_token]\n        token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n        scopes: {}\n    dynamic_client_registration:\
  \ true\n    discovery:\n      - {spec: 'RFC 8414 (Authorization Server Metadata)', url: 'https://mcp.sumble.com/.well-known/oauth-authorization-server', status: 200, file: ../well-known/sumble-mcp-oauth-authorization-server.json}\n      - {spec: 'RFC 9728 (Protected Resource Metadata)', url: 'https://mcp.sumble.com/.well-known/oauth-protected-resource', status: 200, file: ../well-known/sumble-mcp-oauth-protected-resource.json}\n    bearer_methods_supported: [header]\n    failure_status: 401\n    challenge: 'WWW-Authenticate: Bearer error=\"invalid_token\", error_description=\"Authentication required\", resource_metadata=\"https://mcp.sumble.com/.well-known/oauth-protected-resource\"'\n    scopes_published: false\n    note: >-\n      scopes_supported is absent from the authorization-server metadata and no\n      scope/permission reference is published, so there is no scope surface to\n      capture; scopes/ is intentionally not emitted.\nuser_authentication:\n  surface: web app (not the\
  \ API)\n  methods:\n    - {method: magic-link, detail: users sign in with their email address via magic link}\n    - {method: sso, protocol: 'Okta OIDC', availability: enterprise plans, docs: 'https://docs.sumble.com/system-setup-and-configuration/users-access/okta-sso-oidc'}\n  session: JWT-based\n  source: https://docs.sumble.com/trust-and-security/trust-and-security\nevidence:\n  - {url: 'https://docs.sumble.com/api/api.md', status: 200}\n  - {url: 'https://mcp.sumble.com/.well-known/oauth-authorization-server', status: 200}\n  - {url: 'https://mcp.sumble.com/.well-known/oauth-protected-resource', status: 200}\n  - {url: 'https://api.sumble.com/v9/organizations', status: 401, note: live unauthenticated POST confirms bearer enforcement}\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumble/refs/heads/main/authentication/sumble-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Account Intelligence
- Sales Intelligence
- Data Enrichment
- Go-To-Market
- Technographics
- People Data
- Job Posts
- Signals
- MCP
---
