---
anonymous_access: true
api_key_in: []
auth_types:
- none
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Harbinger Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Harbinger Health secures its APIs with none, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Harbinger Health
provider_slug: harbinger-health
scheme_count: 3
schemes:
- applies_to: wp/v2 read routes in view and embed context
  description: The public content surface is readable with no credential at all. GET /wp-json/wp/v2/posts, /pages, /categories, /tags, /media, /types, /taxonomies, /users and /search all returned HTTP 200 to an unauthenticated caller on 2026-08-04.
  name: anonymous
  sources:
  - openapi/harbinger-health-wordpress-wp-v2-openapi.yml
  type: none
- authorization_endpoint: https://harbinger-health.com/wp-admin/authorize-application.php
  description: 'WordPress application password, advertised by the site''s own route-discovery document under authentication.application-passwords. Credentials are issued from https://harbinger-health.com/wp-admin/authorize-application.php and presented as ''Authorization: Basic base64(user:application-password)''. Required for edit context, for every write method, and for the routes that returned 401 anonymously (/wp/v2/settings, wp-abilities/v1/*).'
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/harbinger-health-wordpress-wp-v2-openapi.yml
  - openapi/harbinger-health-wp-json-discovery.json
  type: http
- bearer_methods_supported:
  - header
  client_registration: client-ID metadata document (client_id_metadata_document_supported true)
  description: A real OAuth 2.1 deployment on the provider's own origin, guarding the Model Context Protocol server. Discovered through RFC 8414 authorization-server metadata and RFC 9728 protected-resource metadata. Public clients with PKCE S256; bearer token presented in the Authorization header; a single mcp scope.
  flows:
  - authorizationUrl: https://harbinger-health.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    revocationUrl: https://harbinger-health.com/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://harbinger-health.com/oauth/token
  issuer: https://harbinger-health.com
  name: mcp-oauth
  protected_resource: https://harbinger-health.com/wp-json/mcp/mcp-oauth-server
  scopes_artifact: scopes/harbinger-health-scopes.yml
  sources:
  - well-known/harbinger-health-oauth-authorization-server.json
  - well-known/harbinger-health-oauth-protected-resource.json
  type: oauth2
slug: harbinger-health-authentication
source_filename: harbinger-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  https://harbinger-health.com/wp-json/ route-discovery authentication block,\n  https://harbinger-health.com/.well-known/oauth-authorization-server,\n  https://harbinger-health.com/.well-known/oauth-protected-resource, and live 401 probes on\n  2026-08-04\ndocs: null\nsummary:\n  types: [none, http, oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  anonymous_read: true\n  note: >-\n    Harbinger Health publishes no authentication documentation of any kind — there is no developer\n    portal and no docs site. The profile below is assembled entirely from the machine-readable\n    discovery documents the host serves and from observed HTTP responses.\nschemes:\n  - name: anonymous\n    type: none\n    applies_to: wp/v2 read routes in view and embed context\n    description: >-\n      The public content surface is readable with no credential at all. GET /wp-json/wp/v2/posts,\n      /pages, /categories, /tags,\
  \ /media, /types, /taxonomies, /users and /search all returned HTTP\n      200 to an unauthenticated caller on 2026-08-04.\n    sources: [openapi/harbinger-health-wordpress-wp-v2-openapi.yml]\n  - name: applicationPassword\n    type: http\n    scheme: basic\n    description: >-\n      WordPress application password, advertised by the site's own route-discovery document under\n      authentication.application-passwords. Credentials are issued from\n      https://harbinger-health.com/wp-admin/authorize-application.php and presented as\n      'Authorization: Basic base64(user:application-password)'. Required for edit context, for every\n      write method, and for the routes that returned 401 anonymously (/wp/v2/settings,\n      wp-abilities/v1/*).\n    authorization_endpoint: https://harbinger-health.com/wp-admin/authorize-application.php\n    sources:\n      - openapi/harbinger-health-wordpress-wp-v2-openapi.yml\n      - openapi/harbinger-health-wp-json-discovery.json\n  - name: mcp-oauth\n\
  \    type: oauth2\n    description: >-\n      A real OAuth 2.1 deployment on the provider's own origin, guarding the Model Context Protocol\n      server. Discovered through RFC 8414 authorization-server metadata and RFC 9728\n      protected-resource metadata. Public clients with PKCE S256; bearer token presented in the\n      Authorization header; a single mcp scope.\n    issuer: https://harbinger-health.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://harbinger-health.com/oauth/authorize\n        tokenUrl: https://harbinger-health.com/oauth/token\n        revocationUrl: https://harbinger-health.com/oauth/revoke\n        pkce: [S256]\n        scopes: [mcp]\n    bearer_methods_supported: [header]\n    client_registration: client-ID metadata document (client_id_metadata_document_supported true)\n    protected_resource: https://harbinger-health.com/wp-json/mcp/mcp-oauth-server\n    scopes_artifact: scopes/harbinger-health-scopes.yml\n    sources:\n   \
  \   - well-known/harbinger-health-oauth-authorization-server.json\n      - well-known/harbinger-health-oauth-protected-resource.json\nobserved_challenges:\n  - {url: 'https://harbinger-health.com/wp-json/mcp/mcp-oauth-server', status: 401, code: mcp_unauthorized}\n  - {url: 'https://harbinger-health.com/wp-json/mcp/mcp-adapter-default-server', status: 401, code: rest_forbidden}\n  - {url: 'https://harbinger-health.com/wp-json/wp-abilities/v1/abilities', status: 401, code: rest_forbidden}\n  - {url: 'https://harbinger-health.com/wp-json/wp/v2/settings', status: 401, code: rest_forbidden}\ntransport:\n  https_only: true\n  tls_version: TLSv1.3\n  cors_allowed_headers: [Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type]\ngaps:\n  - No OpenID Connect discovery document; no identity layer is advertised alongside the OAuth server.\n  - No mutual TLS, no API keys and no signed-request scheme anywhere on the host.\n  - No published authentication guide, key-rotation policy\
  \ or credential-lifetime statement.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbinger-health/refs/heads/main/authentication/harbinger-health-authentication.yml
summary_line: none/http/oauth2 · 3 schemes
tags:
- Health
- Healthcare
- Biotechnology
- Cancer Detection
- Diagnostics
- Genomics
- Artificial Intelligence
- Machine Learning
- Life Sciences
- Clinical Laboratory
- Precision Medicine
- United States
- Company
---
