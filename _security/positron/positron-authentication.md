---
api_key_in:
- header
api_specs:
- filename: positron-access-tokens-api-openapi.yml
  format: yaml
  label: Positron Access Tokens API
  slug: positron-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-access-tokens-api-openapi.yml
- filename: positron-completion-api-openapi.yml
  format: yaml
  label: Positron Completion API
  slug: positron-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-completion-api-openapi.yml
- filename: positron-models-api-openapi.yml
  format: yaml
  label: Positron Models API
  slug: positron-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-models-api-openapi.yml
- filename: positron-service-nodes-api-openapi.yml
  format: yaml
  label: Positron Service Nodes API
  slug: positron-service-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-service-nodes-api-openapi.yml
- filename: positron-users-api-openapi.yml
  format: yaml
  label: Positron Users API
  slug: positron-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/openapi/positron-users-api-openapi.yml
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Positron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Positron secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Positron
provider_slug: positron
scheme_count: 2
schemes:
- api: Positron Olivaw OpenAI-Compatible Inference API
  applied: 'root-level `security: [{apiKey: []}]` — applies to all four operations (listModels, getModel, createChatCompletion, createCompletion)'
  in: header
  name: apiKey
  parameter: authorization
  sources:
  - openapi/positron-inference-openapi.yml
  type: apiKey
- api: Positron Olivaw Admin API
  applied: 'root-level `security: [{bearer: [API key]}]` — applies to all 19 admin operations'
  bearerFormat: API key
  name: bearer
  scheme: bearer
  sources:
  - openapi/positron-admin-openapi.yml
  spec_gap: The published admin document references the `bearer` scheme in its root `security` block but declares no `components.securitySchemes`, so the scheme object itself is undefined in the specification. Type/scheme recorded here from the requirement's shape and the "API key" label it carries.
  type: http
slug: positron-authentication
source_filename: positron-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: openapi/positron-inference-openapi.yml, openapi/positron-admin-openapi.yml\ndocs: https://support.positron.ai/api-documentation\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows: []\n  model: >-\n    Static API keys only. Inference calls carry the key in the `authorization` header; the admin\n    control plane declares a bearer requirement. Keys are minted and revoked through the admin\n    API (createAccessToken / deleteAccessToken). No OAuth 2.0, no OIDC, no scopes, no mTLS.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: authorization\n  api: Positron Olivaw OpenAI-Compatible Inference API\n  applied: >-\n    root-level `security: [{apiKey: []}]` — applies to all four operations (listModels, getModel,\n    createChatCompletion, createCompletion)\n  sources:\n  - openapi/positron-inference-openapi.yml\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat:\
  \ API key\n  api: Positron Olivaw Admin API\n  applied: >-\n    root-level `security: [{bearer: [API key]}]` — applies to all 19 admin operations\n  sources:\n  - openapi/positron-admin-openapi.yml\n  spec_gap: >-\n    The published admin document references the `bearer` scheme in its root `security` block but\n    declares no `components.securitySchemes`, so the scheme object itself is undefined in the\n    specification. Type/scheme recorded here from the requirement's shape and the \"API key\"\n    label it carries.\ncredential_lifecycle:\n  issued_by: openapi/positron-admin-openapi.yml#createAccessToken\n  revoked_by: openapi/positron-admin-openapi.yml#deleteAccessToken\n  audited_by:\n  - openapi/positron-admin-openapi.yml#listAccessTokens\n  - openapi/positron-admin-openapi.yml#getAccessToken\n  rotation: >-\n    Create-then-delete. There is no update operation on AccessToken, so rotation means minting a\n    replacement and revoking the old credential.\noperator_authentication:\n\
  \  surface: Olivaw GUI (hosted deployments)\n  method: Google account via Auth0\n  source: https://support.positron.ai/user-guide\n  note: >-\n    Human operator sign-in to the Olivaw web console, distinct from API credentials. No OIDC\n    discovery document is published for the API itself.\ndiscovery:\n  openid_configuration: absent (404 on every Positron host)\n  oauth_authorization_server: absent (404 on every Positron host)\n  oauth_protected_resource: absent (404 on every Positron host)\n  probed: '2026-08-02'\ngaps:\n- No 401/403 responses are documented on either API despite both declaring root-level security.\n- No scope model — see conformance/positron-conformance.yml (oauth2 = false); no scopes/ artifact\n  is emitted for this provider.\n- No documented key prefix, key format, expiry or IP allowlist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/positron/refs/heads/main/authentication/positron-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Artificial Intelligence
- AI Inference
- inference-hardware
- AI Accelerators
- Large Language Models
- Transformers
- OpenAI-Compatible
- Machine-Learning
- Semiconductors
- Data-Center
- llm-serving
- Model Hosting
---
