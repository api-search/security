---
api_key_in: []
api_specs:
- filename: fabric8labs-posts-api-openapi.yml
  format: yaml
  label: Fabric8Labs Posts API
  slug: fabric8labs-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-posts-api-openapi.yml
- filename: fabric8labs-pages-api-openapi.yml
  format: yaml
  label: Fabric8Labs Pages API
  slug: fabric8labs-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-pages-api-openapi.yml
- filename: fabric8labs-media-api-openapi.yml
  format: yaml
  label: Fabric8Labs Media API
  slug: fabric8labs-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-media-api-openapi.yml
- filename: fabric8labs-team-api-openapi.yml
  format: yaml
  label: Fabric8Labs Team API
  slug: fabric8labs-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-team-api-openapi.yml
- filename: fabric8labs-taxonomy-api-openapi.yml
  format: yaml
  label: Fabric8Labs Taxonomy API
  slug: fabric8labs-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-taxonomy-api-openapi.yml
- filename: fabric8labs-search-api-openapi.yml
  format: yaml
  label: Fabric8Labs Search API
  slug: fabric8labs-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-search-api-openapi.yml
- filename: fabric8labs-discovery-api-openapi.yml
  format: yaml
  label: Fabric8Labs Discovery API
  slug: fabric8labs-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/openapi/fabric8labs-discovery-api-openapi.yml
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Fabric8Labs Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Fabric8Labs secures its APIs with none and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Fabric8Labs
provider_slug: fabric8labs
scheme_count: 3
schemes:
- applies_to: https://www.fabric8labs.com/wp-json/wp/v2
  description: Every operation in the seven OpenAPI documents under openapi/ was verified to return HTTP 200 with no Authorization header. WordPress applies read permission per post status, so only published records are visible anonymously.
  name: anonymous
  sources:
  - openapi/fabric8labs-posts-api-openapi.yml
  - openapi/fabric8labs-pages-api-openapi.yml
  - openapi/fabric8labs-media-api-openapi.yml
  - openapi/fabric8labs-team-api-openapi.yml
  - openapi/fabric8labs-taxonomy-api-openapi.yml
  - openapi/fabric8labs-search-api-openapi.yml
  - openapi/fabric8labs-discovery-api-openapi.yml
  type: none
- applies_to: https://www.fabric8labs.com/wp-json/mcp/mcp-oauth-server
  description: OAuth 2.1 protection on the WordPress MCP Adapter endpoint, discoverable via RFC 9728 protected-resource metadata. An anonymous JSON-RPC tools/list returns HTTP 401 mcp_unauthorized with WWW-Authenticate Bearer realm="https://www.fabric8labs.com", resource_metadata="https://www.fabric8labs.com/.well-known/oauth-protected-resource".
  flows:
  - authorizationUrl: https://www.fabric8labs.com/oauth/authorize
    client_registration: No dynamic client registration endpoint is advertised. The metadata sets client_id_metadata_document_supported = true, so clients are expected to identify themselves with a client-ID metadata document URL rather than pre-registering.
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    revocationUrl: https://www.fabric8labs.com/oauth/revoke
    scopes:
      mcp: The only scope the authorization server advertises. Grants access to the MCP endpoint.
    tokenUrl: https://www.fabric8labs.com/oauth/token
    token_endpoint_auth_methods:
    - none
  name: MCPOAuth
  sources:
  - well-known/fabric8labs-oauth-authorization-server.json
  - well-known/fabric8labs-oauth-protected-resource.json
  type: oauth2
- applies_to: https://www.fabric8labs.com/wp-json/wp/v2
  description: The route index registers /wp/v2/users/{user_id}/application-passwords, the WordPress application-password endpoints, which means HTTP Basic with an application password is the mechanism for the authenticated write half of the REST API. This is administrative access for site operators, not a developer credential Fabric8Labs issues to third parties — there is no signup, no key request and no pricing for it.
  name: WordPressApplicationPasswords
  scheme: basic
  sources:
  - openapi/_source/fabric8labs-wp-json-root.json
  type: http
slug: fabric8labs-authentication
source_filename: fabric8labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  Live anonymous probes of www.fabric8labs.com plus the RFC 8414 / RFC 9728 documents saved in\n  well-known/. Fabric8Labs publishes no authentication documentation of any kind — there is no\n  developer portal, no API reference and no docs host — so every statement below is an observed\n  runtime fact, not a provider claim.\nsummary:\n  types:\n  - none\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  note: >-\n    The surface splits cleanly in two. The public WordPress REST content surface (wp/v2) requires no\n    credential at all: it answers anonymously with HTTP 200 and declares no securityScheme, which is\n    why 0-working/derive-authentication.py found no schemes to aggregate across the seven OpenAPI\n    documents in openapi/. The MCP endpoint is the opposite: it is fully gated behind an OAuth 2.1\n    authorization-code + PKCE flow served by the site itself.\nschemes:\n- name: anonymous\n\
  \  type: none\n  applies_to: https://www.fabric8labs.com/wp-json/wp/v2\n  description: >-\n    Every operation in the seven OpenAPI documents under openapi/ was verified to return HTTP 200\n    with no Authorization header. WordPress applies read permission per post status, so only\n    published records are visible anonymously.\n  sources:\n  - openapi/fabric8labs-posts-api-openapi.yml\n  - openapi/fabric8labs-pages-api-openapi.yml\n  - openapi/fabric8labs-media-api-openapi.yml\n  - openapi/fabric8labs-team-api-openapi.yml\n  - openapi/fabric8labs-taxonomy-api-openapi.yml\n  - openapi/fabric8labs-search-api-openapi.yml\n  - openapi/fabric8labs-discovery-api-openapi.yml\n- name: MCPOAuth\n  type: oauth2\n  applies_to: https://www.fabric8labs.com/wp-json/mcp/mcp-oauth-server\n  description: >-\n    OAuth 2.1 protection on the WordPress MCP Adapter endpoint, discoverable via RFC 9728\n    protected-resource metadata. An anonymous JSON-RPC tools/list returns HTTP 401 mcp_unauthorized\n  \
  \  with WWW-Authenticate Bearer realm=\"https://www.fabric8labs.com\",\n    resource_metadata=\"https://www.fabric8labs.com/.well-known/oauth-protected-resource\".\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.fabric8labs.com/oauth/authorize\n    tokenUrl: https://www.fabric8labs.com/oauth/token\n    revocationUrl: https://www.fabric8labs.com/oauth/revoke\n    pkce: S256\n    grant_types:\n    - authorization_code\n    - refresh_token\n    scopes:\n      mcp: The only scope the authorization server advertises. Grants access to the MCP endpoint.\n    token_endpoint_auth_methods:\n    - none\n    client_registration: >-\n      No dynamic client registration endpoint is advertised. The metadata sets\n      client_id_metadata_document_supported = true, so clients are expected to identify themselves\n      with a client-ID metadata document URL rather than pre-registering.\n  sources:\n  - well-known/fabric8labs-oauth-authorization-server.json\n  - well-known/fabric8labs-oauth-protected-resource.json\n\
  - name: WordPressApplicationPasswords\n  type: http\n  scheme: basic\n  applies_to: https://www.fabric8labs.com/wp-json/wp/v2\n  description: >-\n    The route index registers /wp/v2/users/{user_id}/application-passwords, the WordPress\n    application-password endpoints, which means HTTP Basic with an application password is the\n    mechanism for the authenticated write half of the REST API. This is administrative access for\n    site operators, not a developer credential Fabric8Labs issues to third parties — there is no\n    signup, no key request and no pricing for it.\n  sources:\n  - openapi/_source/fabric8labs-wp-json-root.json\ngated_surfaces:\n- endpoint: /wp-json/wp/v2/users\n  status: 401\n  code: rest_user_cannot_view\n- endpoint: /wp-json/wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- endpoint: /wp-json/wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n- endpoint: /wp-json/gf/v2/forms\n  status: 401\n  code: rest_forbidden\n- endpoint: /wp-json/mcp/mcp-oauth-server\n\
  \  status: 401\n  code: mcp_unauthorized\n- endpoint: /wp-json/wp/v2/comments\n  status: 403\n  code: rest_comment_disabled\nx-evidence:\n  fetched: '2026-08-12'\n  host: www.fabric8labs.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric8labs/refs/heads/main/authentication/fabric8labs-authentication.yml
summary_line: none/oauth2 · 3 schemes
tags:
- Company
- Advanced Manufacturing
- Additive Manufacturing
- 3D Printing
- Metal 3D Printing
- Electrochemical Additive Manufacturing
- Thermal Management
- Liquid Cooling
- Data Centers
- Semiconductors
- Electronics
- Aerospace
- Photonics
- Power Electronics
- Hardware
- Content
---
