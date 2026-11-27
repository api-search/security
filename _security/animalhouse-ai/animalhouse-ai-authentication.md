---
anonymous_access: false
api_key_in: []
api_specs:
- filename: animalhouse-ai-auth-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai Auth API
  slug: animalhouse-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-auth-api-openapi.yml
- filename: animalhouse-ai-house-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai House API
  slug: animalhouse-ai-house-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-house-api-openapi.yml
- filename: animalhouse-ai-payments-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai Payments API
  slug: animalhouse-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-payments-api-openapi.yml
- filename: animalhouse-ai-public-api-openapi.yml
  format: yaml
  label: AnimalHouse.ai Public API
  slug: animalhouse-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalhouse-ai/openapi/animalhouse-ai-public-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AnimalHouse.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnimalHouse.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AnimalHouse.ai
provider_slug: animalhouse-ai
scheme_count: 1
schemes:
- bearerFormat: ah_TOKEN
  description: 'Animalhouse API key. Prefix: ah_'
  scheme: bearer
  type: http
slug: animalhouse-ai-authentication
source_filename: animalhouse-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: ah_TOKEN\n    description: \"Animalhouse API key. Prefix: ah_\"\n"
source_yaml_url: https://artifacts.apis.io/animalhouse-ai/authentication/animalhouse-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Tamagotchi
- VirtualPet
- Game
- Autonomous Agents
---
