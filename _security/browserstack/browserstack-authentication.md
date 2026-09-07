---
anonymous_access: false
api_key_in: []
api_specs:
- filename: browserstack-accesskey-api-openapi.yml
  format: yaml
  label: BrowserStack AccessKey API
  slug: browserstack-accesskey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-accesskey-api-openapi.yml
- filename: browserstack-browsers-api-openapi.yml
  format: yaml
  label: BrowserStack Browsers API
  slug: browserstack-browsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-browsers-api-openapi.yml
- filename: browserstack-builds-api-openapi.yml
  format: yaml
  label: BrowserStack Builds API
  slug: browserstack-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-builds-api-openapi.yml
- filename: browserstack-plan-api-openapi.yml
  format: yaml
  label: BrowserStack Plan API
  slug: browserstack-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-plan-api-openapi.yml
- filename: browserstack-projects-api-openapi.yml
  format: yaml
  label: BrowserStack Projects API
  slug: browserstack-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-projects-api-openapi.yml
- filename: browserstack-sessions-api-openapi.yml
  format: yaml
  label: BrowserStack Sessions API
  slug: browserstack-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-sessions-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Browserstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrowserStack secures its APIs with http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BrowserStack
provider_slug: browserstack
scheme_count: 5
schemes:
- applies_to:
  - BrowserStack Automate API
  - BrowserStack App Automate API
  - BrowserStack Test Management API
  - BrowserStack Accessibility Testing API
  - BrowserStack User Management API
  description: HTTP Basic using the BrowserStack username and access key, read from https://www.browserstack.com/accounts/profile/details. Applies to Automate, App Automate, Test Management, Accessibility Testing and User Management.
  name: basicAuth
  observed_failure:
    body: 'HTTP Basic: Access denied.'
    content_type: text/html; charset=utf-8
    http_status: 401
    note: The failure response is HTML, not JSON. See errors/browserstack-problem-types.yml.
    url: https://api.browserstack.com/automate/plan.json
    www_authenticate: Basic realm="Application"
  rotation:
    note: Rotation is immediate and irreversible; no grace period is documented for the old key.
    operationId: recycleAccessKey
    path: PUT /automate/recycle_key.json
    supported: true
  scheme: basic
  sources:
  - openapi/_original/browserstack-openapi.yml
  - https://www.browserstack.com/docs/automate/api-reference/selenium/introduction
  - https://www.browserstack.com/docs/test-management/api-reference/authentication
  - https://www.browserstack.com/docs/accessibility/api/authentication
  type: http
- applies_to:
  - BrowserStack Percy API
  - BrowserStack App Percy API
  bearerFormat: Token
  description: Per-project Percy API tokens in three classes — write-only (create builds, create snapshots; SDK use), read-only (read builds, download snapshots; API use) and full-access (all project read and write). Tokens are found on a project's Settings page.
  header: 'Authorization: Token ${PERCY_TOKEN}'
  name: percyToken
  note: The only BrowserStack credential with any scoping. It is per-project and has three capability classes, which is meaningfully safer to hand an agent than the account-wide access key every other product API requires.
  observed_failure:
    body: '{"errors":[{"status":"unauthorized","detail":"Percy::Errors::AuthenticationRequired"}]}'
    http_status: 401
    url: https://percy.io/api/v1/projects
    www_authenticate: Token realm="Application"
  scheme: bearer
  source: https://www.browserstack.com/docs/percy/api-reference/authentication
  type: http
- authorization_endpoint: https://auth.browserstack.com/oauth2/v2/authorize
  code_challenge_methods:
  - S256
  - plain
  description: BrowserStack operates a full OAuth 2.0 authorization server at https://auth.browserstack.com, discoverable from www.browserstack.com, api.browserstack.com and api-enterprise.browserstack.com.
  documented_for_rest_api: false
  file: well-known/browserstack-www-oauth-authorization-server.json
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  introspection_endpoint: https://auth.browserstack.com/oauth2/v2/introspect
  issuer: https://auth.browserstack.com
  jwks_uri: https://auth.browserstack.com/oauth2/v2/discovery/keys
  name: browserstackOAuth
  note: Not documented on any product API reference page. The scope names suggest it serves integrations (jira_integration), service-to-service calls (service_auth, central_ai_s2s), the Automate test-case generator (automate_tcg), the AI agents (ai_agent, ai_agent_notify) and a Part 11 re-authentication flow, rather than general REST access.
  revocation_endpoint: https://auth.browserstack.com/oauth2/v2/revoke
  scopes:
  - read
  - write
  - update
  - jira_integration
  - service_auth
  - central_ai_s2s
  - part11_reauth
  - automate_tcg
  - ai_agent
  - ai_agent_notify
  source: https://www.browserstack.com/.well-known/oauth-authorization-server
  token_endpoint: https://auth.browserstack.com/oauth2/v2/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://auth.browserstack.com/oauth2/v3/userinfo
- claims_supported:
  - iss
  - sub
  - aud
  - exp
  - iat
  file: well-known/browserstack-www-openid-configuration.json
  id_token_signing_alg_values_supported:
  - RS256
  name: browserstackOIDC
  openIdConnectUrl: https://www.browserstack.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  type: openIdConnect
- authorization_endpoint: https://mcp.browserstack.com/auth/oauth2/authorize
  code_challenge_methods:
  - S256
  description: 'Separate OAuth 2.1 authorization server for the hosted Remote MCP server. Open dynamic client registration (token_endpoint_auth_methods_supported: none), so an MCP client registers itself without a pre-shared secret.'
  file: well-known/browserstack-mcp-oauth-authorization-server.json
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.browserstack.com/
  name: mcpOAuth
  note: This is the only BrowserStack surface where OAuth is the documented and enforced authentication path, and the only one where a caller gets a scoped, revocable credential instead of the account access key. The provider's own README frames it as a benefit — "Secure OAuth integration – no password sharing or manual credential handling."
  protected_resource: https://mcp.browserstack.com/mcp
  registration_endpoint: https://mcp.browserstack.com/auth/oauth2/register
  scopes:
  - read
  - write
  - admin
  source: https://mcp.browserstack.com/.well-known/oauth-authorization-server
  token_endpoint: https://mcp.browserstack.com/auth/oauth2/token
  type: oauth2
slug: browserstack-authentication
source_filename: browserstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  BrowserStack product API authentication pages (Automate, Test Management, Accessibility,\n  Percy, App Percy, App Automate, User Management), the OAuth/OIDC discovery documents served\n  from www.browserstack.com, api.browserstack.com, api-enterprise.browserstack.com and\n  auth.browserstack.com, and openapi/_original/browserstack-openapi.yml. Fetched 2026-09-04.\ndocs: https://www.browserstack.com/docs/automate/api-reference/selenium/introduction#authentication\nprovider: BrowserStack\nproviderId: browserstack\nsummary:\n  types:\n    - http\n    - oauth2\n    - openIdConnect\n  primary: HTTP Basic with a long-lived account access key\n  detail: >-\n    Five of BrowserStack's six product APIs authenticate with HTTP Basic — the account username\n    as the user and the account access key as the password. Percy is the exception: it uses an\n    Authorization header of the form \"Token <PERCY_TOKEN>\" with per-project tokens\
  \ in three\n    classes. A full OAuth 2.0 / OpenID Connect provider exists at auth.browserstack.com and\n    advertises itself from three BrowserStack hosts, but no product API reference documents it\n    as a way to call the API. The hosted MCP server is the one BrowserStack surface that\n    actually requires OAuth.\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic using the BrowserStack username and access key, read from\n      https://www.browserstack.com/accounts/profile/details. Applies to Automate, App Automate,\n      Test Management, Accessibility Testing and User Management.\n    applies_to:\n      - BrowserStack Automate API\n      - BrowserStack App Automate API\n      - BrowserStack Test Management API\n      - BrowserStack Accessibility Testing API\n      - BrowserStack User Management API\n    sources:\n      - openapi/_original/browserstack-openapi.yml\n      - https://www.browserstack.com/docs/automate/api-reference/selenium/introduction\n\
  \      - https://www.browserstack.com/docs/test-management/api-reference/authentication\n      - https://www.browserstack.com/docs/accessibility/api/authentication\n    rotation:\n      supported: true\n      operationId: recycleAccessKey\n      path: PUT /automate/recycle_key.json\n      note: Rotation is immediate and irreversible; no grace period is documented for the old\n        key.\n    observed_failure:\n      url: https://api.browserstack.com/automate/plan.json\n      http_status: 401\n      www_authenticate: Basic realm=\"Application\"\n      content_type: text/html; charset=utf-8\n      body: 'HTTP Basic: Access denied.'\n      note: The failure response is HTML, not JSON. See errors/browserstack-problem-types.yml.\n  - name: percyToken\n    type: http\n    scheme: bearer\n    bearerFormat: Token\n    header: 'Authorization: Token ${PERCY_TOKEN}'\n    description: >-\n      Per-project Percy API tokens in three classes — write-only (create builds, create\n      snapshots; SDK\
  \ use), read-only (read builds, download snapshots; API use) and full-access\n      (all project read and write). Tokens are found on a project's Settings page.\n    applies_to:\n      - BrowserStack Percy API\n      - BrowserStack App Percy API\n    source: https://www.browserstack.com/docs/percy/api-reference/authentication\n    note: >-\n      The only BrowserStack credential with any scoping. It is per-project and has three\n      capability classes, which is meaningfully safer to hand an agent than the account-wide\n      access key every other product API requires.\n    observed_failure:\n      url: https://percy.io/api/v1/projects\n      http_status: 401\n      www_authenticate: Token realm=\"Application\"\n      body: '{\"errors\":[{\"status\":\"unauthorized\",\"detail\":\"Percy::Errors::AuthenticationRequired\"}]}'\n  - name: browserstackOAuth\n    type: oauth2\n    description: >-\n      BrowserStack operates a full OAuth 2.0 authorization server at\n      https://auth.browserstack.com,\
  \ discoverable from www.browserstack.com,\n      api.browserstack.com and api-enterprise.browserstack.com.\n    issuer: https://auth.browserstack.com\n    authorization_endpoint: https://auth.browserstack.com/oauth2/v2/authorize\n    token_endpoint: https://auth.browserstack.com/oauth2/v2/token\n    revocation_endpoint: https://auth.browserstack.com/oauth2/v2/revoke\n    introspection_endpoint: https://auth.browserstack.com/oauth2/v2/introspect\n    userinfo_endpoint: https://auth.browserstack.com/oauth2/v3/userinfo\n    jwks_uri: https://auth.browserstack.com/oauth2/v2/discovery/keys\n    grant_types: [authorization_code, client_credentials, refresh_token]\n    code_challenge_methods: [S256, plain]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n    scopes:\n      - read\n      - write\n      - update\n      - jira_integration\n      - service_auth\n      - central_ai_s2s\n      - part11_reauth\n      - automate_tcg\n      - ai_agent\n      - ai_agent_notify\n\
  \    source: https://www.browserstack.com/.well-known/oauth-authorization-server\n    file: well-known/browserstack-www-oauth-authorization-server.json\n    documented_for_rest_api: false\n    note: >-\n      Not documented on any product API reference page. The scope names suggest it serves\n      integrations (jira_integration), service-to-service calls (service_auth, central_ai_s2s),\n      the Automate test-case generator (automate_tcg), the AI agents (ai_agent,\n      ai_agent_notify) and a Part 11 re-authentication flow, rather than general REST access.\n  - name: browserstackOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://www.browserstack.com/.well-known/openid-configuration\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    claims_supported: [iss, sub, aud, exp, iat]\n    file: well-known/browserstack-www-openid-configuration.json\n  - name: mcpOAuth\n    type: oauth2\n    description: >-\n      Separate OAuth 2.1 authorization\
  \ server for the hosted Remote MCP server. Open dynamic\n      client registration (token_endpoint_auth_methods_supported: none), so an MCP client\n      registers itself without a pre-shared secret.\n    issuer: https://mcp.browserstack.com/\n    authorization_endpoint: https://mcp.browserstack.com/auth/oauth2/authorize\n    token_endpoint: https://mcp.browserstack.com/auth/oauth2/token\n    registration_endpoint: https://mcp.browserstack.com/auth/oauth2/register\n    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    scopes: [read, write, admin]\n    protected_resource: https://mcp.browserstack.com/mcp\n    source: https://mcp.browserstack.com/.well-known/oauth-authorization-server\n    file: well-known/browserstack-mcp-oauth-authorization-server.json\n    note: >-\n      This is the only BrowserStack surface where OAuth is the documented and enforced\n      authentication path, and the only one where a caller gets a scoped, revocable credential\n\
  \      instead of the account access key. The provider's own README frames it as a benefit —\n      \"Secure OAuth integration – no password sharing or manual credential handling.\"\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/authentication/browserstack-authentication.yml
summary_line: http/oauth2/openIdConnect · 5 schemes
tags:
- Accessibility
- Appium
- Application
- Automation
- CI/CD
- Cross-Browser Testing
- Enterprise
- JavaScript
- Low-Code
- Mobile Testing
- QA
- Regression Testing
- Selenium
- Testing
- Unit Testing
- Visual Testing
---
