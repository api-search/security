---
api_key_in:
- header
api_specs:
- filename: lili-application-api-openapi.yml
  format: yaml
  label: Lili Application API
  slug: lili-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-application-api-openapi.yml
- filename: lili-customer-management-api-openapi.yml
  format: yaml
  label: Lili Customer Management API
  slug: lili-customer-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-customer-management-api-openapi.yml
- filename: lili-webhooks-api-openapi.yml
  format: yaml
  label: Lili Webhooks API
  slug: lili-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/openapi/lili-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Lili Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lili secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lili
provider_slug: lili
scheme_count: 2
schemes:
- applies_to:
  - openapi/lili-application-api-openapi.yml
  - openapi/lili-customer-management-api-openapi.yml
  - openapi/lili-webhooks-api-openapi.yml
  description: 'The authorization in the format:<br/>

    Authorization: Lili accessKey:secretKey'
  example_from_docs: 'curl -X GET https://prod.lili.co/lili/api/v1/webhooks -H "Authorization: Lili accessKey:secretKey"'
  in: header
  issuance:
    environments:
    - sandbox
    - production
    key_prefix_convention: none
    key_prefix_note: There is no test/live prefix. A sandbox key and a production key are indistinguishable by inspection, so environment binding has to be enforced by the integrator's own configuration.
    process: Contact dev-resources@lili.co. Lili issues an access/secret key pair per environment on account creation.
    self_serve: false
  name: accessKey
  operations: all
  parameter: Authorization
  rotation_policy: not published
  scheme_word: Lili
  scopes: none
  surface: REST
  type: apiKey
  value_format: Lili <accessKey>:<secretKey>
- applies_to:
  - https://mcp.lili.co/mcp
  authorization_endpoint: https://mcp.lili.co/oauth/authorize
  bearer_methods_supported:
  - header
  discovery:
  - well-known/lili-mcp-oauth-authorization-server.json
  - well-known/lili-mcp-oauth-protected-resource.json
  dynamic_client_registration: true
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.lili.co
  name: mcp-oauth2
  pkce: S256
  refresh_tokens: true
  registration_endpoint: https://mcp.lili.co/oauth/register
  revocation_endpoint: https://mcp.lili.co/oauth/revoke
  scopes: none
  scopes_note: The authorization-server metadata declares no scopes_supported. See scopes/lili-scopes.yml.
  subject: Tokens are scoped to the authenticated Lili user. Differentiation is by USER TYPE (business owner vs accountant), enforced server-side, not by scope.
  surface: MCP
  token_endpoint: https://mcp.lili.co/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: lili-authentication
source_filename: lili-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: https://dev.lili.co/guides/lili-quick-start\nalso:\n- https://dev.lili.co/guides/lili-mcp-connect\n- https://mcp.lili.co/.well-known/oauth-authorization-server\n- openapi/lili-application-api-openapi.yml\n- openapi/lili-customer-management-api-openapi.yml\n- openapi/lili-webhooks-api-openapi.yml\ndocs: https://dev.lili.co/guides/lili-quick-start\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Two credential models for two audiences. The partner REST APIs use a static accessKey/secretKey\n    pair in a custom Authorization scheme; the MCP server uses full OAuth 2.0 authorization code\n    with PKCE and dynamic client registration. Neither carries scopes.\nschemes:\n- name: accessKey\n  surface: REST\n  type: apiKey\n  in: header\n  parameter: Authorization\n  scheme_word: Lili\n  value_format: 'Lili <accessKey>:<secretKey>'\n  description: |-\n    The authorization in the format:<br/>\n\
  \    Authorization: Lili accessKey:secretKey\n  example_from_docs: 'curl -X GET https://prod.lili.co/lili/api/v1/webhooks -H \"Authorization: Lili accessKey:secretKey\"'\n  issuance:\n    self_serve: false\n    process: Contact dev-resources@lili.co. Lili issues an access/secret key pair per environment on account creation.\n    environments: [sandbox, production]\n    key_prefix_convention: none\n    key_prefix_note: >-\n      There is no test/live prefix. A sandbox key and a production key are indistinguishable by\n      inspection, so environment binding has to be enforced by the integrator's own configuration.\n  rotation_policy: not published\n  applies_to:\n  - openapi/lili-application-api-openapi.yml\n  - openapi/lili-customer-management-api-openapi.yml\n  - openapi/lili-webhooks-api-openapi.yml\n  operations: all\n  scopes: none\n- name: mcp-oauth2\n  surface: MCP\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://mcp.lili.co\n  authorization_endpoint:\
  \ https://mcp.lili.co/oauth/authorize\n  token_endpoint: https://mcp.lili.co/oauth/token\n  revocation_endpoint: https://mcp.lili.co/oauth/revoke\n  registration_endpoint: https://mcp.lili.co/oauth/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods_supported: [none]\n  bearer_methods_supported: [header]\n  grant_types: [authorization_code, refresh_token]\n  refresh_tokens: true\n  scopes: none\n  scopes_note: The authorization-server metadata declares no scopes_supported. See scopes/lili-scopes.yml.\n  subject: >-\n    Tokens are scoped to the authenticated Lili user. Differentiation is by USER TYPE (business\n    owner vs accountant), enforced server-side, not by scope.\n  discovery:\n  - well-known/lili-mcp-oauth-authorization-server.json\n  - well-known/lili-mcp-oauth-protected-resource.json\n  applies_to:\n  - https://mcp.lili.co/mcp\nwebhook_authentication:\n  direction: inbound-to-partner\n  v2: 'Authorization: Bearer <token issued at webhook creation>'\n\
  \  v1: 'lili-secret: <token issued at webhook creation>  (deprecated)'\n  ip_allowlist_published: true\n  signature: none\n  detail: asyncapi/lili-webhooks.yml\nembedded_authentication:\n  mechanism: JWT\n  detail: >-\n    The Create Application response returns a `token` (JWT) that is passed to the embedded\n    onboarding loader as `data-token`. It authorises exactly one applicant's onboarding session.\n  detail_file: components/lili-components.yml\nmfa: not applicable to the API surfaces\nmtls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lili/refs/heads/main/authentication/lili-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Banking
- Business Banking
- Financial Services
- Fintech
- Embedded Finance
- Onboarding
- KYC
- Webhooks
- MCP
- agent-native
- Invoicing
- Bill Pay
- Accounting
- Small Business
---
