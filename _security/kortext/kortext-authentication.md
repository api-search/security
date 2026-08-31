---
api_key_in: []
api_specs:
- filename: kortext-chat-api-openapi.yml
  format: yaml
  label: Kortext Chat API
  slug: kortext-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-chat-api-openapi.yml
- filename: kortext-content-api-openapi.yml
  format: yaml
  label: Kortext Content API
  slug: kortext-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-content-api-openapi.yml
- filename: kortext-health-checks-api-openapi.yml
  format: yaml
  label: Kortext Health Checks API
  slug: kortext-health-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-health-checks-api-openapi.yml
- filename: kortext-labs-api-openapi.yml
  format: yaml
  label: Kortext Labs API
  slug: kortext-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-labs-api-openapi.yml
- filename: kortext-podcast-api-openapi.yml
  format: yaml
  label: Kortext Podcast API
  slug: kortext-podcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-podcast-api-openapi.yml
- filename: kortext-quiz-api-openapi.yml
  format: yaml
  label: Kortext Quiz API
  slug: kortext-quiz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-quiz-api-openapi.yml
- filename: kortext-reading-list-api-openapi.yml
  format: yaml
  label: Kortext Reading List API
  slug: kortext-reading-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-reading-list-api-openapi.yml
- filename: kortext-test-api-openapi.yml
  format: yaml
  label: Kortext Test API
  slug: kortext-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/openapi/kortext-test-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kortext Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kortext secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kortext
provider_slug: kortext
scheme_count: 1
schemes:
- applied_to: 55 of 67 operations (per-operation; no root-level security block)
  bearerFormat: JWT
  failure_response:
    body: '{"detail":"Not authenticated"}'
    note: Uses 403 where 401 is conventional. An agent branching on 401 to trigger a token refresh will not fire on this API.
    observed_at: https://api-demo.labs.kortext.com/podcast/v1/podcasts
    status: 403
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/kortext-labs-api-openapi.json
  type: http
  unsecured_operations:
  - liveness_health_live_get
  - readiness_health_ready_get
  - chat_all_system_message_chat_v1_all_system_message_get
  - user_shelf_system_message_chat_v1_user_shelf_system_message_get
  - hello_chat_v1_test_hello_get
slug: kortext-authentication
source_filename: kortext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: >-\n  openapi/kortext-labs-api-openapi.json (securitySchemes + per-operation security), Kortext's own\n  published front-end runtime configuration at https://vle.kortext.com/assets/config.json, and\n  live unauthenticated probes of https://app.kortext.com/account/token, https://vle.kortext.com and\n  https://api-demo.labs.kortext.com, 2026-08-23.\nsummary:\n  types:\n  - http\n  self_serve: false\n  public_api_keys: false\n  note: >-\n    Kortext has NO public authentication documentation — no developer portal, no auth guide, no\n    key-issuance page. Everything below is read from the one published contract and from observed\n    runtime behaviour. Credentials are institutional: an account is provisioned through a\n    university or publisher agreement, not through a signup form.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/kortext-labs-api-openapi.json\n  applied_to:\
  \ 55 of 67 operations (per-operation; no root-level security block)\n  unsecured_operations:\n  - liveness_health_live_get\n  - readiness_health_ready_get\n  - chat_all_system_message_chat_v1_all_system_message_get\n  - user_shelf_system_message_chat_v1_user_shelf_system_message_get\n  - hello_chat_v1_test_hello_get\n  failure_response:\n    status: 403\n    body: '{\"detail\":\"Not authenticated\"}'\n    observed_at: https://api-demo.labs.kortext.com/podcast/v1/podcasts\n    note: >-\n      Uses 403 where 401 is conventional. An agent branching on 401 to trigger a token refresh will\n      not fire on this API.\ntoken_issuance:\n  endpoint: https://app.kortext.com/account/token\n  status_unauthenticated: 401\n  source: https://vle.kortext.com/assets/config.json (field authTokenApiUrl)\n  grant_documented: false\n  note: >-\n    The token endpoint is named in Kortext's own published runtime configuration but the grant\n    type, credential format and token lifetime are not documented anywhere\
  \ public.\ninstitutional_authentication:\n  mechanism: 1EdTech LTI launch\n  note: >-\n    For institutional users the real front door is not an API credential at all — it is an LTI 1.1\n    or LTI 1.3 launch from the university's VLE, which carries identity from the institution into\n    Kortext. LTI 1.3 is built on an OIDC third-party-initiated login, so an OIDC flow is\n    implemented behind these endpoints even though no discovery document is served.\n  endpoints:\n    lti_1_1_launch: https://vle.kortext.com/api/v1/lti/v1.1/launch\n    lti_1_3_deep_link_request: https://vle.kortext.com/api/v1/lti/v1.3/deep-link-request\n    jwks: https://lti.dev.kortext.com/jwks\n  jwks_observed:\n    url: https://lti.dev.kortext.com/jwks\n    status: 200\n    body: '{\"keys\":[]}'\n    note: >-\n      A JWKS keyset endpoint is deployed on the LTI dev host but is empty; no production keyset is\n      served on a discoverable path.\n  cross_ref: conformance/kortext-conformance.yml\nnot_supported:\n\
  \  oauth2: >-\n    No oauth2 securityScheme, no authorization or token metadata document. See scopes/ — none\n    written, because there is no scope surface to derive.\n  openIdConnect: No openIdConnect scheme declared and no /.well-known/openid-configuration served.\n  apiKey: No apiKey scheme declared on any operation.\n  mutualTLS: Not declared.\n  oauth_discovery:\n  - url: https://api-demo.labs.kortext.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://api-demo.labs.kortext.com/.well-known/openid-configuration\n    status: 404\n  - url: https://kortext.com/.well-known/openid-configuration\n    status: 301\n    note: Redirects to the marketing homepage — a soft-404, not a document.\ngaps:\n- No published authentication documentation of any kind.\n- No token lifetime, refresh mechanism, or revocation path documented.\n- No scopes or permission model — the bearer token is all-or-nothing across 55 operations.\n- 403 used in place of 401, which breaks conventional\
  \ client retry logic.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kortext/refs/heads/main/authentication/kortext-authentication.yml
summary_line: http · 1 scheme
tags:
- education
- edtech
- higher-education
- digital-textbooks
- learning-analytics
- artificial-intelligence
- content-delivery
- lti
- libraries
- student-engagement
- publishing
---
