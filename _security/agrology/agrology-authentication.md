---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agrology-alerts-api-openapi.yml
  format: yaml
  label: Agrology Alerts API
  slug: agrology-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-alerts-api-openapi.yml
- filename: agrology-charts-api-openapi.yml
  format: yaml
  label: Agrology Charts API
  slug: agrology-charts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-charts-api-openapi.yml
- filename: agrology-dashboards-api-openapi.yml
  format: yaml
  label: Agrology Dashboards API
  slug: agrology-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-dashboards-api-openapi.yml
- filename: agrology-experiments-api-openapi.yml
  format: yaml
  label: Agrology Experiments API
  slug: agrology-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-experiments-api-openapi.yml
- filename: agrology-feedback-api-openapi.yml
  format: yaml
  label: Agrology Feedback API
  slug: agrology-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-feedback-api-openapi.yml
- filename: agrology-files-api-openapi.yml
  format: yaml
  label: Agrology Files API
  slug: agrology-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-files-api-openapi.yml
- filename: agrology-ground-truth-api-openapi.yml
  format: yaml
  label: Agrology Ground Truth API
  slug: agrology-ground-truth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-ground-truth-api-openapi.yml
- filename: agrology-metrics-api-openapi.yml
  format: yaml
  label: Agrology Metrics API
  slug: agrology-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-metrics-api-openapi.yml
- filename: agrology-microclimate-api-openapi.yml
  format: yaml
  label: Agrology Microclimate API
  slug: agrology-microclimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-microclimate-api-openapi.yml
- filename: agrology-reports-api-openapi.yml
  format: yaml
  label: Agrology Reports API
  slug: agrology-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-reports-api-openapi.yml
- filename: agrology-summary-data-api-openapi.yml
  format: yaml
  label: Agrology Summary Data API
  slug: agrology-summary-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-summary-data-api-openapi.yml
- filename: agrology-synthetics-api-openapi.yml
  format: yaml
  label: Agrology Synthetics API
  slug: agrology-synthetics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-synthetics-api-openapi.yml
- filename: agrology-topology-api-openapi.yml
  format: yaml
  label: Agrology Topology API
  slug: agrology-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-topology-api-openapi.yml
- filename: agrology-user-api-openapi.yml
  format: yaml
  label: Agrology User API
  slug: agrology-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-user-api-openapi.yml
- filename: agrology-weather-api-openapi.yml
  format: yaml
  label: Agrology Weather API
  slug: agrology-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/openapi/agrology-weather-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agrology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agrology secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agrology
provider_slug: agrology
scheme_count: 2
schemes:
- applied_to: all 90 operations
  bearerFormat: JWT
  format: 'Authorization: Bearer $ACCESS_TOKEN'
  header: Authorization
  in: header
  issuance:
    how: Log in to the Grower's Portal at https://grower.agrology.ag/ and click the username in the application footer to reveal the current access token.
    identity_provider: Amazon Cognito user pool (see identity_provider below)
    lifetime: 1 hour
    lifetime_seconds: 3600
    renewal: Tokens are not refreshable from the Public API. The user must return to the Grower's Portal for a new token after expiry — there is no documented client-credentials or refresh-token flow for machine clients.
    self_service: true
  method: derived
  name: publicApiAuthorizer
  scheme: bearer
  sources:
  - openapi/agrology-public-api-openapi.yml
  type: http
- applied_to: All operations per the README ("Clients must attach either a Bearer Token or an API key to all API requests"). Not declared in the OpenAPI securitySchemes.
  format: 'x-api-key: $API_KEY'
  header: x-api-key
  in: header
  issuance:
    how: Contact Agrology staff to receive an API Key.
    lifetime: not documented
    rotation: Not yet available. The README states "Soon, the Grower's Portal will alllow users to rotate API Keys" (provider's spelling) — key rotation is a stated roadmap item, not a shipped capability as of the 2026-07-01 docs commit.
    self_service: false
  method: searched
  name: apiKey
  sources:
  - https://github.com/agrology/public-api-docs/blob/main/README.md
  type: apiKey
slug: agrology-authentication
source_filename: agrology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://github.com/agrology/public-api-docs/blob/main/README.md\ndocs: https://github.com/agrology/public-api-docs/blob/main/README.md#authentication-security\nspec: openapi/agrology-public-api-openapi.yml\nsummary:\n  types:\n  - http\n  - apiKey\n  note: >-\n    The OpenAPI declares ONE scheme (http bearer JWT, named publicApiAuthorizer) and\n    applies it to all 90 operations. The provider README documents a SECOND, equally\n    valid credential — an x-api-key header — that the spec omits entirely. This\n    artifact records both because the docs are authoritative on the auth surface and\n    the spec is explicitly marked \"under development\" by the provider.\nschemes:\n- name: publicApiAuthorizer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer $ACCESS_TOKEN'\n  applied_to: all 90 operations\n  method: derived\n  sources:\n  - openapi/agrology-public-api-openapi.yml\n\
  \  issuance:\n    how: >-\n      Log in to the Grower's Portal at https://grower.agrology.ag/ and click the\n      username in the application footer to reveal the current access token.\n    self_service: true\n    lifetime: 1 hour\n    lifetime_seconds: 3600\n    renewal: >-\n      Tokens are not refreshable from the Public API. The user must return to the\n      Grower's Portal for a new token after expiry — there is no documented\n      client-credentials or refresh-token flow for machine clients.\n    identity_provider: Amazon Cognito user pool (see identity_provider below)\n- name: apiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  format: 'x-api-key: $API_KEY'\n  applied_to: >-\n    All operations per the README (\"Clients must attach either a Bearer Token or an\n    API key to all API requests\"). Not declared in the OpenAPI securitySchemes.\n  method: searched\n  sources:\n  - https://github.com/agrology/public-api-docs/blob/main/README.md\n  issuance:\n    how: Contact\
  \ Agrology staff to receive an API Key.\n    self_service: false\n    rotation: >-\n      Not yet available. The README states \"Soon, the Grower's Portal will alllow\n      users to rotate API Keys\" (provider's spelling) — key rotation is a stated\n      roadmap item, not a shipped capability as of the 2026-07-01 docs commit.\n    lifetime: not documented\nidentity_provider:\n  kind: oidc\n  vendor: Amazon Cognito\n  region: us-east-1\n  user_pool_id: us-east-1_qBmvSfyNK\n  discovery_document: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_qBmvSfyNK/.well-known/openid-configuration\n  discovery_http_status: 200\n  method: probed\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_qBmvSfyNK\n  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_qBmvSfyNK/.well-known/jwks.json\n  authorization_endpoint: https://auth.agrology.ag/oauth2/authorize\n  token_endpoint: https://auth.agrology.ag/oauth2/token\n  userinfo_endpoint: https://auth.agrology.ag/oauth2/userInfo\n\
  \  revocation_endpoint: https://auth.agrology.ag/oauth2/revoke\n  end_session_endpoint: https://auth.agrology.ag/logout\n  id_token_signing_alg_values_supported:\n  - RS256\n  response_types_supported:\n  - code\n  - token\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  note: >-\n    The Grower's Portal build shipped at https://grower.agrology.ag/ names this pool\n    and a public web client id in its bundle. The pool's OIDC discovery document is\n    anonymously readable and returns 200, and every interactive endpoint it advertises\n    is on auth.agrology.ag — a host Agrology controls — which is how the IdP was\n    confirmed to belong to this company rather than to a shared vendor tenant. The\n    Public API itself does NOT advertise an OIDC or OAuth discovery document on any\n    agrology.ag host; see well-known/agrology-well-known.yml.\nauthorization:\n  model: >-\n    Access is entity-scoped, not scope-scoped. A caller's reach is an access-control\n\
  \    list of customers, sites and nodes, resolved at call time rather than encoded as\n    OAuth scopes in the token.\n  discovery_endpoint: GET /access\n  discovery_url: https://api.agrology.ag/v2/access\n  shape: >-\n    Returns siteAccess[] — one entry per customer the caller can reach, each carrying\n    displayName and a sites{} map keyed by site id, each site carrying a role\n    (e.g. \"admin\") and its nodes[].\n  roles_observed:\n  - admin\n  roles_note: >-\n    The README's example shows role \"admin\" on a site. The full role vocabulary is not\n    published; /access/manage/{customerID}/{accessUser}/{accessLevel} implies an\n    accessLevel vocabulary that the docs also do not enumerate.\n  delegated_administration:\n    list: GET /access/manage/{customerID}\n    grant: POST /access/manage/{customerID}/{accessUser}/{accessLevel}\n    revoke: DELETE /access/manage/{customerID}/{accessUser}\nobserved_behavior:\n  method: probed\n  probes:\n  - url: https://api.agrology.ag/v2/access\n\
  \    request: no credential\n    status: 403\n    body: '{\"message\":\"Forbidden\"}'\n    amzn_error_type: MissingAuthenticationTokenException\n  - url: https://api.agrology.ag/v2/access\n    request: 'x-api-key: <invalid>'\n    status: 401\n    cors_allow_origin: '*'\n  note: >-\n    A missing credential returns 403 with an AWS API Gateway\n    MissingAuthenticationTokenException, while a present-but-invalid key returns 401.\n    This inverts the README, which says \"Any API request without a Bearer Token or API\n    Key will be rejected with a 401 Unauthorized error\" — an agent retrying on 401\n    alone will not recognise the unauthenticated case. The API responds with\n    Access-Control-Allow-Origin *, so browser clients may call it cross-origin.\ngaps:\n- The x-api-key scheme is documented but absent from the OpenAPI securitySchemes.\n- No refresh-token or client-credentials flow is documented; long-running machine\n  clients must use an API key obtained by contacting staff.\n\
  - API key rotation is not yet self-service.\n- The documented 401-on-missing-credential does not match the observed 403.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrology/refs/heads/main/authentication/agrology-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Agriculture
- AgTech
- Climate
- Sensors
- IoT
- Weather
- Soil
- Carbon
- Predictive Analytics
- Geospatial
- Time Series
- Machine Learning
- Viticulture
- Sustainability
- Environmental Monitoring
---
