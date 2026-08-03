---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: probed
name: Dispatchhealth Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DispatchHealth secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DispatchHealth
provider_slug: dispatchhealth
scheme_count: 2
schemes:
- bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  code_challenge_methods:
  - S256
  flows:
  - authorizationUrl: https://www.dispatchhealth.com/oauth/authorize
    flow: authorizationCode
    refreshSupported: true
    revocationUrl: https://www.dispatchhealth.com/oauth/revoke
    scopes:
      mcp: Access the DispatchHealth WordPress MCP server
    tokenUrl: https://www.dispatchhealth.com/oauth/token
  issuer: https://www.dispatchhealth.com
  name: MCPOAuth2
  protects:
  - https://www.dispatchhealth.com/wp-json/mcp/mcp-oauth-server
  sources:
  - well-known/dispatchhealth-oauth-authorization-server.json
  - well-known/dispatchhealth-oauth-protected-resource.json
  standards:
  - RFC 6749
  - RFC 8414
  - RFC 9728
  - RFC 7636
  token_endpoint_auth_methods:
  - none
  type: oauth2
- authorization_page: https://www.dispatchhealth.com/wp-admin/authorize-application.php
  name: WordPressApplicationPasswords
  note: advertised in the WordPress REST API index `authentication` block; covers the wp/v2 and mcp-adapter-default-server routes
  scheme: basic
  sources:
  - https://www.dispatchhealth.com/wp-json/
  type: http
slug: dispatchhealth-authentication
source_filename: dispatchhealth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: https://www.dispatchhealth.com/.well-known/oauth-authorization-server\ndocs: null\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: [S256]\n  public_clients: true\nschemes:\n- name: MCPOAuth2\n  type: oauth2\n  sources:\n  - well-known/dispatchhealth-oauth-authorization-server.json\n  - well-known/dispatchhealth-oauth-protected-resource.json\n  issuer: https://www.dispatchhealth.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.dispatchhealth.com/oauth/authorize\n    tokenUrl: https://www.dispatchhealth.com/oauth/token\n    revocationUrl: https://www.dispatchhealth.com/oauth/revoke\n    refreshSupported: true\n    scopes:\n      mcp: Access the DispatchHealth WordPress MCP server\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  client_id_metadata_document_supported: true\n  protects:\n  - https://www.dispatchhealth.com/wp-json/mcp/mcp-oauth-server\n\
  \  bearer_methods_supported: [header]\n  standards: [RFC 6749, RFC 8414, RFC 9728, RFC 7636]\n- name: WordPressApplicationPasswords\n  type: http\n  scheme: basic\n  sources:\n  - https://www.dispatchhealth.com/wp-json/\n  authorization_page: https://www.dispatchhealth.com/wp-admin/authorize-application.php\n  note: advertised in the WordPress REST API index `authentication` block; covers the\n    wp/v2 and mcp-adapter-default-server routes\nnotes: 'Only the marketing-site surface has a discoverable authentication contract.\n  The partner portal (express.dispatchhealth.com) and patient request flow (request.dispatchhealth.com)\n  are interactive logins with no published machine-readable auth metadata, and api.dispatchhealth.com\n  answers 204 to every anonymous request.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatchhealth/refs/heads/main/authentication/dispatchhealth-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Healthcare
- Health Systems
- Hospital at Home
- Home Health
- Urgent Care
- Care Delivery
- Medical Services
- Telehealth
- Digital Health
---
