---
api_key_in:
- header
api_specs:
- filename: codeproject-articles-api-openapi.yml
  format: yaml
  label: CodeProject Articles API
  slug: codeproject-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-articles-api-openapi.yml
- filename: codeproject-audio-api-openapi.yml
  format: yaml
  label: CodeProject Audio API
  slug: codeproject-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-audio-api-openapi.yml
- filename: codeproject-forummessages-api-openapi.yml
  format: yaml
  label: CodeProject ForumMessages API
  slug: codeproject-forummessages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-forummessages-api-openapi.yml
- filename: codeproject-image-processing-api-openapi.yml
  format: yaml
  label: CodeProject Image-Processing API
  slug: codeproject-image-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-image-processing-api-openapi.yml
- filename: codeproject-my-api-openapi.yml
  format: yaml
  label: CodeProject My API
  slug: codeproject-my-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-my-api-openapi.yml
- filename: codeproject-questions-api-openapi.yml
  format: yaml
  label: CodeProject Questions API
  slug: codeproject-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-questions-api-openapi.yml
- filename: codeproject-status-api-openapi.yml
  format: yaml
  label: CodeProject Status API
  slug: codeproject-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-status-api-openapi.yml
- filename: codeproject-text-api-openapi.yml
  format: yaml
  label: CodeProject Text API
  slug: codeproject-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-text-api-openapi.yml
- filename: codeproject-training-api-openapi.yml
  format: yaml
  label: CodeProject Training API
  slug: codeproject-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-training-api-openapi.yml
- filename: codeproject-vision-alpr-api-openapi.yml
  format: yaml
  label: CodeProject Vision-ALPR API
  slug: codeproject-vision-alpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-alpr-api-openapi.yml
- filename: codeproject-vision-detection-api-openapi.yml
  format: yaml
  label: CodeProject Vision-Detection API
  slug: codeproject-vision-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-detection-api-openapi.yml
- filename: codeproject-vision-face-api-openapi.yml
  format: yaml
  label: CodeProject Vision-Face API
  slug: codeproject-vision-face-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-face-api-openapi.yml
- filename: codeproject-vision-scene-api-openapi.yml
  format: yaml
  label: CodeProject Vision-Scene API
  slug: codeproject-vision-scene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/openapi/codeproject-vision-scene-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Codeproject Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- implicit
overview: CodeProject secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and implicit flow(s).
provider_name: CodeProject
provider_slug: codeproject
scheme_count: 2
schemes:
- description: CodeProject.AI Server runs locally and does not require authentication by default. Operators are expected to keep the service on a private network or behind their own reverse proxy.
  in: header
  name: none
  parameter: X-Disabled
  sources:
  - openapi/codeproject-ai-server-openapi.yml
  type: apiKey
- description: OAuth 2.0 Bearer Tokens are issued by the CodeProject identity server. Use Client Credentials Grant for read access to public resources and Authorization Code Grant or Implicit Grant for the My API.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.codeproject.com/Token
  - authorizationUrl: https://api.codeproject.com/Authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.codeproject.com/Token
  - authorizationUrl: https://api.codeproject.com/Authorize
    flow: implicit
    scopes: 1
  name: oauth2
  sources:
  - openapi/codeproject-rest-api-openapi.yml
  type: oauth2
slug: codeproject-authentication
source_filename: codeproject-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/codeproject-ai-server-openapi.yml, openapi/codeproject-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - implicit\nschemes:\n- name: none\n  type: apiKey\n  in: header\n  parameter: X-Disabled\n  description: CodeProject.AI Server runs locally and does not require authentication by default.\n    Operators are expected to keep the service on a private network or behind their own reverse\n    proxy.\n  sources:\n  - openapi/codeproject-ai-server-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.codeproject.com/Token\n    scopes: 1\n  - flow: authorizationCode\n    authorizationUrl: https://api.codeproject.com/Authorize\n    tokenUrl: https://api.codeproject.com/Token\n    scopes: 1\n  - flow: implicit\n    authorizationUrl: https://api.codeproject.com/Authorize\n\
  \    scopes: 1\n  description: OAuth 2.0 Bearer Tokens are issued by the CodeProject identity server. Use Client\n    Credentials Grant for read access to public resources and Authorization Code Grant or Implicit\n    Grant for the My API.\n  sources:\n  - openapi/codeproject-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeproject/refs/heads/main/authentication/codeproject-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI
- Articles
- Community
- Computer Vision
- Developer Community
- Face Recognition
- Forum
- Knowledge Base
- License Plate Recognition
- Object Detection
- Q&A
- Software Development
- Tutorials
---
