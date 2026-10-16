---
anonymous_access: false
api_key_in: []
api_specs:
- filename: allmodels-openapi-generated.yml
  format: yaml
  label: Allmodels API
  slug: allmodels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allmodels/refs/heads/main/openapi/_ae-authored/allmodels-openapi-generated.yml
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
- RealTime
---
