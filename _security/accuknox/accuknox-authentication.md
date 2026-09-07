---
anonymous_access: false
api_key_in:
- header
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Accuknox Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AccuKnox secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AccuKnox
provider_slug: accuknox
scheme_count: 3
schemes:
- description: AccuKnox API token. Created in the console under Settings -> Tokens with a name and an operator-chosen expiration; shown once at creation and never again. Used for cron-job deployments and integrations (KIEM, Kubernetes CIS Benchmark, cluster misconfiguration).
  format: 'Authorization: Bearer <token>'
  header: Authorization
  name: apiToken
  scheme: bearer
  sources:
  - https://help.accuknox.com/how-to/how-to-create-tokens/
  - https://github.com/accuknox/mcp_server/blob/main/shared/api.py
  type: http
- description: Access keys, a separate credential class used to onboard clusters and virtual machines to a tenant rather than to call the platform API directly.
  name: accessKey
  scheme: bearer
  sources:
  - https://help.accuknox.com/how-to/create-access-keys/
  - https://help.accuknox.com/how-to/cluster-onboarding-access-keys/
  - https://help.accuknox.com/how-to/vm-onboard-access-keys/
  type: http
- description: OAuth 2.0 for third-party applications. Developers register an OAuth application with AccuKnox, supplying redirect URIs, and receive a client id and client secret. Short-lived access tokens plus long-lived refresh tokens.
  flows:
  - authorizationUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/authorize/
    flow: authorizationCode
    note: No scope vocabulary is published. AccuKnox documents authorization as role-based on the user profile rather than scope-based on the token. See scopes/accuknox-scopes.yml.
    scopes: {}
    tokenUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/token/
  name: oauth2
  sources:
  - https://help.accuknox.com/integrations/oauth/
  type: oauth2
slug: accuknox-authentication
source_filename: accuknox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://help.accuknox.com/integrations/oauth/\ndocs: https://help.accuknox.com/how-to/how-to-create-tokens/\nnote: >-\n  Derived mechanically from OpenAPI is not possible here — AccuKnox publishes no\n  machine-readable contract (its Swagger UI at /api/swagger/ redirects to a Django admin\n  login). This profile is assembled from AccuKnox's own documentation and from its\n  first-party MCP server source, plus one anonymous live probe of the JWKS endpoint.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  token_signing: RS256\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  description: >-\n    AccuKnox API token. Created in the console under Settings -> Tokens with a name and an\n    operator-chosen expiration; shown once at creation and never again. Used for cron-job\n\
  \    deployments and integrations (KIEM, Kubernetes CIS Benchmark, cluster misconfiguration).\n  sources:\n  - https://help.accuknox.com/how-to/how-to-create-tokens/\n  - https://github.com/accuknox/mcp_server/blob/main/shared/api.py\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: >-\n    Access keys, a separate credential class used to onboard clusters and virtual machines\n    to a tenant rather than to call the platform API directly.\n  sources:\n  - https://help.accuknox.com/how-to/create-access-keys/\n  - https://help.accuknox.com/how-to/cluster-onboarding-access-keys/\n  - https://help.accuknox.com/how-to/vm-onboard-access-keys/\n- name: oauth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 for third-party applications. Developers register an OAuth application with\n    AccuKnox, supplying redirect URIs, and receive a client id and client secret.\n    Short-lived access tokens plus long-lived refresh tokens.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://cspm.<tenant>.accuknox.com/api/v1/o/authorize/\n    tokenUrl: https://cspm.<tenant>.accuknox.com/api/v1/o/token/\n    scopes: {}\n    note: >-\n      No scope vocabulary is published. AccuKnox documents authorization as role-based on\n      the user profile rather than scope-based on the token. See scopes/accuknox-scopes.yml.\n  sources:\n  - https://help.accuknox.com/integrations/oauth/\njwks:\n  url: https://cspm.<tenant>.accuknox.com/api/v1/jwks/\n  algorithm: RS256\n  key_type: RSA\n  anonymous: true\n  probed:\n  - {url: 'https://cspm.accuknox.com/api/v1/jwks/', status: 200, content_type: application/json}\n  - {url: 'https://cspm.demo.accuknox.com/api/v1/jwks/', status: 200, content_type: application/json}\n  - {url: 'https://cspm.dev.accuknox.com/api/v1/jwks/', status: 200, content_type: application/json}\n  note: >-\n    Each tenant host publishes its own RSA signing key set anonymously. AccuKnox's own MCP\n    server verifies inbound JWTs against this endpoint (shared/utils/auth_validator.py),\n\
  \    so it is the documented verification surface for the platform's tokens.\nunauthenticated_behaviour:\n  probed_url: https://cspm.accuknox.com/api/v1/assets\n  status: 403\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  note: Django REST Framework default — 403, not 401, and no WWW-Authenticate challenge.\ntenancy:\n  pattern: https://cspm.<tenant>.accuknox.com\n  observed: [cspm.accuknox.com, cspm.demo.accuknox.com, cspm.dev.accuknox.com]\n  note: >-\n    The API host is per tenant. AccuKnox's own MCP server takes the host as the\n    ACCUKNOX_BASE_URL environment variable rather than hard-coding one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accuknox/refs/heads/main/authentication/accuknox-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Security
- Cloud Security
- Cloud Native Application Protection Platform
- Kubernetes Security
- Runtime Security
- Zero Trust
- DevSecOps
- Compliance
- AI Security
- Vulnerability Management
- Container Security
---
