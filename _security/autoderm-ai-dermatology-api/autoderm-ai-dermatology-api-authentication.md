---
api_key_in: []
api_specs:
- filename: autoderm-ai-dermatology-api-device-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Device API
  slug: autoderm-ai-dermatology-api-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-device-api-openapi.yml
- filename: autoderm-ai-dermatology-api-inference-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Inference API
  slug: autoderm-ai-dermatology-api-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-inference-api-openapi.yml
- filename: autoderm-ai-dermatology-api-system-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API System API
  slug: autoderm-ai-dermatology-api-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-system-api-openapi.yml
- filename: autoderm-ai-dermatology-api-utils-api-openapi.yml
  format: yaml
  label: Autoderm – AI Dermatology API Utils API
  slug: autoderm-ai-dermatology-api-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/openapi/autoderm-ai-dermatology-api-utils-api-openapi.yml
auth_types:
- http
description: 'Autoderm uses a single authentication mechanism: an HTTP Bearer token in the Authorization header, issued per organization from the Autoderm web application. There is no OAuth 2.0 authorization server, no OpenID Connect discovery document, and therefore no scope surface — see the no_oauth_surface block below. The legacy platform used a different scheme (an Api-Key header against autoderm.ai/v1) which the current platform does not accept.'
kind: authentication
layout: security
method: searched
name: Autoderm Ai Dermatology Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autoderm – AI Dermatology API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Autoderm – AI Dermatology API
provider_slug: autoderm-ai-dermatology-api
scheme_count: 1
schemes:
- applied_to:
  - detect_blur_v1_utils_detect_blur_post
  - infer_genitals_v1_v1_infer_genitals_v1_post
  - infer_diseases_v1_v1_infer_diseases_v1_post
  - get_disease_catalog_v1_v1_infer_diseases_v1_diseases_get
  - infer_skin_tone_v1_v1_infer_skin_tone_v1_post
  format: 'Authorization: Bearer YOUR_API_TOKEN'
  header: Authorization
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/autoderm-ai-dermatology-api-openapi.yml
  type: http
slug: autoderm-ai-dermatology-api-authentication
source_filename: autoderm-ai-dermatology-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: openapi/autoderm-ai-dermatology-api-openapi.yml\ndocs: https://docs.autoderm.ai/en/getting-started/getting-started\ndescription: >-\n  Autoderm uses a single authentication mechanism: an HTTP Bearer token in the\n  Authorization header, issued per organization from the Autoderm web\n  application. There is no OAuth 2.0 authorization server, no OpenID Connect\n  discovery document, and therefore no scope surface — see the\n  no_oauth_surface block below. The legacy platform used a different scheme\n  (an Api-Key header against autoderm.ai/v1) which the current platform does\n  not accept.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - bearer\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    header: Authorization\n    format: 'Authorization: Bearer YOUR_API_TOKEN'\n    sources:\n      - openapi/autoderm-ai-dermatology-api-openapi.yml\n    applied_to:\n    \
  \  - detect_blur_v1_utils_detect_blur_post\n      - infer_genitals_v1_v1_infer_genitals_v1_post\n      - infer_diseases_v1_v1_infer_diseases_v1_post\n      - get_disease_catalog_v1_v1_infer_diseases_v1_diseases_get\n      - infer_skin_tone_v1_v1_infer_skin_tone_v1_post\nunauthenticated_operations:\n  description: >-\n    Operations the spec declares with no security requirement. Verified live:\n    GET https://api.autoderm.ai/v1/label and /health and /version all return 200\n    anonymously.\n  operations:\n    - get_health_healthz_get\n    - get_health_healthz_head\n    - get_health_health_get\n    - get_health_health_head\n    - get_version_version_get\n    - get_health_v1_system_healthz_get\n    - get_health_v1_system_healthz_head\n    - get_health_v1_system_health_get\n    - get_health_v1_system_health_head\n    - get_version_v1_system_version_get\n    - get_label_v1_label_get\n  spec_gap:\n    - operation: infer_age_v1_v1_infer_age_v1_post\n      note: >-\n        Declared with NO\
  \ security requirement in the published OpenAPI while\n        every sibling inference operation requires HTTPBearer. Recorded as an\n        observed spec inconsistency, not as a claim that the endpoint is open —\n        it was not called, because calling an inference endpoint anonymously\n        would be probing for an auth bypass.\ncredential_issuance:\n  console: https://app.autoderm.ai\n  sign_up: https://app.autoderm.ai/en/auth/sign-up\n  login: https://app.autoderm.ai/en/auth/login\n  key_management: >-\n    API key management from the Autoderm dashboard; the Basic plan advertises\n    \"unlimited API keys with role-based access\".\n  rotation: >-\n    Docs place responsibility for rotation on the client: \"The API client is\n    responsible for preventing unauthorized access and for rotating keys if\n    compromise is suspected.\"\nhandling_rules:\n  quoted_from_docs:\n    - API access tokens are confidential credentials and must be kept secret at all times.\n    - Be stored\
  \ securely\n    - Never be embedded in client-side code\n    - Never be exposed in public repositories, logs, or user interfaces\n  server_to_server_only: >-\n    \"API keys are intended for server-to-server communication only.\"\nno_oauth_surface:\n  oauth2: false\n  openid_connect: false\n  scopes: false\n  evidence:\n    - https://api.autoderm.ai/.well-known/openid-configuration returned 404\n    - https://api.autoderm.ai/.well-known/oauth-authorization-server returned 404\n    - OpenAPI components.securitySchemes declares only HTTPBearer (type http)\n  note: >-\n    scopes/ is deliberately NOT emitted for this provider — a bearer-token API\n    with no authorization server has no scope surface to capture.\nfailure_behavior:\n  status: 401\n  content_type: application/json\n  body: '{\"detail\":\"Missing Authorization header\"}'\n  observed: '2026-08-09 — GET https://api.autoderm.ai/v1/infer-diseases/v1/diseases with no Authorization header'\n  note: >-\n    The 401 is NOT documented\
  \ in the OpenAPI; the spec declares only 200 and\n    422 on secured operations. See errors/ for the full catalog.\nlegacy:\n  platform: https://legacy.autoderm.ai\n  base_url: https://autoderm.ai/v1\n  scheme: Api-Key header\n  status: >-\n    Not supported on the new platform. Docs: \"Legacy authentication mechanisms\n    are not supported on the new platform.\"\n  docs: https://docs.autoderm.ai/en/disease-detection-api/migrating-from-legacy-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoderm-ai-dermatology-api/refs/heads/main/authentication/autoderm-ai-dermatology-api-authentication.yml
summary_line: http · 1 scheme
tags:
- dermatology-api
- ai-dermatology
- medical-imaging
- telemedicine
- skin-analysis
- rest-api
- openapi
- llms-txt
- ce-marked
- white-label
- healthcare
- medical-ai
- computer-vision
- medical-device
- icd-10
- image-classification
- clinical-decision-support
- triage
---
