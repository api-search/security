---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: 8B Education Investments Authentication
name_suffix: Authentication
oauth_flows: []
overview: 8B Education Investments declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 8B Education Investments
provider_slug: 8b-education-investments
scheme_count: 1
schemes:
- applies_to: https://www.8b.africa/wp-json/mcp/mcp-oauth-server
  bearer:
    methods_supported:
    - header
    note: Bearer token in the Authorization header. No query-parameter or body form offered.
  client_authentication:
    note: Public clients only — the token endpoint accepts no client secret, which is the expected posture for MCP clients running on a user's machine and is why PKCE is mandatory rather than optional.
    token_endpoint_auth_methods_supported:
    - none
  client_registration:
    client_id_metadata_document_supported: true
    dynamic_client_registration_endpoint: null
    note: No RFC 7591 registration endpoint is advertised. Instead the server declares client_id_metadata_document_supported, so a client identifies itself by publishing a client-ID metadata document at an HTTPS URL and using that URL as its client_id.
  flows:
    authorization_code:
      authorization_url: https://www.8b.africa/oauth/authorize
      pkce_methods:
      - S256
      pkce_required: true
      refresh_supported: true
      revocation_url: https://www.8b.africa/oauth/revoke
      scopes:
        mcp: Access to the Model Context Protocol endpoint.
      token_url: https://www.8b.africa/oauth/token
  name: mcp_oauth
  type: oauth2
slug: 8b-education-investments-authentication
source_filename: 8b-education-investments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://www.8b.africa/.well-known/oauth-authorization-server ,\n  https://www.8b.africa/.well-known/oauth-protected-resource , and an anonymous\n  JSON-RPC POST to https://www.8b.africa/wp-json/mcp/mcp-oauth-server\ndocs: null\ndocs_note: >-\n  There is no authentication page to search: 8B publishes no developer documentation.\n  Everything below was read off documents the site actually serves or off a live\n  challenge response. derive-authentication.py produced nothing because the repository\n  holds no OpenAPI with securitySchemes.\nsummary: >-\n  The only authenticated API surface 8B exposes is its Model Context Protocol endpoint,\n  and it is protected by OAuth 2.1-style authorization code with PKCE. Discovery is\n  standards-correct end to end: the protected resource advertises its authorization\n  server, the authorization server advertises its endpoints and scope, and an\n  unauthenticated call returns 401 with\
  \ a WWW-Authenticate Bearer challenge that points\n  back at the resource metadata. No API keys, no basic auth, no mTLS and no OpenID\n  Connect are offered.\nschemes:\n- name: mcp_oauth\n  type: oauth2\n  applies_to: https://www.8b.africa/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorization_code:\n      authorization_url: https://www.8b.africa/oauth/authorize\n      token_url: https://www.8b.africa/oauth/token\n      revocation_url: https://www.8b.africa/oauth/revoke\n      refresh_supported: true\n      pkce_required: true\n      pkce_methods:\n      - S256\n      scopes:\n        mcp: Access to the Model Context Protocol endpoint.\n  client_authentication:\n    token_endpoint_auth_methods_supported:\n    - none\n    note: >-\n      Public clients only — the token endpoint accepts no client secret, which is the\n      expected posture for MCP clients running on a user's machine and is why PKCE is\n      mandatory rather than optional.\n  client_registration:\n    dynamic_client_registration_endpoint:\
  \ null\n    client_id_metadata_document_supported: true\n    note: >-\n      No RFC 7591 registration endpoint is advertised. Instead the server declares\n      client_id_metadata_document_supported, so a client identifies itself by publishing a\n      client-ID metadata document at an HTTPS URL and using that URL as its client_id.\n  bearer:\n    methods_supported:\n    - header\n    note: Bearer token in the Authorization header. No query-parameter or body form offered.\nchallenge:\n  observed: '2026-09-05'\n  url: https://www.8b.africa/wp-json/mcp/mcp-oauth-server\n  http_status: 401\n  www_authenticate: >-\n    Bearer realm=\"https://www.8b.africa\",\n    resource_metadata=\"https://www.8b.africa/.well-known/oauth-protected-resource\"\n  body: '{\"code\":\"mcp_unauthorized\",\"message\":\"MCP authentication required.\",\"data\":{\"status\":401}}'\n  note: >-\n    An RFC 9728 conformant challenge. An agent that receives this can discover how to\n    authenticate without any out-of-band\
  \ documentation, which matters here precisely\n    because there is no documentation.\nunauthenticated_surfaces:\n- url: https://www.8b.africa/llms.txt\n  status: 200\n  note: Served anonymously.\n- url: https://www.8b.africa/.well-known/oauth-authorization-server\n  status: 200\n- url: https://www.8b.africa/.well-known/oauth-protected-resource\n  status: 200\n- url: https://www.8b.africa/wp-json/\n  status: 200\n  note: >-\n    The WordPress core REST discovery index is anonymously readable and lists 449 routes\n    across 28 namespaces. It is the CMS platform's own API, not a product API 8B\n    publishes, and it is deliberately NOT registered as an 8B API in apis.yml. It is\n    recorded here only because it is the surface on which the MCP endpoint is mounted.\nabsent:\n- api_keys\n- http_basic\n- http_bearer_static\n- mutual_tls\n- openid_connect\n- jwt_signed_requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8b-education-investments/refs/heads/main/authentication/8b-education-investments-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Education
- Student Loans
- Financial Services
- Lending
- FinTech
- Africa
- Higher Education
- Study Abroad
- Community
---
