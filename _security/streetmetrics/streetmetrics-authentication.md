---
api_key_in: []
api_specs:
- filename: streetmetrics-ad-groups-api-openapi.yml
  format: yaml
  label: StreetMetrics Ad Groups API
  slug: streetmetrics-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-ad-groups-api-openapi.yml
- filename: streetmetrics-assets-api-openapi.yml
  format: yaml
  label: StreetMetrics Assets API
  slug: streetmetrics-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-assets-api-openapi.yml
- filename: streetmetrics-attribution-studies-api-openapi.yml
  format: yaml
  label: StreetMetrics Attribution Studies API
  slug: streetmetrics-attribution-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-attribution-studies-api-openapi.yml
- filename: streetmetrics-authentication-api-openapi.yml
  format: yaml
  label: StreetMetrics Authentication API
  slug: streetmetrics-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-authentication-api-openapi.yml
- filename: streetmetrics-campaigns-api-openapi.yml
  format: yaml
  label: StreetMetrics Campaigns API
  slug: streetmetrics-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-campaigns-api-openapi.yml
- filename: streetmetrics-creatives-api-openapi.yml
  format: yaml
  label: StreetMetrics Creatives API
  slug: streetmetrics-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-creatives-api-openapi.yml
- filename: streetmetrics-frames-api-openapi.yml
  format: yaml
  label: StreetMetrics Frames API
  slug: streetmetrics-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-frames-api-openapi.yml
- filename: streetmetrics-markets-api-openapi.yml
  format: yaml
  label: StreetMetrics Markets API
  slug: streetmetrics-markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-markets-api-openapi.yml
- filename: streetmetrics-media-api-openapi.yml
  format: yaml
  label: StreetMetrics Media API
  slug: streetmetrics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-media-api-openapi.yml
- filename: streetmetrics-pixels-api-openapi.yml
  format: yaml
  label: StreetMetrics Pixels API
  slug: streetmetrics-pixels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-pixels-api-openapi.yml
- filename: streetmetrics-reporting-api-openapi.yml
  format: yaml
  label: StreetMetrics Reporting API
  slug: streetmetrics-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/openapi/streetmetrics-reporting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Streetmetrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: StreetMetrics secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: StreetMetrics
provider_slug: streetmetrics
scheme_count: 2
schemes:
- applied: false
  applied_note: Declared in components.securitySchemes but never referenced — no root-level `security` and zero of 54 operations carry an operation-level `security`. The contract therefore describes an anonymous API while the service returns 401 UNAUTHORIZED without a token (probed against GET /v3/public/markets on 2026-08-12). Corrected in overlays/streetmetrics-public-api-overlay.yaml.
  bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/streetmetrics-public-api-openapi.json
  type: http
- applied_to:
  - AuthController_authenticate
  in: header
  name: api-key
  note: Not modelled as a securityScheme — it is declared as a required header *parameter* on the token-minting operation only. It is therefore invisible to any tooling that reads securitySchemes, which is how this API can look keyless when it is not.
  parameter_name: api-key
  required: true
  sources:
  - openapi/streetmetrics-public-api-openapi.json
  type: apiKey
slug: streetmetrics-authentication
source_filename: streetmetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://docs.streetmetrics.com/recipes/how-to-authenticate-requests-and-create-tokens +\n  openapi/streetmetrics-public-api-openapi.json + live probes of\n  https://dashboard.streetmetrics.io/v3/public/ on 2026-08-12\ndocs: https://docs.streetmetrics.com/recipes/how-to-authenticate-requests-and-create-tokens\napi: StreetMetrics Public API\nsummary:\n  types:\n  - http\n  model: credential-exchange → JWT bearer\n  self_serve: false\n  note: >-\n    Credentials are the user's StreetMetrics platform email and password, so an API consumer must\n    already hold a platform account; there is no developer signup, no key-provisioning UI documented,\n    and no OAuth.\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applied: false\n  applied_note: >-\n    Declared in components.securitySchemes but never referenced — no root-level `security` and zero of\n    54 operations carry an operation-level\
  \ `security`. The contract therefore describes an anonymous\n    API while the service returns 401 UNAUTHORIZED without a token (probed against\n    GET /v3/public/markets on 2026-08-12). Corrected in\n    overlays/streetmetrics-public-api-overlay.yaml.\n  sources:\n  - openapi/streetmetrics-public-api-openapi.json\n- name: api-key\n  type: apiKey\n  in: header\n  parameter_name: api-key\n  applied_to:\n  - AuthController_authenticate\n  required: true\n  note: >-\n    Not modelled as a securityScheme — it is declared as a required header *parameter* on the\n    token-minting operation only. It is therefore invisible to any tooling that reads securitySchemes,\n    which is how this API can look keyless when it is not.\n  sources:\n  - openapi/streetmetrics-public-api-openapi.json\nflow:\n  step_1:\n    operation: AuthController_authenticate\n    request: POST https://dashboard.streetmetrics.io/v3/public/auth/authenticate\n    headers:\n      api-key: required\n      content-type: application/json\n\
  \    body: '{ \"email\": \"<platform email>\", \"password\": \"<platform password>\" }'\n    schema: AuthDto\n    note: Only `email` is listed in AuthDto.required; `password` is required in practice.\n  step_2:\n    response_schema: AuthResponse\n    response: '{ \"statusCode\": 201, \"message\": \"Token to attach to subsequent requests\", \"meta\": {}, \"data\": \"<token>\" }'\n    note: The token is the `data` string itself, not a nested object.\n  step_3:\n    usage: 'Authorization: Bearer <token> on every other operation'\ntoken:\n  lifetime_published: false\n  refresh_endpoint: none\n  revocation_endpoint: none\n  note: No expiry, refresh or revocation is documented. Treat a 401 on a previously-working token as\n    expiry and re-mint.\noauth:\n  present: false\n  oidc_discovery: 404 on all probed hosts\n  scopes: none — nothing to model, so no scopes/ artifact is written\nobserved:\n- url: https://dashboard.streetmetrics.io/v3/public/markets\n  method: GET\n  http_status: 401\n \
  \ body: '{\"status\":\"error\",\"statusCode\":401,\"errorCode\":\"UNAUTHORIZED\",\"message\":\"You do not have permission for this action\",...}'\n  fetched: '2026-08-12'\n- url: https://dashboard.streetmetrics.io/v3/public/auth/authenticate\n  method: POST\n  http_status: 400\n  body: '{\"status\":\"error\",\"statusCode\":400,\"errorCode\":\"BAD_REQUEST\",\"message\":\"Email must be an email\",...}'\n  fetched: '2026-08-12'\ndocumentation_drift:\n  finding: >-\n    The published authentication recipe (last updated 2025-05-12) shows\n    https://dashboard.streetmetrics.io/v3/api/auth/authenticate and warns readers about a \"v3/\" vs\n    \"v3/api/\" distinction. On 2026-08-12 POST to /v3/api/auth/authenticate returned 404, /v3/public/auth/authenticate\n    returned the current envelope, and the legacy /v3/auth/authenticate still answered with the older\n    envelope. The one recipe a new integrator follows first documents a path that no longer exists.\ntransport_security:\n  https_required:\
  \ true\n  tls: TLSv1.3\n  hsts: 'max-age=31536000; includeSubDomains (observed on dashboard.streetmetrics.io)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streetmetrics/refs/heads/main/authentication/streetmetrics-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Advertising
- Out-of-Home
- Measurements
- Attribution
- Analytics
- Marketing
- Location Data
- Media Planning
- Transit Advertising
- Campaign Reporting
- Audience Data
---
