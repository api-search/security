---
api_key_in: []
api_specs:
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Text-to-Video API
  slug: kling-ai-text-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Image-to-Video API
  slug: kling-ai-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Multi-Image-to-Video API
  slug: kling-ai-multi-image-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Video Extension API
  slug: kling-ai-video-extension-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Lip-Sync API
  slug: kling-ai-lip-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Video Effects API
  slug: kling-ai-video-effects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Image Generation API
  slug: kling-ai-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Virtual Try-On API
  slug: kling-ai-virtual-try-on-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
- filename: kling-ai-openapi.yml
  format: yaml
  label: Kling AI Account Resource API
  slug: kling-ai-account-resource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/openapi/kling-ai-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kling Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kling AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kling AI
provider_slug: kling-ai
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Kling AI authenticates each request with a short-lived JSON Web Token signed from an Access Key / Secret Key pair issued in the Kling AI Open Platform console. The JWT is created client-side with the HS256 algorithm: the Access Key becomes the `iss` claim, `exp` is set roughly 30 minutes in the future, and `nbf` is set about 5 seconds in the past. The Secret Key is the signing secret. The resulting token is sent as `Authorization: Bearer <token>` on every call. Because tokens expire in ~30 minutes, clients typically regenerate (and cache) tokens rather than reusing a static key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kling-ai-openapi.yml
  - https://app.klingai.com/global/dev/document-api/apiReference/commonInfo
  type: http
slug: kling-ai-authentication
source_filename: kling-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kling-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Kling AI authenticates each request with a short-lived JSON Web Token\n    signed from an Access Key / Secret Key pair issued in the Kling AI Open\n    Platform console. The JWT is created client-side with the HS256 algorithm:\n    the Access Key becomes the `iss` claim, `exp` is set roughly 30 minutes in\n    the future, and `nbf` is set about 5 seconds in the past. The Secret Key is\n    the signing secret. The resulting token is sent as `Authorization: Bearer\n    <token>` on every call. Because tokens expire in ~30 minutes, clients\n    typically regenerate (and cache) tokens rather than reusing a static key.\n  sources:\n  - openapi/kling-ai-openapi.yml\n  - https://app.klingai.com/global/dev/document-api/apiReference/commonInfo\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kling-ai/refs/heads/main/authentication/kling-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Video Generation
- AI Video
- Generative AI
- Text-to-Video
- Image-to-Video
- AI
- Generative Video
- Lip Sync
- Virtual Try-On
- Image Generation
---
