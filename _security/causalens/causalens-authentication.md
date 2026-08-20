---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Causalens Authentication
name_suffix: Authentication
oauth_flows: []
overview: CausaLens declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CausaLens
provider_slug: causalens
scheme_count: 0
schemes: []
slug: causalens-authentication
source_filename: causalens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://dara.causalens.com/docs/generated/dara/reference/dara/core/auth/routes\ndocs:\n- https://dara.causalens.com/docs/generated/dara/reference/dara/core/auth/base\n- https://dara.causalens.com/docs/generated/dara/reference/dara/core/auth/basic\n- https://dara.causalens.com/docs/generated/dara/reference/dara/core/auth/definitions\n- https://dara.causalens.com/docs/generated/dara/reference/dara/core/auth/routes\n- https://dara.causalens.com/docs/generated/dara/docs/advanced/custom-endpoints\nscope: 'Dara open-source application framework. The commercial decisionOS platform''s\n  auth model is documented only behind the login wall at docs.causalens.com and is\n  therefore NOT described here.'\nsummary: 'Dara applications authenticate with a bearer JWT session token carried in\n  the HTTP Authorization header, paired with a cookie-borne refresh token. Endpoints\n  registered through the dara.core.http decorators are authenticated\
  \ by default\n  (authenticated=True), which attaches the framework security dependency; setting\n  authenticated=False opts an endpoint out. Dara ships pluggable auth backends,\n  including a basic username/password configuration and an OIDC integration.'\nsecurity_schemes:\n- id: sessionToken\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  description: 'Session JWT verified by the /verify-session route. Extracted with\n    FastAPI HTTPBearer; HTTPBearer(auto_error=False) is used where the credential is\n    optional and HTTPBearer() where it is mandatory.'\n  default: true\n- id: refreshToken\n  type: apiKey\n  in: cookie\n  description: 'Refresh token supplied as a cookie to the /refresh-token route, which\n    returns a new session token plus a new refresh-token cookie.'\n- id: oidc\n  type: openIdConnect\n  description: 'Dara supports OIDC-backed authentication; the changelog records\n    OpenTelemetry instrumentation covering \"authentication\
  \ and OIDC\" as a first-class\n    code path.'\n  evidence: https://raw.githubusercontent.com/causalens/dara/master/packages/dara-core/changelog.md\n- id: basic\n  type: http\n  scheme: basic\n  description: 'BasicAuth configuration for local/simple deployments (dara.core.auth.basic).'\n  evidence: https://dara.causalens.com/docs/generated/dara/reference/dara/core/auth/basic\nroutes:\n- path: /verify-session\n  method: POST\n  description: Verify that the request carries a valid session JWT. Designed to be\n    applied as a FastAPI dependency on routes that require a session.\n- path: /refresh-token\n  method: POST\n  description: Exchange a refresh-token cookie for a new session token and a new\n    refresh-token cookie.\ncontext_accessors:\n- name: USER\n  import: from dara.core.auth import USER\n  description: Current authenticated user; None on unsecured endpoints.\n- name: SESSION\n  import: from dara.core.auth import SESSION\n  description: Current session id; None on unsecured endpoints.\n\
  signing:\n  secret_env: JWT_SECRET\n  notes: 'Production and Docker deployments are documented as needing JWT_SECRET set.\n    Local development reuses a generated development signing key from the user cache\n    when no secret is set. Session storage is configurable via config.auth_session_backend\n    with InMemoryAuthSessionBackend (default) and FileAuthSessionBackend built in.'\n  evidence: https://raw.githubusercontent.com/causalens/dara/master/packages/dara-core/changelog.md\noauth_scopes: none\nnotes: 'No OAuth 2.0 authorization-server metadata is published on any causaLens host\n  (/.well-known/oauth-authorization-server returns 404 on every host that answers\n  honestly). Dara has no scope surface, so scopes/ is intentionally not emitted.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causalens/refs/heads/main/authentication/causalens-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Artificial Intelligence
- Causal AI
- Machine-Learning
- Data Science
- Decision Intelligence
- Analytics
- Agents
- Open-Source
- Python
---
