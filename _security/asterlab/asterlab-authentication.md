---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Asterlab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Asterlab secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Asterlab
provider_slug: asterlab
scheme_count: 1
schemes:
- description: 'Aster API key sent as an HTTP bearer token (Authorization: Bearer <key>). Keys are created and managed in the inference console at https://www.asterlab.ai/inference/console.'
  location: header
  name: bearerAuth
  parameter: Authorization
  scheme: bearer
  source: https://www.asterlab.ai/inference
  type: http
slug: asterlab-authentication
source_filename: asterlab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.asterlab.ai/inference\ndocs: https://www.asterlab.ai/inference\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  notes: >-\n    Aster Inference is OpenAI-compatible. Authentication uses a bearer API key passed in the\n    HTTP Authorization header (Authorization: Bearer <ASTER_API_KEY>), exactly as the OpenAI\n    SDKs send it. API keys are created in the inference console; the base URL is set to\n    https://api.asterlab.ai/v1. No OAuth, OIDC, or scope surface is published.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Aster API key sent as an HTTP bearer token (Authorization: Bearer <key>). Keys are created\n    and managed in the inference console at https://www.asterlab.ai/inference/console.\n  location: header\n  parameter: Authorization\n  source: https://www.asterlab.ai/inference\nkey_management:\n  console: https://www.asterlab.ai/inference/console\n  provisioning:\
  \ Create an API key in the console and add credits; volume pricing via info@asterlab.ai.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asterlab/refs/heads/main/authentication/asterlab-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Inference
- OpenAI Compatible
- Autonomous Research
- GPU
- Developer Tools
---
