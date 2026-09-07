---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eden-ai-audio-features-openapi.json
  format: json
  label: Eden AI Audio API
  slug: eden-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-audio-features-openapi.json
- filename: eden-ai-image-features-openapi.json
  format: json
  label: Eden AI Image API
  slug: eden-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-image-features-openapi.json
- filename: eden-ai-ocr-features-openapi.json
  format: json
  label: Eden AI OCR API
  slug: eden-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-ocr-features-openapi.json
- filename: eden-ai-text-features-openapi.json
  format: json
  label: Eden AI Text API
  slug: eden-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-text-features-openapi.json
- filename: eden-ai-translation-features-openapi.json
  format: json
  label: Eden AI Translation API
  slug: eden-ai-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-translation-features-openapi.json
- filename: eden-ai-v3-openapi.json
  format: json
  label: Eden AI API V3
  slug: eden-ai-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-v3-openapi.json
- filename: eden-ai-video-features-openapi.json
  format: json
  label: Eden AI Video API
  slug: eden-ai-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-video-features-openapi.json
- filename: eden-ai-llm-features-openapi.json
  format: json
  label: Eden AI LLM API (v2)
  slug: eden-ai-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-llm-features-openapi.json
- filename: eden-ai-multimodal-features-openapi.json
  format: json
  label: Eden AI Multimodal API
  slug: eden-ai-multimodal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-multimodal-features-openapi.json
- filename: eden-ai-user-management-openapi.json
  format: json
  label: Eden AI User Management API
  slug: eden-ai-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-user-management-openapi.json
- filename: eden-ai-cost-monitoring-openapi.json
  format: json
  label: Eden AI Cost Monitoring API
  slug: eden-ai-cost-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-cost-monitoring-openapi.json
- filename: eden-ai-organization-management-openapi.json
  format: json
  label: Eden AI Organization Management API
  slug: eden-ai-organization-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/_original/eden-ai-organization-management-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Eden Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eden AI secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eden AI
provider_slug: eden-ai
scheme_count: 2
schemes:
- name: AuthBearer
  note: The v3 gateway scheme. Authorization; Bearer <key>.
  scheme: bearer
  sources:
  - openapi/_original/eden-ai-v3-openapi.json
  type: http
- bearerFormat: JWT
  name: FeatureApiAuth
  note: The legacy v2 feature scheme. bearerFormat is declared as JWT, which matches Eden AI's own description of the legacy primary/sandbox key as "a JWT stored in a User column, not a Token row".
  scheme: bearer
  sources:
  - openapi/_original/eden-ai-text-features-openapi.json
  - openapi/_original/eden-ai-image-features-openapi.json
  - openapi/_original/eden-ai-ocr-features-openapi.json
  - openapi/_original/eden-ai-audio-features-openapi.json
  - openapi/_original/eden-ai-video-features-openapi.json
  - openapi/_original/eden-ai-translation-features-openapi.json
  - openapi/_original/eden-ai-multimodal-features-openapi.json
  - openapi/_original/eden-ai-llm-features-openapi.json
  - openapi/_original/eden-ai-user-management-openapi.json
  type: http
slug: eden-ai-authentication
source_filename: eden-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.edenai.co/docs/v3/organization/management-api\ndocs:\n  - https://www.edenai.co/docs/v3/organization/management-api\n  - https://www.edenai.co/docs/v3/general/custom-api-keys\n  - https://www.edenai.co/docs/v3/general/sandbox\n  - https://www.edenai.co/docs/v3/quickstart/first-llm-call\nspecs:\n  - openapi/_original/eden-ai-v3-openapi.json\n  - openapi/_original/eden-ai-text-features-openapi.json\n  - openapi/_original/eden-ai-user-management-openapi.json\nsummary:\n  types:\n    - http\n  model: bearer-api-key\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Eden AI is a pure bearer-key API. There is no OAuth 2.0 or OIDC surface anywhere in the twelve\n    first-party specs, and no /.well-known/openid-configuration or\n    /.well-known/oauth-authorization-server is served on any host (all 404, see\n    well-known/eden-ai-well-known.yml). Authorization is nevertheless SCOPED — see\n\
  \    scopes/eden-ai-scopes.yml — because management keys carry explicit manage:* scopes.\nschemes:\n  - name: AuthBearer\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/_original/eden-ai-v3-openapi.json\n    note: The v3 gateway scheme. Authorization; Bearer <key>.\n  - name: FeatureApiAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    sources:\n      - openapi/_original/eden-ai-text-features-openapi.json\n      - openapi/_original/eden-ai-image-features-openapi.json\n      - openapi/_original/eden-ai-ocr-features-openapi.json\n      - openapi/_original/eden-ai-audio-features-openapi.json\n      - openapi/_original/eden-ai-video-features-openapi.json\n      - openapi/_original/eden-ai-translation-features-openapi.json\n      - openapi/_original/eden-ai-multimodal-features-openapi.json\n      - openapi/_original/eden-ai-llm-features-openapi.json\n      - openapi/_original/eden-ai-user-management-openapi.json\n    note: >-\n      The legacy v2 feature\
  \ scheme. bearerFormat is declared as JWT, which matches Eden AI's own\n      description of the legacy primary/sandbox key as \"a JWT stored in a User column, not a Token row\".\ncredential_tiers:\n  - tier: issuer key\n    prefix: mgmt-eden-\n    can: [mint auth keys]\n    cannot: [read, write, call inference]\n    issued_by: Dashboard, Account -> Management Keys (shown once)\n    docs: https://www.edenai.co/docs/v3/organization/management-api\n    note: Store like a root secret — it can mint its way down to inference.\n  - tier: auth key (worker)\n    prefix: mgmt-eden-\n    scopes: [manage:read, manage:write]\n    can: [manage the org, mint inference keys]\n    issued_by: POST /v3/manage/auth-keys with an issuer key (manage:mint), or the dashboard\n  - tier: inference key\n    prefix: sk-eden-\n    can: [call the inference API, bills the org]\n    issued_by: POST /v3/manage/keys with an auth key (manage:write), or the dashboard\n    attributes: [name, balance, balance_reset_period,\
  \ balance_reset_amount, expire_time, guardrail]\n  - tier: legacy account token\n    prefix: null\n    format: JWT stored on the User row\n    can: [call the inference API]\n    note: >-\n      Superseded. POST /v2/user/custom_token/legacy/{legacy_type}/regenerate/ converts one into a real\n      hashed sk-eden custom key.\ntoken_types:\n  - {type: api_token, real_provider_calls: true, cost: pay-per-use}\n  - {type: sandbox_api_token, real_provider_calls: false, cost: free,\n     docs: https://www.edenai.co/docs/v3/general/sandbox}\ntransport:\n  header: Authorization\n  format: 'Bearer <key>'\n  hosts:\n    - https://api.edenai.run\n    - https://api.eu.edenai.run\n    - https://mcp.edenai.run/mcp\n  note: The same key works on the global and EU endpoints; there is no separate EU key to issue.\nexpiry_and_rotation:\n  default: >-\n    Management and inference keys do not expire unless expire_time is set explicitly.\n  rotate_inference_key: POST /v3/manage/keys/{key_id}/rotate (manage:write)\
  \ — same identity, new secret, returned once\n  rotate_legacy_token: POST /v2/user/custom_token/{name}/rotate/\n  revoke: DELETE /v3/manage/keys/{key_id} (irreversible — destroys the secret, keeps the row marked revoked)\n  introspection: GET /v3/manage/whoami (own org, scopes, expiry) and GET /v2/user/custom_token/me/ (own label, masking, budget, balance)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/authentication/eden-ai-authentication.yml
summary_line: http · 2 schemes
tags:
- Artificial Intelligence
- AI Gateway
- LLM
- Machine Learning
- OCR
- Translation
- Speech
- Computer Vision
- Model Context Protocol
- Emotion Detection
---
