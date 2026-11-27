---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: videobackgroundremover-ai-jobs-api-openapi.yml
  format: yaml
  label: Video Background Remover Jobs API
  slug: videobackgroundremover-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/videobackgroundremover-ai/openapi/videobackgroundremover-ai-jobs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Video Background Remover Authentication
name_suffix: Authentication
oauth_flows: []
overview: Video Background Remover secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Video Background Remover
provider_slug: videobackgroundremover-ai
scheme_count: 3
schemes:
- description: 'API key issued on /video-background-remover-api, prefix vbr (Authorization: Bearer vbr_sk_...). Keep keys in backend scripts.'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/videobackgroundremover-ai-openapi.json
  type: http
- in: query
  name: DownloadExpiry
  parameter: exp
  sources:
  - openapi/videobackgroundremover-ai-openapi.json
  type: apiKey
- in: query
  name: DownloadSignature
  parameter: sig
  sources:
  - openapi/videobackgroundremover-ai-openapi.json
  type: apiKey
slug: videobackgroundremover-ai-authentication
source_filename: videobackgroundremover-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/videobackgroundremover-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: 'API key issued on /video-background-remover-api, prefix vbr (Authorization:\n    Bearer vbr_sk_...). Keep keys in backend scripts.'\n  sources:\n  - openapi/videobackgroundremover-ai-openapi.json\n- name: DownloadExpiry\n  type: apiKey\n  in: query\n  parameter: exp\n  sources:\n  - openapi/videobackgroundremover-ai-openapi.json\n- name: DownloadSignature\n  type: apiKey\n  in: query\n  parameter: sig\n  sources:\n  - openapi/videobackgroundremover-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/videobackgroundremover-ai/authentication/videobackgroundremover-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Video
- Background
- Removal
- Artificial Intelligence
- Media
- Editing
---
