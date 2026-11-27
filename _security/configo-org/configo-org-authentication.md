---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Configo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Configo secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Configo
provider_slug: configo-org
scheme_count: 2
schemes:
- docs: https://configo.org/docs/dev/authentication
  dynamic_client_registration:
    endpoint: https://configo.org/oauth/register
    note: Always public clients; only projects, materials and configurators scopes can be requested.
    standard: RFC 7591
  flows:
    authorizationCode:
      authorizationUrl: https://configo.org/oauth/authorize
      refreshUrl: https://configo.org/api/auth/token
      revocationUrl: https://configo.org/api/auth/token/revoke
      scopes:
      - identify
      - billing
      - files
      - projects
      - members
      - orders
      - clients
      - tasks
      - reports
      - materials
      - configurators
      - products
      - warehouses
      - wiki
      - documents
      - email_templates
      - automations
      tokenUrl: https://configo.org/api/auth/token
  grants:
  - authorization_code
  - refresh_token
  header: 'Authorization: Bearer <access_token>'
  metadata: https://configo.org/.well-known/oauth-authorization-server
  name: oauth2
  pkce: S256 only; required for public clients, recommended for everyone else
  token_lifetimes:
    access_token: 2 hours
    authorization_code: 5 minutes, single use
    refresh_token: 30 days, single use (rotates)
  type: oauth2
  unsupported_grants: There are no client credentials, password or implicit grants.
- description: Project-specific widget token (JWT) for /api/v1/widget endpoints, intended for embedding Configo on a public-facing website.
  docs: https://configo.org/docs/dev/widget
  header: X-Widget-Token
  in: header
  name: widgetToken
  type: apiKey
slug: configo-org-authentication
source_filename: configo-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://configo.org/docs/dev/authentication\n- https://configo.org/docs/dev/reference\ndocs: https://configo.org/docs/dev/authentication\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  note: OAuth 2.0 authorization code (+PKCE) bearer tokens for the REST API; a separate project-specific widget JWT in X-Widget-Token\n    for /api/v1/widget. No OpenAPI is published; profile read from the docs.\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://configo.org/oauth/authorize\n      tokenUrl: https://configo.org/api/auth/token\n      refreshUrl: https://configo.org/api/auth/token\n      revocationUrl: https://configo.org/api/auth/token/revoke\n      scopes:\n      - identify\n      - billing\n      - files\n      - projects\n      - members\n      - orders\n      - clients\n      - tasks\n      - reports\n      - materials\n      - configurators\n      - products\n      -\
  \ warehouses\n      - wiki\n      - documents\n      - email_templates\n      - automations\n  pkce: S256 only; required for public clients, recommended for everyone else\n  grants:\n  - authorization_code\n  - refresh_token\n  unsupported_grants: There are no client credentials, password or implicit grants.\n  token_lifetimes:\n    authorization_code: 5 minutes, single use\n    access_token: 2 hours\n    refresh_token: 30 days, single use (rotates)\n  dynamic_client_registration:\n    endpoint: https://configo.org/oauth/register\n    standard: RFC 7591\n    note: Always public clients; only projects, materials and configurators scopes can be requested.\n  metadata: https://configo.org/.well-known/oauth-authorization-server\n  header: 'Authorization: Bearer <access_token>'\n  docs: https://configo.org/docs/dev/authentication\n- name: widgetToken\n  type: apiKey\n  in: header\n  header: X-Widget-Token\n  description: Project-specific widget token (JWT) for /api/v1/widget endpoints, intended\
  \ for embedding Configo on a public-facing\n    website.\n  docs: https://configo.org/docs/dev/widget\n"
source_yaml_url: https://artifacts.apis.io/configo-org/authentication/configo-org-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- CPQ
- Product Configurator
- Manufacturing
- Pricing
- CRM
- Inventory
- MCP
---
