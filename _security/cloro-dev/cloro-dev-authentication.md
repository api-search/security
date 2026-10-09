---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloro-dev-async-api-openapi.yml
  format: yaml
  label: cloro Async API
  slug: cloro-dev-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-async-api-openapi.yml
- filename: cloro-dev-countries-api-openapi.yml
  format: yaml
  label: cloro Countries API
  slug: cloro-dev-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-countries-api-openapi.yml
- filename: cloro-dev-credits-api-openapi.yml
  format: yaml
  label: cloro Credits API
  slug: cloro-dev-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-credits-api-openapi.yml
- filename: cloro-dev-monitor-api-openapi.yml
  format: yaml
  label: cloro Monitor API
  slug: cloro-dev-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-monitor-api-openapi.yml
- filename: cloro-dev-states-api-openapi.yml
  format: yaml
  label: cloro States API
  slug: cloro-dev-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/openapi/cloro-dev-states-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cloro Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: cloro secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: cloro
provider_slug: cloro-dev
scheme_count: 2
schemes:
- applies_to: REST API (https://api.cloro.dev) and the MCP server when used with an API key
  description: cloro API key as a bearer token. One key grants every endpoint in this spec; per-key scopes are not available, so a client cannot request a narrower permission. Keys are created and revoked in the [dashboard](https://dashboard.cloro.dev/api-keys).
  errors:
    codes:
    - MISSING_API_KEY
    - INVALID_API_KEY_FORMAT
    - INVALID_OR_EXPIRED_API_KEY
    note: a lowercase "bearer" prefix counts as no key
    status: 401
  header: 'Authorization: Bearer <key>'
  key_management:
    create: https://dashboard.cloro.dev/api-keys
    naming: optional human-readable name up to 64 characters
    rotation: No rotate action - create a new key and invalidate the old one; an invalidated key can keep working for up to a minute.
    shown_once: true
    test_keys: There are no separate test keys or sandbox - every key calls the production API and draws from the organization's single credit balance.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloro-dev-openapi.yml
  - https://cloro.dev/docs/guides/authentication
  type: http
- applies_to: MCP server only (https://mcp.cloro.dev/mcp)
  description: OAuth 2.1 authorization-code flow with PKCE (S256) against https://clerk.cloro.dev, advertised through RFC 9728 protected-resource metadata at https://mcp.cloro.dev/.well-known/oauth-protected-resource; the MCP server verifies tokens against the issuer's JWKS. In Claude the user signs in in the browser and selects the organization whose credits pay for the calls; no API key is pasted.
  flows:
    authorizationCode:
      authorizationUrl: https://clerk.cloro.dev/oauth/authorize
      refreshUrl: https://clerk.cloro.dev/oauth/token
      scopes:
        email: user email claims
        profile: user profile claims
        user:org:read: organization membership used for billing
      tokenUrl: https://clerk.cloro.dev/oauth/token
    deviceCode:
      deviceAuthorizationUrl: https://clerk.cloro.dev/oauth/device_authorization
      tokenUrl: https://clerk.cloro.dev/oauth/token
  name: mcpOAuth
  pkce: S256
  sources:
  - https://cloro.dev/docs/integrations/mcp
  - https://mcp.cloro.dev/.well-known/oauth-protected-resource
  - https://clerk.cloro.dev/.well-known/oauth-authorization-server
  type: oauth2
slug: cloro-dev-authentication
source_filename: cloro-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: openapi/cloro-dev-openapi.yml (securitySchemes.bearerAuth); https://cloro.dev/docs/guides/authentication (markdown twin read 2026-10-07); https://cloro.dev/docs/integrations/mcp; https://mcp.cloro.dev/.well-known/oauth-protected-resource (HTTP 200)\ndocs: https://cloro.dev/docs/guides/authentication\nsummary:\n  types:\n  - http\n  - oauth2\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  applies_to: REST API (https://api.cloro.dev) and the MCP server when used with an API key\n  description: cloro API key as a bearer token. One key grants every endpoint in this spec; per-key scopes are not available, so a client cannot request a narrower permission. Keys are created and revoked in the [dashboard](https://dashboard.cloro.dev/api-keys).\n  header: 'Authorization: Bearer <key>'\n  key_management:\n    create: https://dashboard.cloro.dev/api-keys\n    shown_once: true\n    naming: optional human-readable name up\
  \ to 64 characters\n    rotation: No rotate action - create a new key and invalidate the old one; an invalidated key can keep working for up to a minute.\n    test_keys: There are no separate test keys or sandbox - every key calls the production API and draws from the organization's single credit balance.\n  errors:\n    status: 401\n    codes: [MISSING_API_KEY, INVALID_API_KEY_FORMAT, INVALID_OR_EXPIRED_API_KEY]\n    note: a lowercase \"bearer\" prefix counts as no key\n  sources:\n  - openapi/cloro-dev-openapi.yml\n  - https://cloro.dev/docs/guides/authentication\n- name: mcpOAuth\n  type: oauth2\n  applies_to: MCP server only (https://mcp.cloro.dev/mcp)\n  description: OAuth 2.1 authorization-code flow with PKCE (S256) against https://clerk.cloro.dev, advertised through RFC 9728 protected-resource metadata at https://mcp.cloro.dev/.well-known/oauth-protected-resource; the MCP server verifies tokens against the issuer's JWKS. In Claude the user signs in in the browser and selects the\
  \ organization whose credits pay for the calls; no API key is pasted.\n  flows:\n    authorizationCode:\n      authorizationUrl: https://clerk.cloro.dev/oauth/authorize\n      tokenUrl: https://clerk.cloro.dev/oauth/token\n      refreshUrl: https://clerk.cloro.dev/oauth/token\n      scopes:\n        profile: user profile claims\n        email: user email claims\n        user:org:read: organization membership used for billing\n    deviceCode:\n      deviceAuthorizationUrl: https://clerk.cloro.dev/oauth/device_authorization\n      tokenUrl: https://clerk.cloro.dev/oauth/token\n  pkce: S256\n  sources:\n  - https://cloro.dev/docs/integrations/mcp\n  - https://mcp.cloro.dev/.well-known/oauth-protected-resource\n  - https://clerk.cloro.dev/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloro-dev/refs/heads/main/authentication/cloro-dev-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Search
- AI
- Web Scraping
- SERP
- Generative Engine Optimization
- SEO
- Brand Monitoring
- Market Research
- Data Extraction
- MCP
---
