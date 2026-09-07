---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: developerhub-documentation-api-openapi.yml
  format: yaml
  label: DeveloperHub Documentation API
  slug: developerhub-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-documentation-api-openapi.yml
- filename: developerhub-pages-api-openapi.yml
  format: yaml
  label: DeveloperHub Pages API
  slug: developerhub-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-pages-api-openapi.yml
- filename: developerhub-project-api-openapi.yml
  format: yaml
  label: DeveloperHub Project API
  slug: developerhub-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-project-api-openapi.yml
- filename: developerhub-reader-access-api-openapi.yml
  format: yaml
  label: DeveloperHub Reader Access API
  slug: developerhub-reader-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-reader-access-api-openapi.yml
- filename: developerhub-references-api-openapi.yml
  format: yaml
  label: DeveloperHub References API
  slug: developerhub-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-references-api-openapi.yml
- filename: developerhub-versions-api-openapi.yml
  format: yaml
  label: DeveloperHub Versions API
  slug: developerhub-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-versions-api-openapi.yml
- filename: developerhub-changelog-api-openapi.yml
  format: yaml
  label: DeveloperHub Changelog API
  slug: developerhub-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/openapi/developerhub-changelog-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Developerhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeveloperHub secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DeveloperHub
provider_slug: developerhub
scheme_count: 2
schemes:
- applied_to: all 25 operations (top-level security requirement)
  description: 'Generate an API Key from the DeveloperHub.io platform (https://app.developerhub.io) and provide it in the header, e.g. --header "X-Api-Key: <api-key>", for all requests requiring this authentication.'
  docs: https://docs.developerhub.io/support-center/api-key
  in: header
  issuance: Project Settings → API Keys. Keys are per project, and each key carries its own permission set.
  name: Api-Key
  observed:
  - body: '{"error":{"message":"No API Key was provided. Read our API Reference at https://docs.developerhub.io/api","httpCode":403,"code":403}}'
    request: GET https://api.developerhub.io/api/v1/version with no key
    status: 403
  - body: '{"error":{"message":"API Key is invalid","httpCode":400,"code":0}}'
    request: GET https://api.developerhub.io/api/v1/version with an invalid key
    status: 400
  parameter: X-Api-Key
  permissions_documented:
  - changelog.edit
  - changelog.read
  permissions_note: The docs say "Each API Key can have different permissions. Consult the API to know which permissions you need", but only the two changelog operations name their permission in the contract. There is no published permissions reference page.
  rotation: Not documented. The docs describe generating and copying a key; no rotation, expiry or last-used signal is published.
  sources:
  - openapi/_original/developerhub-openapi.yml
  surface: https://api.developerhub.io/api/v1
  transport: TLS only
  type: apiKey
- authorization_endpoint: https://ai.developerhub.io/authorize
  cross_reference: scopes/developerhub-scopes.yml
  description: Each editor connects with their own DeveloperHub account and the agent acts as that person, so it reaches only the projects they can already edit and only those with the Editor MCP server turned on. The first connection opens a browser consent page naming the client, the account and the address the approval is sent to. The connection lasts as long as the DeveloperHub login.
  docs: https://docs.developerhub.io/support-center/editor-mcp-server
  dynamic_client_registration: true
  flow: authorization_code
  issuer: https://ai.developerhub.io/
  name: Editor MCP OAuth
  observed:
  - body: '{"error":"invalid_token","error_description":"Missing editor access token"}'
    request: POST https://ai.developerhub.io/mcp with no token
    status: 401
    www_authenticate: Bearer resource_metadata="https://ai.developerhub.io/.well-known/oauth-protected-resource"
  pkce: S256
  registration_endpoint: https://ai.developerhub.io/register
  scopes:
  - editor
  surface: https://ai.developerhub.io/mcp
  token_endpoint: https://ai.developerhub.io/token
  type: oauth2
slug: developerhub-authentication
source_filename: developerhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://docs.developerhub.io/support-center/api-key ,\n  https://docs.developerhub.io/support-center/editor-mcp-server ,\n  https://ai.developerhub.io/.well-known/oauth-authorization-server ,\n  openapi/_original/developerhub-openapi.yml ; live unauthenticated responses observed against\n  https://api.developerhub.io/api/v1/version on 2026-09-06\nprovider: DeveloperHub\nproviderId: developerhub\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  surfaces: 2\n  note: >-\n    Two authentication surfaces, one per product. The v1 REST API is API-key only. The hosted Editor\n    MCP server is OAuth 2.0 only and has no key at all — \"There is no key to create or share out.\"\nschemes:\n- name: Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  surface: https://api.developerhub.io/api/v1\n  description: >-\n    Generate an API Key from the DeveloperHub.io platform (https://app.developerhub.io)\
  \ and provide\n    it in the header, e.g. --header \"X-Api-Key: <api-key>\", for all requests requiring this\n    authentication.\n  issuance: Project Settings → API Keys. Keys are per project, and each key carries its own permission set.\n  rotation: >-\n    Not documented. The docs describe generating and copying a key; no rotation, expiry or\n    last-used signal is published.\n  permissions_documented:\n  - changelog.edit\n  - changelog.read\n  permissions_note: >-\n    The docs say \"Each API Key can have different permissions. Consult the API to know which\n    permissions you need\", but only the two changelog operations name their permission in the\n    contract. There is no published permissions reference page.\n  transport: TLS only\n  applied_to: all 25 operations (top-level security requirement)\n  docs: https://docs.developerhub.io/support-center/api-key\n  observed:\n  - request: GET https://api.developerhub.io/api/v1/version with no key\n    status: 403\n    body: '{\"error\"\
  :{\"message\":\"No API Key was provided. Read our API Reference at https://docs.developerhub.io/api\",\"httpCode\":403,\"code\":403}}'\n  - request: GET https://api.developerhub.io/api/v1/version with an invalid key\n    status: 400\n    body: '{\"error\":{\"message\":\"API Key is invalid\",\"httpCode\":400,\"code\":0}}'\n  sources:\n  - openapi/_original/developerhub-openapi.yml\n- name: Editor MCP OAuth\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  surface: https://ai.developerhub.io/mcp\n  issuer: https://ai.developerhub.io/\n  authorization_endpoint: https://ai.developerhub.io/authorize\n  token_endpoint: https://ai.developerhub.io/token\n  registration_endpoint: https://ai.developerhub.io/register\n  dynamic_client_registration: true\n  scopes:\n  - editor\n  description: >-\n    Each editor connects with their own DeveloperHub account and the agent acts as that person, so\n    it reaches only the projects they can already edit and only those with the Editor MCP server\n\
  \    turned on. The first connection opens a browser consent page naming the client, the account and\n    the address the approval is sent to. The connection lasts as long as the DeveloperHub login.\n  observed:\n  - request: POST https://ai.developerhub.io/mcp with no token\n    status: 401\n    www_authenticate: 'Bearer resource_metadata=\"https://ai.developerhub.io/.well-known/oauth-protected-resource\"'\n    body: '{\"error\":\"invalid_token\",\"error_description\":\"Missing editor access token\"}'\n  docs: https://docs.developerhub.io/support-center/editor-mcp-server\n  cross_reference: scopes/developerhub-scopes.yml\nreader_authentication:\n  note: >-\n    Distinct from API authentication: DeveloperHub also authenticates READERS of a customer's docs\n    site (custom login, magic-link email invite, reader SSO, and a ?jwt= query parameter). The REST\n    API touches this through get_reader_access / create_reader_access / revoke_reader_access, which\n    manage invited readers by email\
  \ address.\n  docs: https://docs.developerhub.io/support-center/private-docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/developerhub/refs/heads/main/authentication/developerhub-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- API Reference
- Developer Portals
- Documentation
- Knowledge Base
- OpenAPI
- Docs as Code
- Model Context Protocol
- Agent Skills
---
