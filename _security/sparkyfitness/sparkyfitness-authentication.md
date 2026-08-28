---
api_key_in: []
api_specs:
- filename: sparkyfitness-openapi.yml
  format: yaml
  label: SparkyFitness API
  slug: sparkyfitness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sparkyfitness/refs/heads/main/openapi/sparkyfitness-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sparkyfitness Authentication
name_suffix: Authentication
oauth_flows: []
overview: SparkyFitness declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: SparkyFitness
provider_slug: sparkyfitness
scheme_count: 0
schemes: []
slug: sparkyfitness-authentication
source_filename: sparkyfitness-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://codewithcj.github.io/SparkyFitness/developer/api-reference\nspec: openapi/sparkyfitness-openapi.yml\nsummary: >-\n  Three credential types reach the API, and the published contract only declares\n  one of them. API keys (x-api-key header, or Authorization: Bearer) are the\n  machine credential and the only one usable by an agent. Browser sessions use\n  an HTTP-only cookie named \"token\". End-user login can additionally be federated\n  through OIDC to an operator-configured identity provider.\nsecurity_schemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    declared_in_spec: true\n    applied_to_operations: 279\n    is_global_default: true\n    description: >-\n      API key authentication via the x-api-key header. Keys are created in the\n      web UI under Settings -> Developer & Integrations -> API Key Management.\n      The API reference states the same key is also accepted\
  \ as\n      \"Authorization: Bearer <API_KEY>\", and the MCP docs use only the Bearer\n      form — so the header the spec declares is not the only one the server takes.\n  - name: cookieAuth\n    type: apiKey\n    in: cookie\n    parameter: token\n    declared_in_spec: false\n    description: >-\n      A secure, HTTP-only cookie named \"token\" carrying the session JWT. It IS\n      defined in the project's swagger source (config/swagger.ts) and then\n      deliberately STRIPPED before the spec is served: a post-processing step\n      deletes cookieAuth from components.securitySchemes and rewrites every\n      operation that required it to require apiKeyAuth instead, so Swagger UI\n      offers the key rather than a cookie the browser sets. The published\n      contract therefore understates the real auth surface by one scheme.\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    declared_in_spec: false\n    applied_to_operations: 15\n    defect: true\n    description: >-\n\
  \      Fifteen operations declare `security: [{bearerAuth: []}]` but bearerAuth\n      is never defined under components.securitySchemes. This is a real dangling\n      reference in the contract: a generator or validator will fail or silently\n      drop auth on those fifteen operations. Semantically it is the JWT the API\n      reference describes (\"Authorization: Bearer <JWT_TOKEN>\").\npermissions:\n  model: per-key permission strings, not OAuth scopes\n  examples:\n    - name: health_data_write\n      required_by: POST /health-data\n      failure: '403 — Forbidden: API Key does not have health_data_write permission'\n  note: >-\n    Permissions are attached to an API key at creation time in the UI. They are\n    NOT OAuth scopes, are not enumerated in the spec, and there is no\n    machine-readable permission catalogue — which is why no scopes/ artifact is\n    emitted for this provider.\nrow_level_security:\n  enabled: true\n  description: >-\n    Data access is enforced in PostgreSQL\
  \ with Row Level Security, scoped to the\n    user the API key authenticates. The MCP path deliberately scopes to\n    authenticatedUserId rather than the delegation cookie, so family-sharing\n    delegation cannot make an agent act as another user.\n  exception: >-\n    Five admin developer tools run on the owner pool and bypass RLS. They require\n    both DEV_TOOLS_ENABLED=true and an admin caller, and are gated at\n    registration so they never appear in a non-admin tools/list.\nfederated_identity:\n  protocol: OpenID Connect\n  library: openid-client\n  docs: https://codewithcj.github.io/SparkyFitness/administration/oauth-authentication\n  multiple_providers: true\n  scope: openid profile email\n  discovery: >-\n    The operator supplies an Issuer URL and SparkyFitness discovers the IdP\n    configuration from it. SparkyFitness is the OIDC RELYING PARTY here, not a\n    provider — it publishes no /.well-known/openid-configuration of its own.\n  configurable:\n    - Issuer URL\n  \
  \  - Client ID\n    - Client Secret\n    - Redirect URI\n    - Auto-register users\n    - Token endpoint auth method\n    - ID token signed response algorithm\n    - Userinfo signed response algorithm\n    - Request timeout (default 3500 ms)\n  admin_api: /admin/oidc-settings (GET, POST, PUT, DELETE)\nmfa:\n  supported: true\n  evidence: >-\n    /api/auth/mfa/* endpoints are rate-limited by name in the nginx config, and\n    an admin operation exists to reset a user's MFA\n    (POST /admin/auth/users/{userId}/mfa/reset) and to make MFA mandatory\n    (/admin/auth/settings/mfa-mandatory).\npasskeys:\n  supported: true\n  evidence: >-\n    SparkyFitnessServer/routes/auth/templates/passkey-login.html and\n    passkey-register.html ship with a bundled @simplewebauthn/browser build.\nagent_guidance: >-\n  An agent should use an API key. Generate it in the UI, send it as\n  \"Authorization: Bearer <key>\" (works for both REST and MCP) or as x-api-key,\n  and expect 401 for a missing/invalid\
  \ key and 403 when the key lacks the\n  required permission.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sparkyfitness/refs/heads/main/authentication/sparkyfitness-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Health
- Fitness
- Nutrition
- Self-Hosted
- Open Source
- Wearables
- MCP
- AI Assistant
- Quantified Self
---
