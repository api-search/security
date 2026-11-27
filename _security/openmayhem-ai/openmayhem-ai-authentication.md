---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openmayhem-ai-artifacts-api-openapi.yml
  format: yaml
  label: OpenMayhem Artifacts API
  slug: openmayhem-ai-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-artifacts-api-openapi.yml
- filename: openmayhem-ai-audio-api-openapi.yml
  format: yaml
  label: OpenMayhem Audio API
  slug: openmayhem-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-audio-api-openapi.yml
- filename: openmayhem-ai-balance-api-openapi.yml
  format: yaml
  label: OpenMayhem Balance API
  slug: openmayhem-ai-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-balance-api-openapi.yml
- filename: openmayhem-ai-completions-api-openapi.yml
  format: yaml
  label: OpenMayhem Completions API
  slug: openmayhem-ai-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-completions-api-openapi.yml
- filename: openmayhem-ai-count-tokens-api-openapi.yml
  format: yaml
  label: OpenMayhem Count Tokens API
  slug: openmayhem-ai-count-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-count-tokens-api-openapi.yml
- filename: openmayhem-ai-decisions-api-openapi.yml
  format: yaml
  label: OpenMayhem Decisions API
  slug: openmayhem-ai-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-decisions-api-openapi.yml
- filename: openmayhem-ai-embeddings-api-openapi.yml
  format: yaml
  label: OpenMayhem Embeddings API
  slug: openmayhem-ai-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-embeddings-api-openapi.yml
- filename: openmayhem-ai-estimates-api-openapi.yml
  format: yaml
  label: OpenMayhem Estimates API
  slug: openmayhem-ai-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-estimates-api-openapi.yml
- filename: openmayhem-ai-images-api-openapi.yml
  format: yaml
  label: OpenMayhem Images API
  slug: openmayhem-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-images-api-openapi.yml
- filename: openmayhem-ai-jobs-api-openapi.yml
  format: yaml
  label: OpenMayhem Jobs API
  slug: openmayhem-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-jobs-api-openapi.yml
- filename: openmayhem-ai-models-api-openapi.yml
  format: yaml
  label: OpenMayhem Models API
  slug: openmayhem-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-models-api-openapi.yml
- filename: openmayhem-ai-music-api-openapi.yml
  format: yaml
  label: OpenMayhem Music API
  slug: openmayhem-ai-music-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-music-api-openapi.yml
- filename: openmayhem-ai-profile-api-openapi.yml
  format: yaml
  label: OpenMayhem Profile API
  slug: openmayhem-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-profile-api-openapi.yml
- filename: openmayhem-ai-requests-api-openapi.yml
  format: yaml
  label: OpenMayhem Requests API
  slug: openmayhem-ai-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-requests-api-openapi.yml
- filename: openmayhem-ai-responses-api-openapi.yml
  format: yaml
  label: OpenMayhem Responses API
  slug: openmayhem-ai-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-responses-api-openapi.yml
- filename: openmayhem-ai-tokenize-api-openapi.yml
  format: yaml
  label: OpenMayhem Tokenize API
  slug: openmayhem-ai-tokenize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-tokenize-api-openapi.yml
- filename: openmayhem-ai-videos-api-openapi.yml
  format: yaml
  label: OpenMayhem Videos API
  slug: openmayhem-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-videos-api-openapi.yml
- filename: openmayhem-ai-workflows-api-openapi.yml
  format: yaml
  label: OpenMayhem Workflows API
  slug: openmayhem-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-workflows-api-openapi.yml
- filename: openmayhem-ai-chat-completions-api-openapi.yml
  format: yaml
  label: OpenMayhem Chat Completions API
  slug: openmayhem-ai-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmayhem-ai/openapi/openmayhem-ai-chat-completions-api-openapi.yml
auth_types: []
description: Authentication schemes for OpenMayhem
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: OpenMayhem Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMayhem declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpenMayhem
provider_slug: openmayhem-ai
scheme_count: 1
schemes:
- evidence: 'Every API request carries a bearer key:'
  header: Authorization
  how_to_obtain: Keys are created in the dashboard (browser session only); the secret is shown exactly once at creation.
  location: header
  name: API Key
  type: http-bearer
slug: openmayhem-ai-authentication
source_filename: openmayhem-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://openmayhem.ai/docs/authentication.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://openmayhem.ai/docs/authentication.md\nsources:\n- https://openmayhem.ai/docs/authentication.md\n- https://openmayhem.ai/docs/authentication\n- https://openmayhem.ai/docs/quickstart.md\n- https://openmayhem.ai/docs/quickstart\ndescription: Authentication schemes for OpenMayhem\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every API request carries a bearer key:'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are created in the dashboard (browser session only); the secret is shown exactly once at creation.\ndocs: https://openmayhem.ai/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/openmayhem-ai/authentication/openmayhem-ai-authentication.yml
summary_line: 1 scheme
tags:
- Inference
- Marketplace
- Models
- Peer-to-Peer
---
