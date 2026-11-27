---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Custodio Legal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Custodio Legal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Custodio Legal
provider_slug: custodio-legal
scheme_count: 1
schemes:
- authorization_server: https://custodio.legal
  bearer_methods:
  - header
  description: Remote MCP clients authenticate with OAuth. The docs state a compatible client "Must support Streamable HTTP, OAuth with PKCE, dynamic registration, and credential refresh", and that "You do not copy a password or create an API key - the client opens Custodio's secure sign-in and receives a revocable credential."
  dynamic_client_registration: true
  grant_binding: An authorization belongs to one person, one practice, and one set of scopes.
  name: oauth2
  pkce: true
  protected_resource_metadata: https://custodio.legal/.well-known/oauth-protected-resource
  refresh: true
  revocation: My account -> How you sign in -> Authorized applications -> Revoke access; revocation immediately invalidates that grant's tokens.
  type: oauth2
slug: custodio-legal-authentication
source_filename: custodio-legal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.custodio.legal/en/manual/24-conectar-custodio-a-tu-asistente/\ndocs: https://docs.custodio.legal/en/manual/24-conectar-custodio-a-tu-asistente/\napplies_to: https://custodio.legal/mcp\nschemes:\n- name: oauth2\n  type: oauth2\n  description: Remote MCP clients authenticate with OAuth. The docs state a compatible client \"Must support Streamable HTTP, OAuth with PKCE, dynamic registration, and credential refresh\", and that \"You do not copy a password or create an API key - the client opens Custodio's secure sign-in and receives a revocable credential.\"\n  pkce: true\n  dynamic_client_registration: true\n  refresh: true\n  bearer_methods: [header]\n  authorization_server: https://custodio.legal\n  protected_resource_metadata: https://custodio.legal/.well-known/oauth-protected-resource\n  grant_binding: An authorization belongs to one person, one practice, and one set of scopes.\n  revocation: My account -> How\
  \ you sign in -> Authorized applications -> Revoke access; revocation immediately invalidates that grant's tokens.\napi_keys: none documented\nevidence:\n- url: https://custodio.legal/.well-known/oauth-protected-resource\n  http_status: 200\n  note: RFC 9728 document lists authorization_servers [https://custodio.legal], bearer_methods_supported [header], resource https://custodio.legal/mcp.\n- url: https://custodio.legal/mcp\n  http_status: 401\n  note: Unauthenticated request answered 401 (pre-flight contract discovery, 2026-11-04).\n"
source_yaml_url: https://artifacts.apis.io/custodio-legal/authentication/custodio-legal-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Legal
- Legal Tech
- Practice Management
- Judicial Monitoring
- Artificial Intelligence
- MCP
- Latin America
- Colombia
---
