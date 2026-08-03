---
api_key_in: []
api_specs:
- filename: engrail-therapeutics-content-openapi.yml
  format: yaml
  label: Engrail Therapeutics Site Content API
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engrail-therapeutics/refs/heads/main/openapi/engrail-therapeutics-content-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Engrail Therapeutics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Engrail Therapeutics secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Engrail Therapeutics
provider_slug: engrail-therapeutics
scheme_count: 2
schemes:
- authorization_endpoint: https://www.engrail.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, advertised by the site's own REST index (authentication.application-passwords.endpoints.authorization). Required for write operations and non-public collections such as /wp/v2/users, which returns 401 anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/engrail-therapeutics-content-openapi.yml
  - https://www.engrail.com/wp-json/
  surface: content-api
  type: http
- bearer_methods_supported:
  - header
  client_id_metadata_document_supported: true
  code_challenge_methods_supported:
  - S256
  description: OAuth 2.1 authorization server protecting the site's MCP endpoints. Public clients only — token_endpoint_auth_methods_supported is ["none"] — with PKCE S256 mandatory and client identity supplied by a client-id metadata document rather than pre-registration.
  flows:
  - authorizationUrl: https://www.engrail.com/oauth/authorize
    flow: authorizationCode
    revocationUrl: https://www.engrail.com/oauth/revoke
    scopes:
      mcp: Access the site's Model Context Protocol servers.
    tokenUrl: https://www.engrail.com/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://www.engrail.com
  name: mcpOAuth
  protected_resource: https://www.engrail.com/wp-json/mcp/mcp-oauth-server
  response_types_supported:
  - code
  sources:
  - well-known/engrail-therapeutics-oauth-authorization-server.json
  - well-known/engrail-therapeutics-oauth-protected-resource.json
  surface: mcp
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
slug: engrail-therapeutics-authentication
source_filename: engrail-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: https://www.engrail.com/.well-known/oauth-authorization-server\ndocs: https://www.engrail.com/wp-json/\nnote: >-\n  Upgraded from the mechanical OpenAPI derivation (which saw only the WordPress Application Password\n  scheme) with the live RFC 8414 / RFC 9728 discovery documents served at the apex. Engrail runs two\n  distinct auth models on one host: HTTP Basic Application Passwords for the WordPress REST content\n  API, and a full OAuth 2.1 authorization-code + PKCE flow that exists solely to authorize its Model\n  Context Protocol servers.\nsummary:\n  types:\n  - http\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  anonymous_read: true\n  anonymous_read_note: >-\n    The 16 content operations in openapi/engrail-therapeutics-content-openapi.yml were each verified\n    to return HTTP 200 without credentials on 2026-08-01.\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  surface:\
  \ content-api\n  description: >-\n    WordPress Application Passwords, advertised by the site's own REST index\n    (authentication.application-passwords.endpoints.authorization). Required for write operations and\n    non-public collections such as /wp/v2/users, which returns 401 anonymously.\n  authorization_endpoint: https://www.engrail.com/wp-admin/authorize-application.php\n  sources:\n  - openapi/engrail-therapeutics-content-openapi.yml\n  - https://www.engrail.com/wp-json/\n- name: mcpOAuth\n  type: oauth2\n  surface: mcp\n  description: >-\n    OAuth 2.1 authorization server protecting the site's MCP endpoints. Public clients only —\n    token_endpoint_auth_methods_supported is [\"none\"] — with PKCE S256 mandatory and client identity\n    supplied by a client-id metadata document rather than pre-registration.\n  issuer: https://www.engrail.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.engrail.com/oauth/authorize\n    tokenUrl: https://www.engrail.com/oauth/token\n\
  \    revocationUrl: https://www.engrail.com/oauth/revoke\n    scopes:\n      mcp: Access the site's Model Context Protocol servers.\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  response_types_supported:\n  - code\n  code_challenge_methods_supported:\n  - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  client_id_metadata_document_supported: true\n  bearer_methods_supported:\n  - header\n  protected_resource: https://www.engrail.com/wp-json/mcp/mcp-oauth-server\n  sources:\n  - well-known/engrail-therapeutics-oauth-authorization-server.json\n  - well-known/engrail-therapeutics-oauth-protected-resource.json\nx-evidence:\n  fetched: '2026-08-01'\n  probes:\n  - url: https://www.engrail.com/.well-known/oauth-authorization-server\n    http_status: 200\n    content_type: application/json\n  - url: https://www.engrail.com/.well-known/oauth-protected-resource\n    http_status: 200\n    content_type: application/json\n  - url: https://www.engrail.com/wp-json/\n\
  \    http_status: 200\n    content_type: application/json\n  - url: https://www.engrail.com/wp-json/wp/v2/users\n    http_status: 401\n    note: Anonymous read denied — confirms the gated half of the surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engrail-therapeutics/refs/heads/main/authentication/engrail-therapeutics-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Neuroscience
- Clinical Trials
- Drug Development
- Healthcare
- Mental Health
- Model Context Protocol
---
