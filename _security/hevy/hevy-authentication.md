---
api_key_in: []
api_specs:
- filename: hevy-exercisehistory-api-openapi.yml
  format: yaml
  label: Hevy Exercise History API
  slug: hevy-exercisehistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-exercisehistory-api-openapi.yml
- filename: hevy-exercisetemplates-api-openapi.yml
  format: yaml
  label: Hevy Exercise Templates API
  slug: hevy-exercisetemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-exercisetemplates-api-openapi.yml
- filename: hevy-measurements-api-openapi.yml
  format: yaml
  label: Hevy Measurements API
  slug: hevy-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-measurements-api-openapi.yml
- filename: hevy-routinefolders-api-openapi.yml
  format: yaml
  label: Hevy Routine Folders API
  slug: hevy-routinefolders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-routinefolders-api-openapi.yml
- filename: hevy-routines-api-openapi.yml
  format: yaml
  label: Hevy Routines API
  slug: hevy-routines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-routines-api-openapi.yml
- filename: hevy-users-api-openapi.yml
  format: yaml
  label: Hevy Users API
  slug: hevy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-users-api-openapi.yml
- filename: hevy-workouts-api-openapi.yml
  format: yaml
  label: Hevy Workouts API
  slug: hevy-workouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/openapi/hevy-workouts-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Hevy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hevy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hevy
provider_slug: hevy
scheme_count: 2
schemes:
- applies_to: https://api.hevyapp.com (all 22 operations)
  declared_as_security_scheme: false
  declared_note: 'IMPORTANT SPEC GAP — the published OpenAPI declares NO `components.securitySchemes` and no `security` block anywhere. The key is modelled instead as a `required: true` header PARAMETER named `api-key` (schema type string, format uuid) repeated on all 22 operations. Functionally identical for a human reader; invisible to any tool that reads securitySchemes, including most codegen and every scorer that checks "securitySchemes defined + applied". Our overlay (overlays/hevy-public-api-overlay.yaml) proposes the missing ApiKeyAuth scheme.'
  expiry_documented: false
  failure:
    body: InvalidApiKey
    media_type: text/html; charset=utf-8
    note: Observed live 2026-08-27 with a syntactically valid but unissued UUID. The body is the bare string `InvalidApiKey` with a text/html content type — not JSON, not RFC 9457, and not declared anywhere in the OpenAPI (no operation declares a 401). See errors/hevy-problem-types.yml.
    status: 401
  format: uuid
  id: api-key-header
  in: header
  issuance:
    gate: Hevy Pro subscription required
    probed:
    - note: 302/307s to /login?postLoginPath=%2Fsettings%3Fdeveloper%3D for anonymous callers.
      status: 200
      url: https://hevy.com/settings?developer
    self_serve: true
    url: https://hevy.com/settings?developer
  name: api-key
  rotation_documented: false
  scopes: none
  transport: HTTPS only (TLSv1.3 observed)
  type: apiKey
- applies_to: https://hevy.com/api/v1 (6 operations, Hevy's own ChatGPT Custom GPT)
  authorization_endpoint: https://hevy.com/oauth/authorize
  discovery:
    note: No RFC 8414 / RFC 9728 / OIDC discovery document on any Hevy host — see well-known/hevy-well-known.yml. A third-party agent cannot self-onboard to this surface.
    oauth_authorization_server: 404
    oauth_protected_resource: 404
    openid_configuration: 404
  dynamic_client_registration: false
  evidence:
  - checked: '2026-08-27'
    location: /login?postLoginPath=%2Foauth%2Fauthorize
    status: 307
    url: https://hevy.com/oauth/authorize
  - checked: '2026-08-27'
    note: 'README "#### Authentication" section for the api.hevyapp.com action reads simply: OAuth.'
    status: 200
    url: https://github.com/hevyapp/hevy-gpt
  flow: authorization_code
  id: oauth2-gpt-action
  scopes_documented: false
  token_endpoint: null
  token_endpoint_note: Not published. Probed https://hevy.com/oauth/token and https://hevy.com/api/oauth/token on 2026-08-27 — both 404. The value lives only in the GPT's private action configuration.
  type: oauth2
slug: hevy-authentication
source_filename: hevy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://api.hevyapp.com/docs (Swagger UI; the OpenAPI document is embedded in\n  /docs/swagger-ui-init.js) + https://github.com/hevyapp/hevy-gpt + live probes of\n  https://api.hevyapp.com/v1/workouts and https://hevy.com/oauth/authorize on 2026-08-27.\nsummary: >-\n  Hevy runs two distinct authenticated surfaces. The public REST API on api.hevyapp.com takes a\n  per-account UUID API key in an `api-key` request header, issued to Hevy Pro subscribers from the web\n  app at https://hevy.com/settings?developer. Hevy's own ChatGPT Custom GPT calls a different host,\n  hevy.com/api/v1, over OAuth 2.0 — the authorization endpoint https://hevy.com/oauth/authorize is\n  live (307 to /login when unauthenticated) — but Hevy publishes no OAuth client registration flow,\n  token endpoint, or scope reference, so OAuth is in practice a first-party-only surface.\nschemes:\n- id: api-key-header\n  type: apiKey\n  in: header\n  name:\
  \ api-key\n  format: uuid\n  applies_to: https://api.hevyapp.com (all 22 operations)\n  declared_as_security_scheme: false\n  declared_note: >-\n    IMPORTANT SPEC GAP — the published OpenAPI declares NO `components.securitySchemes` and no\n    `security` block anywhere. The key is modelled instead as a `required: true` header PARAMETER\n    named `api-key` (schema type string, format uuid) repeated on all 22 operations. Functionally\n    identical for a human reader; invisible to any tool that reads securitySchemes, including\n    most codegen and every scorer that checks \"securitySchemes defined + applied\". Our overlay\n    (overlays/hevy-public-api-overlay.yaml) proposes the missing ApiKeyAuth scheme.\n  issuance:\n    self_serve: true\n    url: https://hevy.com/settings?developer\n    gate: Hevy Pro subscription required\n    probed:\n    - url: https://hevy.com/settings?developer\n      status: 200\n      note: 302/307s to /login?postLoginPath=%2Fsettings%3Fdeveloper%3D for anonymous\
  \ callers.\n  rotation_documented: false\n  expiry_documented: false\n  scopes: none\n  transport: HTTPS only (TLSv1.3 observed)\n  failure:\n    status: 401\n    body: InvalidApiKey\n    media_type: text/html; charset=utf-8\n    note: >-\n      Observed live 2026-08-27 with a syntactically valid but unissued UUID. The body is the bare\n      string `InvalidApiKey` with a text/html content type — not JSON, not RFC 9457, and not declared\n      anywhere in the OpenAPI (no operation declares a 401). See errors/hevy-problem-types.yml.\n- id: oauth2-gpt-action\n  type: oauth2\n  flow: authorization_code\n  applies_to: https://hevy.com/api/v1 (6 operations, Hevy's own ChatGPT Custom GPT)\n  authorization_endpoint: https://hevy.com/oauth/authorize\n  token_endpoint: null\n  token_endpoint_note: >-\n    Not published. Probed https://hevy.com/oauth/token and https://hevy.com/api/oauth/token on\n    2026-08-27 — both 404. The value lives only in the GPT's private action configuration.\n  scopes_documented:\
  \ false\n  dynamic_client_registration: false\n  discovery:\n    oauth_authorization_server: 404\n    oauth_protected_resource: 404\n    openid_configuration: 404\n    note: >-\n      No RFC 8414 / RFC 9728 / OIDC discovery document on any Hevy host — see\n      well-known/hevy-well-known.yml. A third-party agent cannot self-onboard to this surface.\n  evidence:\n  - url: https://hevy.com/oauth/authorize\n    status: 307\n    location: /login?postLoginPath=%2Foauth%2Fauthorize\n    checked: '2026-08-27'\n  - url: https://github.com/hevyapp/hevy-gpt\n    status: 200\n    note: 'README \"#### Authentication\" section for the api.hevyapp.com action reads simply: OAuth.'\n    checked: '2026-08-27'\nmtls: false\nopenid_connect: false\nsigned_requests: false\ncors:\n  allow_origin: '*'\n  allow_headers: Origin, X-Requested-With, Content-Type, Accept, api-key\n  allow_methods: GET, POST, PUT, PATCH, DELETE, OPTIONS\n  method: probed\n  note: >-\n    Observed on the live 401 from api.hevyapp.com.\
  \ The API key is a bearer-equivalent secret and the\n    API sets Access-Control-Allow-Origin `*`, so browser-side use of a Hevy key exposes it to any\n    origin; keys belong on a server.\nagent_notes: >-\n  For an autonomous agent the only reachable door is the api-key header, and it cannot be obtained\n  programmatically — a human must hold a Hevy Pro subscription and copy the key out of the web app.\n  There is no OAuth flow an arbitrary client can complete, no scopes, and no way to issue a\n  reduced-privilege credential: one key grants full read AND write over the whole account.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hevy/refs/heads/main/authentication/hevy-authentication.yml
summary_line: 2 schemes
tags:
- company
- fitness
- Health
- workout-tracking
- strength-training
- consumer-apps
- Mobile
- quantified-self
- personal-training
- health-data
---
