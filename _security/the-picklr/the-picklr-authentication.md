---
api_key_in: []
api_specs:
- filename: the-picklr-wordpress-rest-openapi.json
  format: json
  label: The Picklr WordPress REST API
  slug: the-picklr-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/openapi/the-picklr-wordpress-rest-openapi.json
auth_types: []
description: Two distinct authentication models are live on thepicklr.com, and they gate different surfaces. The wp/v2 content collections are readable with no credential at all. Writes and the MCP endpoints are gated — by WordPress Application Passwords for the classic REST routes, and by an OAuth 2.1 authorization server (dynamic registration, PKCE-only) for the MCP resource. Everything below was read from documents the site serves; nothing is inferred from vendor documentation.
kind: authentication
layout: security
method: probed
name: The Picklr Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Picklr declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: The Picklr
provider_slug: the-picklr
scheme_count: 3
schemes:
- applies_to: GET on the public wp/v2 collections (posts, pages, media, location, press, event, categories, tags, types, taxonomies, search)
  evidence:
    status: 200
    url: https://thepicklr.com/wp-json/wp/v2/posts?per_page=1
  id: anonymous
  note: No API key, token or registration is required to read the published content surface.
  type: none
  verified: probed
- applies_to: WordPress REST write operations and the non-OAuth MCP endpoints
  authorization_endpoint: https://thepicklr.com/wp-admin/authorize-application.php
  evidence:
    field: authentication.application-passwords.endpoints.authorization
    status: 200
    url: https://thepicklr.com/wp-json/
  id: application_password
  note: Advertised by the live API root document. Credentials are issued per-user from the WordPress admin; there is no self-service developer signup.
  scheme: basic
  type: http
  verified: probed
- applies_to: https://thepicklr.com/wp-json/mcp/novamira-oauth
  bearer_methods_supported:
  - header
  code_challenge_methods:
  - S256
  dynamic_client_registration: true
  endpoints:
    authorization: https://thepicklr.com/wp-admin/admin.php?page=novamira-oauth-authorize
    device_authorization: https://thepicklr.com/wp-json/novamira/v1/oauth/device
    introspection: https://thepicklr.com/wp-json/novamira/v1/oauth/introspect
    registration: https://thepicklr.com/wp-json/novamira/v1/oauth/register
    revocation: https://thepicklr.com/wp-json/novamira/v1/oauth/revoke
    token: https://thepicklr.com/wp-json/novamira/v1/oauth/token
  evidence:
    status: 200
    url: https://thepicklr.com/.well-known/oauth-authorization-server
  grant_types:
  - authorization_code
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id: oauth2
  issuer: https://thepicklr.com
  metadata: https://thepicklr.com/.well-known/oauth-authorization-server
  protected_resource_metadata: https://thepicklr.com/.well-known/oauth-protected-resource
  response_types:
  - code
  scopes:
  - mcp
  token_endpoint_auth_methods:
  - none
  type: oauth2
  verified: probed
slug: the-picklr-authentication
source_filename: the-picklr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://thepicklr.com/.well-known/oauth-authorization-server\nname: The Picklr — authentication profile\ndescription: >-\n  Two distinct authentication models are live on thepicklr.com, and they gate different\n  surfaces. The wp/v2 content collections are readable with no credential at all. Writes and\n  the MCP endpoints are gated — by WordPress Application Passwords for the classic REST\n  routes, and by an OAuth 2.1 authorization server (dynamic registration, PKCE-only) for the\n  MCP resource. Everything below was read from documents the site serves; nothing is inferred\n  from vendor documentation.\nschemes:\n- id: anonymous\n  type: none\n  applies_to: GET on the public wp/v2 collections (posts, pages, media, location, press, event, categories, tags, types, taxonomies, search)\n  verified: probed\n  evidence:\n    url: https://thepicklr.com/wp-json/wp/v2/posts?per_page=1\n    status: 200\n  note: No API key, token or registration\
  \ is required to read the published content surface.\n- id: application_password\n  type: http\n  scheme: basic\n  applies_to: WordPress REST write operations and the non-OAuth MCP endpoints\n  authorization_endpoint: https://thepicklr.com/wp-admin/authorize-application.php\n  verified: probed\n  evidence:\n    url: https://thepicklr.com/wp-json/\n    status: 200\n    field: authentication.application-passwords.endpoints.authorization\n  note: >-\n    Advertised by the live API root document. Credentials are issued per-user from the\n    WordPress admin; there is no self-service developer signup.\n- id: oauth2\n  type: oauth2\n  applies_to: https://thepicklr.com/wp-json/mcp/novamira-oauth\n  verified: probed\n  metadata: https://thepicklr.com/.well-known/oauth-authorization-server\n  protected_resource_metadata: https://thepicklr.com/.well-known/oauth-protected-resource\n  issuer: https://thepicklr.com\n  endpoints:\n    authorization: https://thepicklr.com/wp-admin/admin.php?page=novamira-oauth-authorize\n\
  \    token: https://thepicklr.com/wp-json/novamira/v1/oauth/token\n    registration: https://thepicklr.com/wp-json/novamira/v1/oauth/register\n    revocation: https://thepicklr.com/wp-json/novamira/v1/oauth/revoke\n    introspection: https://thepicklr.com/wp-json/novamira/v1/oauth/introspect\n    device_authorization: https://thepicklr.com/wp-json/novamira/v1/oauth/device\n  grant_types: [authorization_code, refresh_token, 'urn:ietf:params:oauth:grant-type:device_code']\n  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  bearer_methods_supported: [header]\n  scopes: [mcp]\n  dynamic_client_registration: true\n  evidence:\n    url: https://thepicklr.com/.well-known/oauth-authorization-server\n    status: 200\nposture:\n  public_read: true\n  self_service_signup: false\n  api_keys: false\n  mtls: false\n  pkce_required: true\n  note: >-\n    token_endpoint_auth_methods is [\"none\"] and code_challenge_methods is [\"S256\"] only —\n    a public-client,\
  \ PKCE-mandatory OAuth 2.1 profile, which is the shape the MCP\n    authorization spec expects. There is no client_secret path and no implicit grant.\ngaps:\n- No human-readable authentication documentation is published anywhere on thepicklr.com; the\n  entire auth model above had to be read out of machine metadata.\n- No developer portal, signup or key-issuance flow exists for third parties.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-picklr/refs/heads/main/authentication/the-picklr-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Sports
- Pickleball
- Fitness
- Franchising
- Recreation
- Health and Wellness
- Consumer
- Content Management
- MCP
---
