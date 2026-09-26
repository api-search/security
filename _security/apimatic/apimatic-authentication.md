---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: apimatic-docs-portal-api-openapi.yml
  format: yaml
  label: APIMatic Portals API
  slug: apimatic-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-docs-portal-api-openapi.yml
- filename: apimatic-sdk-api-openapi.yml
  format: yaml
  label: APIMatic SDK Generation API
  slug: apimatic-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-sdk-api-openapi.yml
- filename: apimatic-transformation-api-openapi.yml
  format: yaml
  label: APIMatic Transformation API
  slug: apimatic-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-transformation-api-openapi.yml
- filename: apimatic-validation-api-openapi.yml
  format: yaml
  label: APIMatic Validation API
  slug: apimatic-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/openapi/apimatic-validation-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apimatic Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: APIMatic secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: APIMatic
provider_slug: apimatic
scheme_count: 2
schemes:
- applies_to: platform-api
  docs: https://docs.apimatic.io/account-management/obtaining-auth-keys/
  in: header
  lifecycle: Created and named under Settings -> Account Settings -> API Authentication in the APIMatic dashboard; revoked from the same screen. No documented expiry or rotation policy.
  name: apiKey
  parameter: Authorization
  scheme_note: '"The Auth Key is required to authenticate the APIMatic APIs. It is passed in as an Authorization header." Generated first-party SDKs model it as a Custom Header Signature, not as a bearer token.'
  sources:
  - openapi/apimatic-docs-portal-api-openapi.yml
  - openapi/apimatic-docs-portal-async-api-openapi.yml
  - openapi/apimatic-sdk-api-openapi.yml
  - openapi/apimatic-sdk-async-api-openapi.yml
  - openapi/apimatic-transformation-api-openapi.yml
  - openapi/apimatic-validation-api-openapi.yml
  - openapi/apimatic-validation-v2-api-openapi.yml
  - https://github.com/apimatic/apimatic-sdk-for-js/blob/main/doc/auth/custom-header-signature.md
  type: apiKey
- applies_to: mcp
  dynamic_client_registration: https://chatbotapi.apimatic.io/register
  enforced: false
  enforced_note: initialize and tools/list both answered HTTP 200 with no Authorization header on 2026-09-15
  flows:
  - authorizationUrl: https://chatbotapi.apimatic.io/authorize
    flow: authorizationCode
    scopes:
    - mcp:tools
    tokenUrl: https://chatbotapi.apimatic.io/token
  - flow: clientCredentials
    scopes:
    - mcp:tools
    tokenUrl: https://chatbotapi.apimatic.io/token
  issuer: https://chatbotapi.apimatic.io
  metadata: https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server
  name: chatbotapi-mcp-oauth
  pkce:
  - S256
  protected_resource: https://chatbotapi.apimatic.io/.well-known/oauth-protected-resource
  sources:
  - well-known/apimatic-oauth-authorization-server.json
  - well-known/apimatic-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: apimatic-authentication
source_filename: apimatic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-15'\nmethod: searched\ndocs: https://docs.apimatic.io/account-management/obtaining-auth-keys/\nsource: |-\n  https://docs.apimatic.io/account-management/obtaining-auth-keys/ ;\n  https://github.com/apimatic/apimatic-sdk-for-js/blob/main/doc/auth/custom-header-signature.md ;\n  https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server (probed 2026-09-15) ;\n  openapi/apimatic-*-openapi.yml securitySchemes\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  note: >-\n    Two unrelated auth surfaces. The PLATFORM API (api.apimatic.io) uses a single long-lived\n    Auth Key sent verbatim in the Authorization header — no scopes, no expiry, no refresh, no\n    OAuth. The hosted MCP server (chatbotapi.apimatic.io) advertises a full OAuth 2.0\n    authorization server with PKCE and dynamic client registration, and also answers\n    anonymously. OAuth 2.0 additionally\
  \ appears as an SDK GENERATION feature for customers'\n    APIs, which is a product capability and not APIMatic's own auth.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  applies_to: platform-api\n  scheme_note: >-\n    \"The Auth Key is required to authenticate the APIMatic APIs. It is passed in as an\n    Authorization header.\" Generated first-party SDKs model it as a Custom Header Signature,\n    not as a bearer token.\n  lifecycle: >-\n    Created and named under Settings -> Account Settings -> API Authentication in the APIMatic\n    dashboard; revoked from the same screen. No documented expiry or rotation policy.\n  docs: https://docs.apimatic.io/account-management/obtaining-auth-keys/\n  sources:\n  - openapi/apimatic-docs-portal-api-openapi.yml\n  - openapi/apimatic-docs-portal-async-api-openapi.yml\n  - openapi/apimatic-sdk-api-openapi.yml\n  - openapi/apimatic-sdk-async-api-openapi.yml\n  - openapi/apimatic-transformation-api-openapi.yml\n\
  \  - openapi/apimatic-validation-api-openapi.yml\n  - openapi/apimatic-validation-v2-api-openapi.yml\n  - https://github.com/apimatic/apimatic-sdk-for-js/blob/main/doc/auth/custom-header-signature.md\n- name: chatbotapi-mcp-oauth\n  type: oauth2\n  applies_to: mcp\n  issuer: https://chatbotapi.apimatic.io\n  metadata: https://chatbotapi.apimatic.io/.well-known/oauth-authorization-server\n  protected_resource: https://chatbotapi.apimatic.io/.well-known/oauth-protected-resource\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://chatbotapi.apimatic.io/authorize\n    tokenUrl: https://chatbotapi.apimatic.io/token\n    scopes: [mcp:tools]\n  - flow: clientCredentials\n    tokenUrl: https://chatbotapi.apimatic.io/token\n    scopes: [mcp:tools]\n  pkce: [S256]\n  dynamic_client_registration: https://chatbotapi.apimatic.io/register\n  token_endpoint_auth_methods_supported: [none]\n  enforced: false\n  enforced_note: initialize and tools/list both answered HTTP 200 with no Authorization\
  \ header on 2026-09-15\n  sources:\n  - well-known/apimatic-oauth-authorization-server.json\n  - well-known/apimatic-oauth-protected-resource.json\ncli_auth:\n  commands: [apimatic auth login, apimatic auth status, apimatic auth logout]\n  flow: browser-based login, credentials cached locally\n  docs: https://docs.apimatic.io/apimatic-cli/commands/\nsso:\n  available: true\n  tier: Enterprise\n  docs: https://docs.apimatic.io/platform/sso/\ncross_links:\n  scopes: scopes/apimatic-scopes.yml\n  conventions: conventions/apimatic-conventions.yml\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apimatic/refs/heads/main/authentication/apimatic-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- API Transformation
- Code Generation
- Developer Experience
- Developer Tools
- Documentation
- SDK Generation
- OpenAPI
---
