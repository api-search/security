---
api_key_in: []
auth_types:
- apiKey
- custom-signature
description: Authentication profile for the Meitu AI Open Platform (OpenAPI). Meitu issues an access key / secret key pair per application from the platform console. Requests are authenticated with an HMAC signature computed from the secret key (the platform documents signing helpers in C#, Go, Java, Python, JavaScript and PHP). Legacy MTlab synchronous endpoints accept the credential pair as api_key / api_secret query parameters.
kind: authentication
layout: security
method: searched
name: Meitu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meitu secures its APIs with apiKey and custom-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Meitu
provider_slug: meitu
scheme_count: 2
schemes:
- credential_env:
  - MEITU_OPENAPI_ACCESS_KEY
  - MEITU_OPENAPI_SECRET_KEY
  description: Per-application access key + secret key. The secret key signs each request (signature helpers published per language). Verified via /demo/authorization on the OpenAPI gateway.
  name: openapiSignature
  source: https://ai.meitu.com/doc/?id=92&type=api
  style: access-key/secret-key HMAC signature
  type: signature
- description: Legacy MTlab synchronous vision endpoints (e.g. /v1/AIDenoise, /v1/photo_scissors/sod) accept the credential pair as query parameters over HTTPS.
  in: query
  name: mtlabApiKey
  param_names:
  - api_key
  - api_secret
  source: https://ai.meitu.com/doc/?id=92&type=api
  type: apiKey
slug: meitu-authentication
source_filename: meitu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://ai.meitu.com/doc/?id=92&type=api\ndocs: https://ai.meitu.com/doc/?id=92&type=api\ndescription: >-\n  Authentication profile for the Meitu AI Open Platform (OpenAPI). Meitu issues\n  an access key / secret key pair per application from the platform console.\n  Requests are authenticated with an HMAC signature computed from the secret\n  key (the platform documents signing helpers in C#, Go, Java, Python,\n  JavaScript and PHP). Legacy MTlab synchronous endpoints accept the credential\n  pair as api_key / api_secret query parameters.\nsummary:\n  types:\n    - apiKey\n    - custom-signature\nschemes:\n  - name: openapiSignature\n    type: signature\n    style: access-key/secret-key HMAC signature\n    credential_env:\n      - MEITU_OPENAPI_ACCESS_KEY\n      - MEITU_OPENAPI_SECRET_KEY\n    description: >-\n      Per-application access key + secret key. The secret key signs each request\n      (signature helpers published\
  \ per language). Verified via\n      /demo/authorization on the OpenAPI gateway.\n    source: https://ai.meitu.com/doc/?id=92&type=api\n  - name: mtlabApiKey\n    type: apiKey\n    in: query\n    param_names:\n      - api_key\n      - api_secret\n    description: >-\n      Legacy MTlab synchronous vision endpoints (e.g.\n      /v1/AIDenoise, /v1/photo_scissors/sod) accept the credential pair as query\n      parameters over HTTPS.\n    source: https://ai.meitu.com/doc/?id=92&type=api\nnotes:\n  - HTTPS/TLS required for all requests.\n  - Free trial credentials are rate-limited to 1 QPS / 1000 calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meitu/refs/heads/main/authentication/meitu-authentication.yml
summary_line: apiKey/custom-signature · 2 schemes
tags:
- Company
- Artificial Intelligence
- Image Processing
- Computer Vision
- Video
- Generative AI
- Photo Editing
---
