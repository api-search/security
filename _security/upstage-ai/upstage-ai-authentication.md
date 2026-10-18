---
anonymous_access: false
api_key_in: []
api_specs:
- filename: upstage-ai-system-one-api-openapi.yml
  format: yaml
  label: Upstage System One API
  slug: upstage-ai-system-one-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upstage-ai/refs/heads/main/openapi/upstage-ai-system-one-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Upstage Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upstage declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Upstage
provider_slug: upstage-ai
scheme_count: 1
schemes:
- credential: Upstage Console API key
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  type: http
slug: upstage-ai-authentication
source_filename: upstage-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/_ae-authored/upstage-ai-systemone-openapi-generated.yml\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  credential: Upstage Console API key\nsummary: 'API key issued in Upstage Console sent as Authorization: Bearer <UPSTAGE_API_KEY>.\n  No OAuth scopes.'\ndocs: https://console.upstage.ai/api/systemone\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upstage-ai/refs/heads/main/authentication/upstage-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- LLM
- Document AI
- OCR
- Decision Support
- Structured Outputs
- Embeddings
---
