---
anonymous_access: false
api_key_in: []
api_specs:
- filename: modelrush-public.openapi.yaml
  format: yaml
  label: ModelRush API
  slug: modelrush-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Moonveil-AI/modelrush-developer-tools/main/openapi/modelrush-public.openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Modelrush Authentication
name_suffix: Authentication
oauth_flows: []
overview: ModelRush secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ModelRush
provider_slug: modelrush
scheme_count: 1
schemes:
- bearerFormat: ModelRush API key
  docs: https://modelrush.ai/docs/api-keys
  name: bearerAuth
  notes:
  - 'Keys are sent only as an HTTP Authorization Bearer header: "ModelRush does not accept keys in query strings."'
  - Keys are server-side secrets -- store in a secret manager or server-side env var; never in client-side code, binaries, source control, or logs.
  - 'Rotation guidance: create a replacement key, deploy it, verify traffic, then revoke the old key (immediate revocation only when compromised).'
  - Missing, invalid, or revoked credentials return 401; rotating keys to bypass rate limits is not supported.
  - No scoping or granular permissions are documented; no OAuth2/OIDC surface exists (well-known discovery documents 404 on every host, probed 2026-09-10).
  scheme: bearer
  sources:
  - openapi/modelrush-public.openapi.yaml
  type: http
slug: modelrush-authentication
source_filename: modelrush-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/modelrush-public.openapi.yaml\ndocs: https://modelrush.ai/docs/api-keys\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: ModelRush API key\n  sources:\n  - openapi/modelrush-public.openapi.yaml\n  docs: https://modelrush.ai/docs/api-keys\n  notes:\n  - 'Keys are sent only as an HTTP Authorization Bearer header: \"ModelRush does\n    not accept keys in query strings.\"'\n  - Keys are server-side secrets -- store in a secret manager or server-side env\n    var; never in client-side code, binaries, source control, or logs.\n  - 'Rotation guidance: create a replacement key, deploy it, verify traffic, then\n    revoke the old key (immediate revocation only when compromised).'\n  - Missing, invalid, or revoked credentials return 401; rotating keys to bypass\n    rate limits is not supported.\n  - No scoping or granular permissions are documented; no OAuth2/OIDC surface\n\
  \    exists (well-known discovery documents 404 on every host, probed 2026-09-10).\nkeyless_surface:\n- operationId: listModels\n  path: GET /v1/models\n- operationId: listRegions\n  path: GET /v1/regions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelrush/refs/heads/main/authentication/modelrush-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Inference
- Multimodal
- Model Hosting
- Speech
- Image Generation
---
