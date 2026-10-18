---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allmodels-account-api-openapi.yml
  format: yaml
  label: Allmodels Account API
  slug: allmodels-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-account-api-openapi.yml
- filename: allmodels-allmodels-api-api-openapi.yml
  format: yaml
  label: Allmodels Allmodels API
  slug: allmodels-allmodels-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-allmodels-api-api-openapi.yml
- filename: allmodels-custom-voices-api-openapi.yml
  format: yaml
  label: Allmodels Custom Voices API
  slug: allmodels-custom-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-custom-voices-api-openapi.yml
- filename: allmodels-el-api-openapi.yml
  format: yaml
  label: Allmodels El API
  slug: allmodels-el-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-el-api-openapi.yml
- filename: allmodels-health-api-openapi.yml
  format: yaml
  label: Allmodels Health API
  slug: allmodels-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-health-api-openapi.yml
- filename: allmodels-oai-api-openapi.yml
  format: yaml
  label: Allmodels Oai API
  slug: allmodels-oai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-oai-api-openapi.yml
- filename: allmodels-realtime-api-openapi.yml
  format: yaml
  label: Allmodels Realtime API
  slug: allmodels-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/allmodels-realtime-api-openapi.yml
auth_types: []
description: AllModels uses a single API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Allmodels Authentication
name_suffix: Authentication
oauth_flows: []
overview: Allmodels declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Allmodels
provider_slug: allmodels
scheme_count: 1
schemes:
- evidence: Send your AllModels API key as a Bearer token.
  header: Authorization
  how_to_obtain: Obtain the API key by completing the email‑based sign‑up flow (POST /account/agent-signup and POST /account/agent-signup/verify) which returns the AllModels API key.
  location: header
  name: AllModels API key
  type: http-bearer
slug: allmodels-authentication
source_filename: allmodels-authentication.yml
source_heading: Authentication Profile
source_url: https://allmodels.io/docs/authentication
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://allmodels.io/docs/authentication\nsources:\n- https://allmodels.io/docs/authentication\n- https://allmodels.io/docs/api-reference/account/startAgentSignup\n- https://allmodels.io/docs\n- https://allmodels.io/docs/agentic-setup\ndescription: AllModels uses a single API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: AllModels API key\n  evidence: Send your AllModels API key as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the API key by completing the email‑based sign‑up flow (POST /account/agent-signup and POST /account/agent-signup/verify)\n    which returns the AllModels API key.\ndocs: https://allmodels.io/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/authentication/allmodels-authentication.yml
summary_line: 1 scheme
tags:
- Company
- VoiceAI
- TextToSpeech
- SpeechToText
- Real-Time
---
