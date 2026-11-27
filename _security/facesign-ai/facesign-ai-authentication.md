---
anonymous_access: false
api_key_in: []
api_specs:
- filename: facesign-ai-avatars-api-openapi.yml
  format: yaml
  label: FaceSign Avatars API
  slug: facesign-ai-avatars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facesign-ai/openapi/facesign-ai-avatars-api-openapi.yml
- filename: facesign-ai-langs-api-openapi.yml
  format: yaml
  label: FaceSign Langs API
  slug: facesign-ai-langs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facesign-ai/openapi/facesign-ai-langs-api-openapi.yml
- filename: facesign-ai-sessions-api-openapi.yml
  format: yaml
  label: FaceSign Sessions API
  slug: facesign-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/facesign-ai/openapi/facesign-ai-sessions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FaceSign Authentication
name_suffix: Authentication
oauth_flows: []
overview: FaceSign declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FaceSign
provider_slug: facesign-ai
scheme_count: 1
schemes:
- description: API keys are passed as Bearer tokens in the Authorization header. Prefix sk_test_ for sandbox, sk_prod_ for production.
  type: bearer
slug: facesign-ai-authentication
source_filename: facesign-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://docs.facesign.ai/docs/reference/authentication\nschemes:\n  - type: bearer\n    description: API keys are passed as Bearer tokens in the Authorization header. Prefix sk_test_ for sandbox, sk_prod_ for production.\n"
source_yaml_url: https://artifacts.apis.io/facesign-ai/authentication/facesign-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Identity Verification
- Deepfake Detection
- Liveness Detection
- Biometrics
---
