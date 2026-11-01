---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: animalchecklist-com-account-api-openapi.yml
  format: yaml
  label: animalchecklist-com Account API
  slug: animalchecklist-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-account-api-openapi.yml
- filename: animalchecklist-com-catalogue-api-openapi.yml
  format: yaml
  label: animalchecklist-com Catalogue API
  slug: animalchecklist-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-catalogue-api-openapi.yml
- filename: animalchecklist-com-diagnostics-api-openapi.yml
  format: yaml
  label: animalchecklist-com Diagnostics API
  slug: animalchecklist-com-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-diagnostics-api-openapi.yml
- filename: animalchecklist-com-leaderboard-api-openapi.yml
  format: yaml
  label: animalchecklist-com Leaderboard API
  slug: animalchecklist-com-leaderboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-leaderboard-api-openapi.yml
- filename: animalchecklist-com-quiz-api-openapi.yml
  format: yaml
  label: animalchecklist-com Quiz API
  slug: animalchecklist-com-quiz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-quiz-api-openapi.yml
- filename: animalchecklist-com-recognition-api-openapi.yml
  format: yaml
  label: animalchecklist-com Recognition API
  slug: animalchecklist-com-recognition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-recognition-api-openapi.yml
- filename: animalchecklist-com-sightings-api-openapi.yml
  format: yaml
  label: animalchecklist-com Sightings API
  slug: animalchecklist-com-sightings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/animalchecklist-com/openapi/animalchecklist-com-sightings-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Animalchecklist Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: animalchecklist-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: animalchecklist-com
provider_slug: animalchecklist-com
scheme_count: 2
schemes:
- bearerFormat: AC-XXXX-XXXX-XXXX-XXXX
  description: The person's anonymous sync code. It grants read and write access to that one checklist and nothing else. An agent uses a code only when the person supplied it.
  name: syncCode
  scheme: bearer
  sources:
  - openapi/animalchecklist-com-openapi.json
  type: http
- description: HttpOnly session set after a magic link or passkey sign-in.
  in: cookie
  name: sessionCookie
  parameter: ac_session
  sources:
  - openapi/animalchecklist-com-openapi.json
  type: apiKey
slug: animalchecklist-com-authentication
source_filename: animalchecklist-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/animalchecklist-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: syncCode\n  type: http\n  scheme: bearer\n  bearerFormat: AC-XXXX-XXXX-XXXX-XXXX\n  description: The person's anonymous sync code. It grants read and write access to that one\n    checklist and nothing else. An agent uses a code only when the person supplied it.\n  sources:\n  - openapi/animalchecklist-com-openapi.json\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: ac_session\n  description: HttpOnly session set after a magic link or passkey sign-in.\n  sources:\n  - openapi/animalchecklist-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/animalchecklist-com/authentication/animalchecklist-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Animals
- Checklist
- MobileApp
- Free
---
