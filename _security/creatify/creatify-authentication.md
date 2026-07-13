---
api_key_in: []
api_specs:
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Avatar API
  slug: creatify-ai-avatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Link-to-Video API
  slug: creatify-link-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Shorts API
  slug: creatify-ai-shorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Custom Templates API
  slug: creatify-custom-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Product-to-Video API
  slug: creatify-product-to-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Text-to-Speech API
  slug: creatify-text-to-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Personas API
  slug: creatify-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Voices API
  slug: creatify-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify Music API
  slug: creatify-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
- filename: creatify-openapi.yml
  format: yaml
  label: Creatify AI Editing API
  slug: creatify-ai-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/openapi/creatify-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Creatify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creatify secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Creatify
provider_slug: creatify
scheme_count: 2
schemes:
- description: Your unique Creatify API identifier. Retrieved from the in-app API Dashboard at app.creatify.ai (account menu -> API Dashboard -> Show API Keys). Sent on every request alongside X-API-KEY.
  in: header
  name: apiId
  parameterName: X-API-ID
  sources:
  - openapi/creatify-openapi.yml
  type: apiKey
- description: Your secret Creatify API key. Acts as a password - keep it server-side and never expose it in client-side code. Retrieved from the in-app API Dashboard at app.creatify.ai. Sent on every request alongside X-API-ID. API access requires an active paid subscription.
  in: header
  name: apiKey
  parameterName: X-API-KEY
  sources:
  - openapi/creatify-openapi.yml
  type: apiKey
slug: creatify-authentication
source_filename: creatify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/creatify-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiId\n  type: apiKey\n  in: header\n  parameterName: X-API-ID\n  description: >-\n    Your unique Creatify API identifier. Retrieved from the in-app API Dashboard\n    at app.creatify.ai (account menu -> API Dashboard -> Show API Keys). Sent on\n    every request alongside X-API-KEY.\n  sources:\n  - openapi/creatify-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameterName: X-API-KEY\n  description: >-\n    Your secret Creatify API key. Acts as a password - keep it server-side and\n    never expose it in client-side code. Retrieved from the in-app API Dashboard\n    at app.creatify.ai. Sent on every request alongside X-API-ID. API access\n    requires an active paid subscription.\n  sources:\n  - openapi/creatify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatify/refs/heads/main/authentication/creatify-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- AI Avatars
- Video Generation
- AI Video
- Generative AI
- Marketing Video
- Text to Speech
- UGC Ads
- AI Avatar
---
