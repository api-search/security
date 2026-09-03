---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Veradermics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veradermics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Veradermics
provider_slug: veradermics
scheme_count: 2
schemes:
- applies_to:
  - https://www.veradermics.com/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://www.veradermics.com/oauth/authorize
  client_registration: client_id_metadata_document_supported is true — clients identify themselves with a hosted client-id metadata document rather than by pre-registration.
  client_type: public
  code_challenge_methods_supported:
  - S256
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oauth2_mcp
  issuer: https://www.veradermics.com
  pkce_required: true
  response_types_supported:
  - code
  revocation_endpoint: https://www.veradermics.com/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://www.veradermics.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to:
  - https://www.veradermics.com/wp-json/mcp/mcp-adapter-default-server
  - https://www.veradermics.com/wp-json/wp-abilities/v1/abilities
  id: wordpress_session
  note: The second registered MCP server, /wp-json/mcp/mcp-adapter-default-server, and the wp-abilities/v1 namespace both answer 401 rest_forbidden to anonymous requests, which is the WordPress core REST permission response — they expect a logged-in session or an application password rather than the OAuth bearer above.
  type: cookie-or-application-password
slug: veradermics-authentication
source_filename: veradermics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://www.veradermics.com/.well-known/oauth-authorization-server\nnote: >-\n  Veradermics publishes no authentication documentation, because it publishes no\n  developer program. This profile is read entirely from the RFC 8414 / RFC 9728 metadata\n  documents the WordPress MCP Adapter serves on the corporate marketing host, and it\n  therefore describes access to that incidental MCP surface — not to any Veradermics\n  product API. Nothing here was derived from an OpenAPI: this provider publishes none.\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  flow: authorization_code\n  issuer: https://www.veradermics.com\n  authorization_endpoint: https://www.veradermics.com/oauth/authorize\n  token_endpoint: https://www.veradermics.com/oauth/token\n  revocation_endpoint: https://www.veradermics.com/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  code_challenge_methods_supported:\n\
  \  - S256\n  pkce_required: true\n  token_endpoint_auth_methods_supported:\n  - none\n  client_type: public\n  client_registration: >-\n    client_id_metadata_document_supported is true — clients identify themselves with a\n    hosted client-id metadata document rather than by pre-registration.\n  scopes:\n  - mcp\n  applies_to:\n  - https://www.veradermics.com/wp-json/mcp/mcp-oauth-server\n- id: wordpress_session\n  type: cookie-or-application-password\n  note: >-\n    The second registered MCP server, /wp-json/mcp/mcp-adapter-default-server, and the\n    wp-abilities/v1 namespace both answer 401 rest_forbidden to anonymous requests,\n    which is the WordPress core REST permission response — they expect a logged-in\n    session or an application password rather than the OAuth bearer above.\n  applies_to:\n  - https://www.veradermics.com/wp-json/mcp/mcp-adapter-default-server\n  - https://www.veradermics.com/wp-json/wp-abilities/v1/abilities\nanonymous_surface:\n  note: >-\n    The WordPress\
  \ core REST namespace wp/v2 answers anonymously on this host for public\n    content (pages, types), which is default WordPress behaviour rather than a published\n    API. It is recorded for completeness and is not wired as a Veradermics API.\n  probes:\n  - url: https://www.veradermics.com/wp-json/wp/v2/pages?per_page=1\n    status: 200\n  - url: https://www.veradermics.com/wp-json/wp/v2/types\n    status: 200\nx-evidence:\n  fetched: '2026-09-02'\n  probes:\n  - url: https://www.veradermics.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://www.veradermics.com/.well-known/oauth-protected-resource\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veradermics/refs/heads/main/authentication/veradermics-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Healthcare
- Dermatology
- Clinical Trials
- Drug Development
---
