---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Create Web Page Authentication
name_suffix: Authentication
oauth_flows: []
overview: Create Web Page declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Create Web Page
provider_slug: create-web-page-com
scheme_count: 2
schemes:
- description: Tool discovery, guided setup, demo creation, edits, preview, and publish are no-auth. The create tools return an editToken that must be passed to later write calls for that page.
  name: anonymous-edit-token
  source: https://create-web-page.com/llms-full.txt
  type: none
- description: Claiming a demo page and managing claimed pages use OAuth 2.1 with PKCE. Needed only for page_claim and account_page_manage (account_pages_list lists claimed pages once authenticated).
  dynamic_client_registration: https://create-web-page.com/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://create-web-page.com/oauth/authorize
      refreshUrl: https://create-web-page.com/oauth/token
      scopes:
        account:read: ''
        offline_access: ''
        pages:read: ''
        pages:write: ''
      tokenUrl: https://create-web-page.com/oauth/token
  metadata: https://create-web-page.com/.well-known/oauth-authorization-server
  name: oauth2
  pkce: S256
  protected_resource_metadata: https://create-web-page.com/.well-known/oauth-protected-resource
  revocation_endpoint: https://create-web-page.com/oauth/revoke
  source: https://create-web-page.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: create-web-page-com-authentication
source_filename: create-web-page-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://create-web-page.com/docs/mcp\ndocs: https://create-web-page.com/docs/mcp\nname: Create Web Page authentication\nnote: No OpenAPI is published; profile read from the MCP docs, llms-full.txt, the security page and the live OAuth discovery documents (/.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource, both HTTP 200 on 2026-11-04).\nschemes:\n- name: anonymous-edit-token\n  type: none\n  description: \"Tool discovery, guided setup, demo creation, edits, preview, and publish are no-auth. The create tools return an editToken that must be passed to later write calls for that page.\"\n  source: https://create-web-page.com/llms-full.txt\n- name: oauth2\n  type: oauth2\n  description: \"Claiming a demo page and managing claimed pages use OAuth 2.1 with PKCE. Needed only for page_claim and account_page_manage (account_pages_list lists claimed pages once authenticated).\"\n  flows:\n    authorizationCode:\n\
  \      authorizationUrl: https://create-web-page.com/oauth/authorize\n      tokenUrl: https://create-web-page.com/oauth/token\n      refreshUrl: https://create-web-page.com/oauth/token\n      scopes:\n        account:read: ''\n        pages:read: ''\n        pages:write: ''\n        offline_access: ''\n  pkce: S256\n  token_endpoint_auth_methods: [none]\n  revocation_endpoint: https://create-web-page.com/oauth/revoke\n  dynamic_client_registration: https://create-web-page.com/oauth/register\n  metadata: https://create-web-page.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://create-web-page.com/.well-known/oauth-protected-resource\n  source: https://create-web-page.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/create-web-page-com/authentication/create-web-page-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Website Builder
- Link-in-bio
- Digital Business Card
- MCP
- No-Code
---
