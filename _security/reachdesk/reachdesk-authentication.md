---
api_key_in:
- header
api_specs:
- filename: reachdesk-api-openapi.yml
  format: yaml
  label: Reachdesk API
  slug: reachdesk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/openapi/reachdesk-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: Reachdesk runs two independent authentication models on the same host. The REST API at https://app.reachdesk.com/api/v2 uses a long-lived organization API token presented as a bearer credential in the Authorization header. The remote MCP server at https://app.reachdesk.com/mcp uses OAuth 2.1 with dynamic client registration and PKCE. They do not share credentials.
kind: authentication
layout: security
method: searched
name: Reachdesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reachdesk secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Reachdesk
provider_slug: reachdesk
scheme_count: 2
schemes:
- applies_to: all 9 REST operations (declared as a root-level security requirement)
  example_request: "curl https://app.reachdesk.com/api/v2/organization \\\n  -H \"Authorization: Bearer {api_token}\"\n"
  format: Bearer {api_token}
  in: header
  name: sec0
  notes:
  - The OpenAPI declares this as type apiKey with x-bearer-format bearer, so the literal header value is "Bearer <token>" even though the scheme is not modelled as http/bearer.
  - No token expiry, rotation cadence or scope model is documented. The token carries whatever the organization can do; there is no per-endpoint restriction published.
  parameter: Authorization
  provisioning: An Organization Admin creates and revokes tokens in the Reachdesk platform under Organization > Settings > API Tokens > Add New. Tokens are organization-scoped, not per-user.
  sources:
  - openapi/reachdesk-api-openapi.yml
  - https://reachdesk.readme.io/reference/authentication
  - https://support.reachdesk.com/hc/en-gb/articles/29669486204305-Send-gifts-with-the-Reachdesk-Trigger-Campaign-API
  surface: rest
  token_management: https://app.reachdesk.com/api_tokens
  type: apiKey
- applies_to: https://app.reachdesk.com/mcp
  authorization_endpoint: https://app.reachdesk.com/oauth/authorize
  dynamic_client_registration: true
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  issuer: https://app.reachdesk.com
  name: mcp-oauth
  notes:
  - Discovered by probe. Reachdesk does not document this OAuth surface in its API reference or knowledge base.
  pkce: S256
  registration_endpoint: https://app.reachdesk.com/oauth/register
  scopes:
  - mcp:tools.user.read
  - mcp:tools.user.write
  sources:
  - well-known/reachdesk-oauth-authorization-server.json
  - well-known/reachdesk-oauth-protected-resource.json
  surface: mcp
  token_endpoint: https://app.reachdesk.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
slug: reachdesk-authentication
source_filename: reachdesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://reachdesk.readme.io/reference/authentication\ndocs: https://reachdesk.readme.io/reference/authentication\nderived_from: openapi/reachdesk-api-openapi.yml\ndescription: >-\n  Reachdesk runs two independent authentication models on the same host. The REST\n  API at https://app.reachdesk.com/api/v2 uses a long-lived organization API token\n  presented as a bearer credential in the Authorization header. The remote MCP\n  server at https://app.reachdesk.com/mcp uses OAuth 2.1 with dynamic client\n  registration and PKCE. They do not share credentials.\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_surface: mcp\nschemes:\n  - name: sec0\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: 'Bearer {api_token}'\n    surface: rest\n    applies_to: all 9 REST operations (declared as a root-level security requirement)\n    token_management: https://app.reachdesk.com/api_tokens\n\
  \    provisioning: >-\n      An Organization Admin creates and revokes tokens in the Reachdesk platform\n      under Organization > Settings > API Tokens > Add New. Tokens are\n      organization-scoped, not per-user.\n    example_request: |\n      curl https://app.reachdesk.com/api/v2/organization \\\n        -H \"Authorization: Bearer {api_token}\"\n    sources:\n      - openapi/reachdesk-api-openapi.yml\n      - https://reachdesk.readme.io/reference/authentication\n      - https://support.reachdesk.com/hc/en-gb/articles/29669486204305-Send-gifts-with-the-Reachdesk-Trigger-Campaign-API\n    notes:\n      - >-\n        The OpenAPI declares this as type apiKey with x-bearer-format bearer, so\n        the literal header value is \"Bearer <token>\" even though the scheme is not\n        modelled as http/bearer.\n      - >-\n        No token expiry, rotation cadence or scope model is documented. The token\n        carries whatever the organization can do; there is no per-endpoint\n      \
  \  restriction published.\n  - name: mcp-oauth\n    type: oauth2\n    surface: mcp\n    applies_to: https://app.reachdesk.com/mcp\n    issuer: https://app.reachdesk.com\n    authorization_endpoint: https://app.reachdesk.com/oauth/authorize\n    token_endpoint: https://app.reachdesk.com/oauth/token\n    registration_endpoint: https://app.reachdesk.com/oauth/register\n    grant_types:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n    pkce: S256\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    scopes:\n      - mcp:tools.user.read\n      - mcp:tools.user.write\n    dynamic_client_registration: true\n    sources:\n      - well-known/reachdesk-oauth-authorization-server.json\n      - well-known/reachdesk-oauth-protected-resource.json\n    notes:\n      - >-\n        Discovered by probe. Reachdesk does not document this OAuth surface in its\n        API reference or knowledge base.\n\nplatform_identity:\n\
  \  description: >-\n    Distinct from API authentication: end-user access to the Reachdesk application\n    supports SAML SSO and SCIM 2.0 user provisioning. These govern human logins,\n    not API calls.\n  saml_sso:\n    supported: true\n    providers:\n      - Okta\n      - Microsoft Entra ID\n      - OneLogin\n    jit_provisioning: true\n    source: https://support.reachdesk.com/hc/en-gb/articles/4420374592017-Just-in-Time-JIT-Provisioning-SAML\n  scim:\n    supported: true\n    version: '2.0'\n    source: https://support.reachdesk.com/hc/en-gb/articles/29322223500689-How-to-enable-SCIM-user-provisioning-in-Okta\n\ngaps:\n  - No documented token rotation or expiry policy for REST API tokens.\n  - No scope or permission model on the REST API — one token, full organization access.\n  - >-\n    The MCP OAuth surface is undocumented; a developer cannot learn it exists\n    without probing the host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reachdesk/refs/heads/main/authentication/reachdesk-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Corporate Gifting
- Direct Mail
- Swag
- B2B
- Sales Enablement
- Customer Success
- Marketing Automation
- Gifting Platform
- Rewards
- MCP
- AI Agents
- OpenAPI
---
