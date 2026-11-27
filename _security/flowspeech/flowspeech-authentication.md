---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flowspeech-quota-api-openapi.yml
  format: yaml
  label: FlowSpeech Quota API
  slug: flowspeech-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowspeech/openapi/flowspeech-quota-api-openapi.yml
- filename: flowspeech-tts-api-openapi.yml
  format: yaml
  label: FlowSpeech Tts API
  slug: flowspeech-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowspeech/openapi/flowspeech-tts-api-openapi.yml
- filename: flowspeech-voices-api-openapi.yml
  format: yaml
  label: FlowSpeech Voices API
  slug: flowspeech-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowspeech/openapi/flowspeech-voices-api-openapi.yml
auth_types: []
description: Authentication schemes for FlowSpeech public API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FlowSpeech Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlowSpeech declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FlowSpeech
provider_slug: flowspeech
scheme_count: 1
schemes:
- evidence: Header Value Authorization Bearer YOUR_API_KEY . Required on every API request.
  header: Authorization
  how_to_obtain: Create a key in API settings and copy it immediately.
  location: header
  name: Bearer
  type: http-bearer
slug: flowspeech-authentication
source_filename: flowspeech-authentication.yml
source_heading: Authentication Profile
source_url: https://flowspeech.io/docs/public-api
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flowspeech.io/docs/public-api\nsources:\n- https://flowspeech.io/docs/public-api\ndescription: Authentication schemes for FlowSpeech public API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Header Value Authorization Bearer YOUR_API_KEY . Required on every API request.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in API settings and copy it immediately.\ndocs: https://flowspeech.io/docs/public-api\n"
source_yaml_url: https://artifacts.apis.io/flowspeech/authentication/flowspeech-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Text-to-Speech
- Artificial Intelligence
- Voice
- Asynchronous
---
