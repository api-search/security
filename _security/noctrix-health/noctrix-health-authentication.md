---
api_key_in: []
auth_types: []
description: Noctrix Health publishes no developer program, no API keys and no documented auth page. The only authenticated surface that could be established anonymously is the OAuth 2.0 authorization server backing the Nidra MCP server on nidrarls.com, whose configuration was read verbatim from RFC 8414 Authorization Server Metadata. Everything below comes from that document and from the WWW-Authenticate challenge the MCP endpoint returns — nothing is inferred from marketing prose.
kind: authentication
layout: security
method: probed
name: Noctrix Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noctrix Health declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Noctrix Health
provider_slug: noctrix-health
scheme_count: 1
schemes:
- applies_to: https://nidrarls.com/wp-json/mcp/mcp-oauth-server
  bearer:
    challenge_observed: Bearer realm="https://nidrarls.com", resource_metadata="https://nidrarls.com/.well-known/oauth-protected-resource"
    error_body: '{"code":"mcp_unauthorized","message":"MCP authentication required.","data":{"status":401}}'
    http_status_on_missing_token: 401
    methods_supported:
    - header
  client_registration:
    client_id_metadata_document_supported: true
    dynamic_registration_endpoint: null
    note: No registration_endpoint is advertised. The server declares client_id_metadata_document_supported, i.e. a client identifies itself with a URL that resolves to its own client metadata document rather than pre-registering.
  flows:
    authorization_code:
      authorization_url: https://nidrarls.com/oauth/authorize
      refresh_url: https://nidrarls.com/oauth/token
      revocation_url: https://nidrarls.com/oauth/revoke
      scopes:
        mcp: Access to the Model Context Protocol server.
      token_url: https://nidrarls.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  id: nidra-mcp-oauth2
  iss_parameter_supported: true
  pkce:
    required_methods:
    - S256
  public_client: true
  response_types:
  - code
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: noctrix-health-authentication
source_filename: noctrix-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://nidrarls.com/.well-known/oauth-authorization-server\nname: Noctrix Health authentication profile\ndescription: >-\n  Noctrix Health publishes no developer program, no API keys and no documented auth page.\n  The only authenticated surface that could be established anonymously is the OAuth 2.0\n  authorization server backing the Nidra MCP server on nidrarls.com, whose configuration\n  was read verbatim from RFC 8414 Authorization Server Metadata. Everything below comes\n  from that document and from the WWW-Authenticate challenge the MCP endpoint returns —\n  nothing is inferred from marketing prose.\nschemes:\n- id: nidra-mcp-oauth2\n  type: oauth2\n  applies_to: https://nidrarls.com/wp-json/mcp/mcp-oauth-server\n  flows:\n    authorization_code:\n      authorization_url: https://nidrarls.com/oauth/authorize\n      token_url: https://nidrarls.com/oauth/token\n      refresh_url: https://nidrarls.com/oauth/token\n     \
  \ revocation_url: https://nidrarls.com/oauth/revoke\n      scopes:\n        mcp: Access to the Model Context Protocol server.\n  pkce:\n    required_methods: [S256]\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  token_endpoint_auth_methods: [none]\n  public_client: true\n  client_registration:\n    dynamic_registration_endpoint: null\n    client_id_metadata_document_supported: true\n    note: >-\n      No registration_endpoint is advertised. The server declares\n      client_id_metadata_document_supported, i.e. a client identifies itself with a URL\n      that resolves to its own client metadata document rather than pre-registering.\n  bearer:\n    methods_supported: [header]\n    challenge_observed: >-\n      Bearer realm=\"https://nidrarls.com\",\n      resource_metadata=\"https://nidrarls.com/.well-known/oauth-protected-resource\"\n    http_status_on_missing_token: 401\n    error_body: '{\"code\":\"mcp_unauthorized\",\"message\":\"MCP authentication\
  \ required.\",\"data\":{\"status\":401}}'\n  iss_parameter_supported: true\nunauthenticated_surfaces:\n- surface: https://nidrarls.com/wp-json/wp/v2/*\n  auth: none\n  note: >-\n    The site's WordPress REST API answers read requests anonymously (HTTP 200). This is a\n    CMS default on the marketing/product site, not a published Noctrix Health developer\n    API, and is recorded for completeness only.\nnot_found:\n  api_keys: No API key issuance, key prefix or key management surface is published.\n  openid_connect: /.well-known/openid-configuration returned 404 on nidrarls.com.\n  mutual_tls: Not advertised.\n  docs_page: >-\n    No developer or authentication documentation page exists on either host. The\n    corporate host noctrixhealth.com is behind a SiteGround bot challenge (HTTP 202)\n    for every path, so it could not be read anonymously.\nchecked: '2026-08-26'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noctrix-health/refs/heads/main/authentication/noctrix-health-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Health
- Medical Devices
- Digital Health
- Sleep
- Neurology
- Neurostimulation
- Wearables
- MCP
- Agent Readiness
---
