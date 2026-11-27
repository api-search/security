---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flipletters-com-discovery-api-openapi.yml
  format: yaml
  label: FlipLetters Discovery API
  slug: flipletters-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flipletters-com/openapi/flipletters-com-discovery-api-openapi.yml
- filename: flipletters-com-keys-api-openapi.yml
  format: yaml
  label: FlipLetters Keys API
  slug: flipletters-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flipletters-com/openapi/flipletters-com-keys-api-openapi.yml
- filename: flipletters-com-postiz-api-openapi.yml
  format: yaml
  label: FlipLetters Postiz API
  slug: flipletters-com-postiz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flipletters-com/openapi/flipletters-com-postiz-api-openapi.yml
- filename: flipletters-com-render-api-openapi.yml
  format: yaml
  label: FlipLetters Render API
  slug: flipletters-com-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flipletters-com/openapi/flipletters-com-render-api-openapi.yml
- filename: flipletters-com-teams-api-openapi.yml
  format: yaml
  label: FlipLetters Teams API
  slug: flipletters-com-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flipletters-com/openapi/flipletters-com-teams-api-openapi.yml
- filename: flipletters-com-workspaces-api-openapi.yml
  format: yaml
  label: FlipLetters Workspaces API
  slug: flipletters-com-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flipletters-com/openapi/flipletters-com-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FlipLetters Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlipLetters secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FlipLetters
provider_slug: flipletters-com
scheme_count: 1
schemes:
- description: Firebase ID token or Studio API key `flk_…`. Keys are created by a signed-in human; they are never self-issued by agents.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flipletters-com-openapi.json
  type: http
slug: flipletters-com-authentication
source_filename: flipletters-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flipletters-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Firebase ID token or Studio API key `flk_…`. Keys are created by a signed-in\n    human; they are never self-issued by agents.\n  sources:\n  - openapi/flipletters-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flipletters-com/authentication/flipletters-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Animation
- Web App
- Split-Flap
- Flip-Dot
- Free
- Premium
---
