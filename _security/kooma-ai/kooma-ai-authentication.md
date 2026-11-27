---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kooma-ai-images-api-openapi.yml
  format: yaml
  label: Kooma Images API
  slug: kooma-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kooma-ai/openapi/kooma-ai-images-api-openapi.yml
- filename: kooma-ai-mod-les-api-openapi.yml
  format: yaml
  label: Kooma Modèles API
  slug: kooma-ai-mod-les-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kooma-ai/openapi/kooma-ai-mod-les-api-openapi.yml
- filename: kooma-ai-synth-se-vocale-api-openapi.yml
  format: yaml
  label: Kooma Synthèse vocale API
  slug: kooma-ai-synth-se-vocale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kooma-ai/openapi/kooma-ai-synth-se-vocale-api-openapi.yml
- filename: kooma-ai-traduction-api-openapi.yml
  format: yaml
  label: Kooma Traduction API
  slug: kooma-ai-traduction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kooma-ai/openapi/kooma-ai-traduction-api-openapi.yml
- filename: kooma-ai-transcription-api-openapi.yml
  format: yaml
  label: Kooma Transcription API
  slug: kooma-ai-transcription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kooma-ai/openapi/kooma-ai-transcription-api-openapi.yml
- filename: kooma-ai-voix-api-openapi.yml
  format: yaml
  label: Kooma Voix API
  slug: kooma-ai-voix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kooma-ai/openapi/kooma-ai-voix-api-openapi.yml
auth_types: []
description: Authentication schemes for Kooma API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kooma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kooma declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kooma
provider_slug: kooma-ai
scheme_count: 1
schemes:
- evidence: Every request must carry your API key in the header Authorization , prefixed with Bearer .
  header: Authorization
  location: header
  name: API Key
  type: apiKey
slug: kooma-ai-authentication
source_filename: kooma-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://console.kooma.ai/docs/en/authentication
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://console.kooma.ai/docs/en/authentication\nsources:\n- https://console.kooma.ai/docs/en/authentication\n- https://console.kooma.ai/docs/en/authentication?lang=en\n- https://developer.kooma.ai/docs/en/authentication\n- https://console.kooma.ai/docs/quickstart\ndescription: Authentication schemes for Kooma API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request must carry your API key in the header Authorization , prefixed with Bearer .\n  location: header\n  header: Authorization\nnote: No OAuth2 or other authentication methods are documented.\ndocs: https://console.kooma.ai/docs/en/authentication\n"
source_yaml_url: https://artifacts.apis.io/kooma-ai/authentication/kooma-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Voice
- Translation
- Bambara
- Intermo
- Company
---
