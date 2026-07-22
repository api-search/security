---
api_key_in: []
api_specs:
- filename: openrelay-openapi.json
  format: json
  label: OpenRelay API (control-plane)
  slug: openrelay-api-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Openrelay Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRelay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenRelay
provider_slug: openrelay
scheme_count: 1
schemes:
- alt_header: x-api-key (Inference API only)
  description: 'OpenRelay API key. Send it as `Authorization: Bearer vl_…`.'
  docs: https://docs.openrelay.inc/docs/authentication
  key_prefix: vl_
  name: apiKey
  scheme: bearer
  sources:
  - openapi/openrelay-openapi.json
  - https://docs.openrelay.inc/docs/authentication
  type: http
slug: openrelay-authentication
source_filename: openrelay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/openrelay-openapi.json\ndocs: https://docs.openrelay.inc/docs/authentication\nsummary:\n  types:\n  - http\n  notes: >-\n    Single auth model. Every control-plane request is authenticated with an\n    OpenRelay API key (prefix `vl_`) sent as an HTTP Bearer token. Keys are\n    org-scoped and created in the dashboard under Settings -> API Keys; the\n    plaintext is shown once. The Inference API additionally accepts the same\n    key via an `x-api-key` header for OpenAI-SDK compatibility. No OAuth2 /\n    OIDC flows are offered.\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  key_prefix: vl_\n  description: 'OpenRelay API key. Send it as `Authorization: Bearer vl_…`.'\n  alt_header: x-api-key (Inference API only)\n  docs: https://docs.openrelay.inc/docs/authentication\n  sources:\n  - openapi/openrelay-openapi.json\n  - https://docs.openrelay.inc/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/authentication/openrelay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- GPU
- Inference
- AI
- Machine Learning
- Cloud Compute
- Infrastructure
- OpenAI-Compatible
- GPU Cloud
- LLM
---
