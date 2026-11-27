---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hiapi-ai-openapi-generated.yml
  format: yaml
  label: HiAPI API
  slug: hiapi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hiapi-ai/openapi/_ae-authored/hiapi-ai-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HiAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: HiAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HiAPI
provider_slug: hiapi-ai
scheme_count: 1
schemes:
- evidence: 'Every request needs an API key Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Sign up at hiapi.ai, go to Dashboard → API Keys, click Create New Key, copy the key.
  location: header
  name: Bearer
  type: http-bearer
slug: hiapi-ai-authentication
source_filename: hiapi-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://hiapi.ai/docs/authentication/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hiapi.ai/docs/authentication/\nsources:\n- https://hiapi.ai/docs/authentication/\n- https://hiapi.ai/docs/authentication\n- https://hiapi.ai/docs/zh/authentication\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request needs an API key Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at hiapi.ai, go to Dashboard → API Keys, click Create New Key, copy the key.\ndocs: https://hiapi.ai/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/hiapi-ai/authentication/hiapi-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Generative
- Image
- Video
- Audio
- Text
---
