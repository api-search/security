---
api_key_in: []
auth_types: []
description: Axena Health publishes no developer authentication documentation, because it publishes no developer program. This profile is derived entirely from the anonymous OAuth discovery documents the WordPress MCP Adapter serves on levacares.com, plus the authentication block advertised by the WordPress REST API discovery root on both hosts. Nothing here was read from a docs page, because no docs page exists.
kind: authentication
layout: security
method: probed
name: Axena Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axena Health declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Axena Health
provider_slug: axena-health
scheme_count: 2
schemes:
- client_authentication:
    note: Public clients only — no client secret is accepted at the token endpoint.
    token_endpoint_auth_methods:
    - none
  client_registration:
    client_id_metadata_document_supported: true
    dynamic_client_registration: not-advertised
  discovery:
    authorization_server_metadata: https://levacares.com/.well-known/oauth-authorization-server
    protected_resource_metadata: https://levacares.com/.well-known/oauth-protected-resource
  flows:
    authorizationCode:
      authorizationUrl: https://levacares.com/oauth/authorize
      refreshUrl: https://levacares.com/oauth/token
      revocationUrl: https://levacares.com/oauth/revoke
      scopes:
        mcp: Access the WordPress MCP Adapter endpoint on levacares.com
      tokenUrl: https://levacares.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  host: levacares.com
  id: mcp-oauth2
  pkce:
    code_challenge_methods:
    - S256
    required: true
  protected_resource: https://levacares.com/wp-json/mcp/mcp-oauth-server
  response_types:
  - code
  token_presentation:
    bearer_methods_supported:
    - header
  type: oauth2
- authorization_endpoint: https://levacares.com/wp-admin/authorize-application.php
  hosts:
  - levacares.com
  - axenahealth.com
  id: wp-application-passwords
  note: The WordPress REST API discovery root advertises Application Passwords as its authentication mechanism, with the authorization endpoint at /wp-admin/authorize-application.php. This is an administrative credential for the CMS, not a developer API key.
  scheme: basic
  type: http
slug: axena-health-authentication
source_filename: axena-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://levacares.com/.well-known/oauth-authorization-server\nname: Axena Health — authentication profile\ndescription: >-\n  Axena Health publishes no developer authentication documentation, because it\n  publishes no developer program. This profile is derived entirely from the\n  anonymous OAuth discovery documents the WordPress MCP Adapter serves on\n  levacares.com, plus the authentication block advertised by the WordPress REST\n  API discovery root on both hosts. Nothing here was read from a docs page,\n  because no docs page exists.\n\nx-nature: >-\n  Platform-level authentication for a WordPress install, not a product or\n  clinical API. The Leva mobile app's own authentication surface is not public\n  and was not probed.\n\nschemes:\n- id: mcp-oauth2\n  type: oauth2\n  host: levacares.com\n  flows:\n    authorizationCode:\n      authorizationUrl: https://levacares.com/oauth/authorize\n      tokenUrl: https://levacares.com/oauth/token\n\
  \      refreshUrl: https://levacares.com/oauth/token\n      revocationUrl: https://levacares.com/oauth/revoke\n      scopes:\n        mcp: Access the WordPress MCP Adapter endpoint on levacares.com\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  pkce:\n    required: true\n    code_challenge_methods: [S256]\n  client_authentication:\n    token_endpoint_auth_methods: [none]\n    note: Public clients only — no client secret is accepted at the token endpoint.\n  client_registration:\n    client_id_metadata_document_supported: true\n    dynamic_client_registration: not-advertised\n  token_presentation:\n    bearer_methods_supported: [header]\n  protected_resource: https://levacares.com/wp-json/mcp/mcp-oauth-server\n  discovery:\n    authorization_server_metadata: https://levacares.com/.well-known/oauth-authorization-server\n    protected_resource_metadata: https://levacares.com/.well-known/oauth-protected-resource\n- id: wp-application-passwords\n  type: http\n\
  \  scheme: basic\n  hosts: [levacares.com, axenahealth.com]\n  note: >-\n    The WordPress REST API discovery root advertises Application Passwords as\n    its authentication mechanism, with the authorization endpoint at\n    /wp-admin/authorize-application.php. This is an administrative credential\n    for the CMS, not a developer API key.\n  authorization_endpoint: https://levacares.com/wp-admin/authorize-application.php\n\nanonymous_access:\n  note: >-\n    The default WordPress REST API read routes (wp/v2 posts, pages, media,\n    taxonomies) answer anonymously on both hosts. Every mcp/* route returns 401.\n\nx-evidence:\n  probed: '2026-08-06'\n  results:\n  - url: https://levacares.com/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://levacares.com/.well-known/oauth-protected-resource\n    http_status: 200\n  - url: https://levacares.com/wp-json/\n    http_status: 200\n  - url: https://axenahealth.com/wp-json/\n    http_status: 200\n  - url: https://levacares.com/wp-json/mcp/mcp-oauth-server\n\
  \    http_status: 401\n  - url: https://axenahealth.com/.well-known/openid-configuration\n    http_status: 404\n  - url: https://levacares.com/.well-known/openid-configuration\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axena-health/refs/heads/main/authentication/axena-health-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Health
- Digital Health
- Medical Devices
- Women's Health
- Digital Therapeutics
- Pelvic Health
- Medical Software
- Telehealth
---
