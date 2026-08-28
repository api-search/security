---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Restor3D Authentication
name_suffix: Authentication
oauth_flows: []
overview: restor3d declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: restor3d
provider_slug: restor3d
scheme_count: 3
schemes:
- applies_to: https://www.restor3d.com/wp-json/mcp/mcp-oauth-server
  authorization_endpoint: https://www.restor3d.com/oauth/authorize
  bearer_methods_supported:
  - header
  client_registration: client_id_metadata_document_supported = true - clients are identified by a URL that resolves to a client metadata document (the emerging CIMD pattern) rather than by pre-registration.
  flow: authorization_code
  grant_types_supported:
  - authorization_code
  - refresh_token
  id: oauth2_mcp
  issuer: https://www.restor3d.com
  pkce:
    required_methods:
    - S256
  response_types_supported:
  - code
  revocation_endpoint: https://www.restor3d.com/oauth/revoke
  scopes:
  - mcp
  token_endpoint: https://www.restor3d.com/oauth/token
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- applies_to: https://www.restor3d.com/wp-json/wp/v2/*
  id: application_passwords
  note: WordPress Application Passwords are advertised in the REST index at https://www.restor3d.com/wp-json/ with authorization endpoint https://www.restor3d.com/wp-admin/authorize-application.php. Issuance requires an existing WordPress account on the site; there is no public sign-up.
  scheme: basic
  type: http
- applies_to: public GET routes under https://www.restor3d.com/wp-json/wp/v2/
  id: anonymous
  note: Read access to published content types (pages, posts, event, resource, procedure, product-family, product-category, asset-type, content-type, module) is unauthenticated.
  type: none
slug: restor3d-authentication
source_filename: restor3d-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://www.restor3d.com/.well-known/oauth-authorization-server (HTTP 200),\n  https://www.restor3d.com/.well-known/oauth-protected-resource (HTTP 200) and the\n  `authentication` block of https://www.restor3d.com/wp-json/ (HTTP 200), all fetched 2026-08-26.\n  Derived from no OpenAPI - restor3d publishes none.\napi: restor3d Website Content API (WordPress REST + MCP)\nsummary: >-\n  restor3d publishes no developer authentication documentation of any kind. Everything below was\n  read off machine-readable metadata its website serves, not off a docs page. Anonymous read\n  access is available on the public WordPress REST content routes; every write route and both MCP\n  servers are gated.\nschemes:\n- id: oauth2_mcp\n  type: oauth2\n  flow: authorization_code\n  applies_to: https://www.restor3d.com/wp-json/mcp/mcp-oauth-server\n  issuer: https://www.restor3d.com\n  authorization_endpoint: https://www.restor3d.com/oauth/authorize\n\
  \  token_endpoint: https://www.restor3d.com/oauth/token\n  revocation_endpoint: https://www.restor3d.com/oauth/revoke\n  response_types_supported:\n  - code\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  pkce:\n    required_methods:\n    - S256\n  token_endpoint_auth_methods_supported:\n  - none\n  client_registration: >-\n    client_id_metadata_document_supported = true - clients are identified by a URL that resolves\n    to a client metadata document (the emerging CIMD pattern) rather than by pre-registration.\n  scopes:\n  - mcp\n  bearer_methods_supported:\n  - header\n- id: application_passwords\n  type: http\n  scheme: basic\n  applies_to: https://www.restor3d.com/wp-json/wp/v2/*\n  note: >-\n    WordPress Application Passwords are advertised in the REST index at\n    https://www.restor3d.com/wp-json/ with authorization endpoint\n    https://www.restor3d.com/wp-admin/authorize-application.php. Issuance requires an existing\n    WordPress account on the site;\
  \ there is no public sign-up.\n- id: anonymous\n  type: none\n  applies_to: public GET routes under https://www.restor3d.com/wp-json/wp/v2/\n  note: >-\n    Read access to published content types (pages, posts, event, resource, procedure,\n    product-family, product-category, asset-type, content-type, module) is unauthenticated.\ngaps:\n- No authentication documentation is published anywhere on restor3d.com.\n- No API key programme, no developer sign-up, no partner credential flow.\n- No OpenID Connect - /.well-known/openid-configuration returns 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restor3d/refs/heads/main/authentication/restor3d-authentication.yml
summary_line: 3 schemes
tags:
- Medical Devices
- Health
- Orthopedics
- 3D Printing
- Additive Manufacturing
- Implants
- Surgery
- Artificial Intelligence
- Manufacturing
- Company
---
