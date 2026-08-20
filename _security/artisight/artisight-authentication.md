---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Artisight Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Artisight secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Artisight
provider_slug: artisight
scheme_count: 2
schemes:
- applies_to:
  - https://artisight.com/wp-json/mcp/mcp-oauth-server
  - https://artisight.com/wp-json/wp-abilities/v1
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  flows:
  - authorizationUrl: https://artisight.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://artisight.com/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://artisight.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://artisight.com
  name: mcp-oauth
  response_types_supported:
  - code
  source: well-known/artisight-oauth-authorization-server.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to:
  - https://artisight.com/wp-json/
  authorization_endpoint: https://artisight.com/wp-admin/authorize-application.php
  name: application-passwords
  note: WordPress Application Passwords, advertised in the /wp-json/ index authentication block. Applies to authenticated WordPress REST API calls.
  scheme: basic
  source: well-known/artisight-wp-json-index.json
  type: http
slug: artisight-authentication
source_filename: artisight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://artisight.com/.well-known/oauth-authorization-server\ndocs: https://artisight.com/wp-json/\nnote: Artisight publishes no developer authentication documentation. This profile is\n  assembled from live, anonymous discovery documents on artisight.com — RFC 8414 authorization-server\n  metadata, RFC 9728 protected-resource metadata, and the WordPress REST route index.\n  The derive-authentication.py pass produced nothing because the repo holds no OpenAPI.\nsummary:\n  types: [oauth2, http]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  public_client: true\n  pkce: [S256]\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  source: well-known/artisight-oauth-authorization-server.json\n  issuer: https://artisight.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://artisight.com/oauth/authorize\n    tokenUrl: https://artisight.com/oauth/token\n    revocationUrl: https://artisight.com/oauth/revoke\n\
  \    scopes: [mcp]\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_id_metadata_document_supported: true\n  applies_to:\n  - https://artisight.com/wp-json/mcp/mcp-oauth-server\n  - https://artisight.com/wp-json/wp-abilities/v1\n- name: application-passwords\n  type: http\n  scheme: basic\n  source: well-known/artisight-wp-json-index.json\n  authorization_endpoint: https://artisight.com/wp-admin/authorize-application.php\n  note: WordPress Application Passwords, advertised in the /wp-json/ index authentication\n    block. Applies to authenticated WordPress REST API calls.\n  applies_to:\n  - https://artisight.com/wp-json/\nanonymous_access:\n  supported: true\n  note: Most wp/v2 read routes (posts, pages, media, taxonomies) are readable without\n    credentials. The mcp and wp-abilities/v1 namespaces are not.\nnot_published:\n  product_api_auth:\
  \ Artisight documents no authentication model for the Smart Hospital\n    Platform; EHR integration is delivered as a native Epic/Cerner interface, not a\n    developer-facing API.\nx-evidence:\n- fetched: '2026-08-02'\n  url: https://artisight.com/.well-known/oauth-authorization-server\n  http_status: 200\n- fetched: '2026-08-02'\n  url: https://artisight.com/wp-json/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artisight/refs/heads/main/authentication/artisight-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Healthcare
- Artificial Intelligence
- Computer-Vision
- Hospitals
- Ambient Intelligence
- Electronic Health Records
- Machine-Learning
- Patient Monitoring
- Internet of Things
---
