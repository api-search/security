---
api_key_in: []
api_specs:
- filename: vidu-ai-generation-api-openapi.yml
  format: yaml
  label: Vidu Generation API
  slug: vidu-ai-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-generation-api-openapi.yml
- filename: vidu-ai-tasks-api-openapi.yml
  format: yaml
  label: Vidu Tasks API
  slug: vidu-ai-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/openapi/vidu-ai-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: documented
name: Vidu Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vidu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vidu
provider_slug: vidu-ai
scheme_count: 1
schemes:
- format: Token {api_key}
  headerName: Authorization
  in: header
  keyPrefix: vda_
  name: vidu_token
  note: 'Vidu authenticates every request with an API key sent in the Authorization header using the "Token" scheme (Authorization: Token vda_xxx), not standard HTTP Bearer. Keys are created in the Vidu platform account and are prepaid against a credit balance.'
  sources:
  - https://docs.platform.vidu.com/7207545m0
  - https://platform.vidu.com/docs/text-to-video
  type: apiKey
slug: vidu-ai-authentication
source_filename: vidu-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: documented\nsource: https://docs.platform.vidu.com/7207545m0\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: vidu_token\n  type: apiKey\n  in: header\n  headerName: Authorization\n  format: Token {api_key}\n  keyPrefix: vda_\n  note: >-\n    Vidu authenticates every request with an API key sent in the Authorization\n    header using the \"Token\" scheme (Authorization: Token vda_xxx), not standard\n    HTTP Bearer. Keys are created in the Vidu platform account and are prepaid\n    against a credit balance.\n  sources:\n  - https://docs.platform.vidu.com/7207545m0\n  - https://platform.vidu.com/docs/text-to-video\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidu-ai/refs/heads/main/authentication/vidu-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- Reference-to-Video
- U-ViT
- Diffusion
---
