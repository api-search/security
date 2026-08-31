---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Nextworld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nextworld declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Nextworld
provider_slug: nextworld
scheme_count: 0
schemes: []
slug: nextworld-authentication
source_filename: nextworld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.nextw.com/docs/developerstudiointeroperability\ndocs:\n- https://www.nextw.com/docs/developerstudiointeroperability\n- https://www.nextw.com/docs/mcpserver\n- https://www.nextw.com/docs/developerstudiosecurity\nname: Nextworld authentication profile\nnote: >-\n  Not derived from an OpenAPI — Nextworld publishes none. Every scheme below is stated in the\n  company's public documentation, or was observed directly on a live probe (marked probed).\nsurfaces:\n- surface: Inbound REST API (external system calling into Nextworld)\n  schemes:\n  - type: http\n    scheme: basic\n    description: >-\n      The first call an external system makes is an authentication call using Basic Authentication.\n      Nextworld states \"Nextworld supports Basic Authentication protocols\" for inbound requests.\n    method: searched\n  - type: http\n    scheme: bearer\n    bearerFormat: opaque access token\n    description: >-\n      The\
  \ authentication response is JSON and carries the tenant-specific protocol://host:port that\n      MUST be used for all subsequent calls, plus an access token and a refresh token. The access\n      token expires every 8 minutes. The refresh token lasts several hours and can be used both to\n      refresh the access token and to switch to a different environment/lifecycle.\n    method: searched\n  environment_selection: >-\n    If no environment or lifecycle is supplied in the authentication request body, the credentials\n    used derive the default environment and lifecycle, and every subsequent call stays inside it. A\n    different environment (dev/test vs production) can be named in the request body.\n  base_url_discovery: >-\n    Nextworld does not publish a fixed production base URL. The production authentication URL is\n    documented only in the in-platform Endpoint Documentation (Sidebar > Integrations), which\n    requires a tenant login. The host for data calls is returned by\
  \ the authentication response.\n- surface: Remote MCP server (agent client calling into Nextworld)\n  endpoint: https://apps.nextworld.net/ai/mcp\n  schemes:\n  - type: apiKey\n    in: query\n    name: apikey\n    description: >-\n      Per-user Personal Access Key embedded in the MCP URL that the platform generates via the\n      \"Get MCP URL\" button. Revoked in bulk from User Menu > Settings > Revoke Service Personal\n      Access Keys, which invalidates every key across the user's lifecycles, tenants and environments.\n    method: searched\n  - type: oauth2\n    description: >-\n      OAuth is documented for Claude Enterprise: the tenant ID is entered as the OAuth Client ID and\n      each user supplies their own Personal Access Key at sign-in, so actions are attributed to the\n      acting user rather than to whoever configured the connector.\n    authorization_server: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_EJas25nD4\n    scopes: ../scopes/nextworld-scopes.yml\n  \
  \  method: probed\n    evidence: >-\n      An anonymous tools/list POST to https://apps.nextworld.net/ai/mcp?app=JournalEntry returned\n      HTTP 401 with WWW-Authenticate: Bearer\n      resource_metadata=\"https://apps.nextworld.net/ai/mcp/.well-known/oauth-protected-resource\"\n      on 2026-08-26 — a conformant RFC 9728 challenge.\n- surface: Inbound webhooks (external system notifying Nextworld)\n  schemes:\n  - type: hmac\n    description: >-\n      HMAC authentication. A secret is generated in the Credential Management application and used\n      both in Webhook Setup and in the calling external system; each inbound request is authenticated\n      with the specified HMAC algorithm.\n    method: searched\n  - type: http\n    scheme: basic\n    description: Each inbound webhook request carries a username and password.\n    method: searched\n- surface: Outbound endpoints (Nextworld calling an external API)\n  note: >-\n    Configured per-endpoint in the Endpoint Definitions application.\
  \ Listed for completeness — this\n    is Nextworld acting as a CLIENT, not an authentication surface Nextworld exposes.\n  schemes:\n  - type: none\n    description: No Auth.\n  - type: http\n    scheme: basic\n    description: Basic Auth against a Key/Secret pair stored in the Endpoint Secret Setup application.\n  - type: token\n    description: A referenced Token Creation endpoint mints the token; a Token Release endpoint can end the session.\n  - type: oauth2\n    description: >-\n      OAuth 2.0 with Authorization Code, Refresh Token, and Client Credentials grants. Client\n      Credentials supports both Client Secret and JWT Assertion client authentication. PKCE is\n      automatically included in OAuth requests from the Nextworld platform.\n  - type: jwt\n    description: >-\n      JSON Web Token, configured in the Endpoint JWT Setup application. Tokens are either generated\n      in-platform with a symmetric algorithm or retrieved externally by a logic block.\n  - type: sso\n  \
  \  description: Token retrieved from the URL defined for the chosen third party; configured in Tenant Environment Setup.\n  - type: oauth2.1\n    description: >-\n      OAuth 2.1 with PKCE and, where supported, dynamic client registration — used specifically when\n      the Nextworld assistant \"Ed\" connects out to an external MCP server.\nauthorization_model:\n  description: >-\n    Beyond authentication, access is governed by the platform's own model: security groups collect\n    metadata objects, permission definitions grant RUID (read/update/insert/delete) at row, field,\n    action, application, workflow-data/transition and org-unit level, roles combine permissions, and\n    role hierarchies let roles inherit. Once a role grants access, the only way to remove it is to\n    revoke or remove the role. Security is enabled for all product families except Playpen.\n  source: https://www.nextw.com/docs/developerstudiosecurity\ngaps:\n- No published OpenAPI securitySchemes block.\n- No\
  \ public production authentication URL; it is behind the tenant login.\n- No API-key rotation policy or token-lifetime table published beyond the 8-minute access token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextworld/refs/heads/main/authentication/nextworld-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Enterprise Resource Planning
- No-Code
- Enterprise Application Platform
- Workflow-Automation
- Artificial Intelligence
- MCP
- Integration
- Manufacturing
- Distribution
---
