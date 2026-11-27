---
anonymous_access: true
api_key_in: []
auth_types: []
description: Authentication for the COrdering / Plate & Fork white-label ordering MCP server, as stated on its docs page. No OpenAPI contract is published, so there are no securitySchemes to derive.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: COrdering Authentication
name_suffix: Authentication
oauth_flows: []
overview: COrdering declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: COrdering
provider_slug: cordering-com
scheme_count: 2
schemes:
- applies_to:
  - list_vendors
  - list_menu
  - check_order
  description: '"You can browse restaurants and menus without an account."'
  name: anonymous-browse
  type: none
- description: '"The first time you place an order, your assistant asks you to connect your Plate & Fork account, and you sign in with Google or Apple in a window it opens."'
  flow_tools:
  - login
  - submit_login_code
  - list_accounts
  - switch_account
  - logout
  identity_providers:
  - Google
  - Apple
  name: restaurant-account-sign-in
  note: The live tools/list (examples/cordering-com-mcp-tools-list.json) exposes login / submit_login_code tools for this sign-in. On 2026-11-04 GET https://wl-mcp.cordering.com/.well-known/oauth-protected-resource, /.well-known/oauth-protected-resource/mcp and /.well-known/oauth-authorization-server all returned 404, so no MCP OAuth discovery metadata is published. Auth endpoints were not called.
  type: oauth2-like-user-sign-in
slug: cordering-com-authentication
source_filename: cordering-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://wl-mcp.cordering.com/\ndocs: https://wl-mcp.cordering.com/\ndescription: Authentication for the COrdering / Plate & Fork white-label ordering MCP server, as stated on its docs page. No OpenAPI contract is published, so there are no securitySchemes to derive.\nschemes:\n- name: anonymous-browse\n  type: none\n  description: '\"You can browse restaurants and menus without an account.\"'\n  applies_to: [list_vendors, list_menu, check_order]\n- name: restaurant-account-sign-in\n  type: oauth2-like-user-sign-in\n  description: '\"The first time you place an order, your assistant asks you to connect your Plate & Fork account, and you sign in with Google or Apple in a window it opens.\"'\n  identity_providers: [Google, Apple]\n  flow_tools: [login, submit_login_code, list_accounts, switch_account, logout]\n  note: The live tools/list (examples/cordering-com-mcp-tools-list.json) exposes login / submit_login_code tools for this\
  \ sign-in. On 2026-11-04 GET https://wl-mcp.cordering.com/.well-known/oauth-protected-resource, /.well-known/oauth-protected-resource/mcp and /.well-known/oauth-authorization-server all returned 404, so no MCP OAuth discovery metadata is published. Auth endpoints were not called.\n"
source_yaml_url: https://artifacts.apis.io/cordering-com/authentication/cordering-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Food Ordering
- Restaurant
- Catering
- Corporate Meals
- Food Delivery
- Mobile App
- MCP
- Serbia
---
