---
anonymous_access: false
api_key_in: []
api_specs:
- filename: indieml-app-keys-api-openapi.yml
  format: yaml
  label: indieml-app Keys API
  slug: indieml-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indieml-app/openapi/indieml-app-keys-api-openapi.yml
- filename: indieml-app-score-api-openapi.yml
  format: yaml
  label: indieml-app Score API
  slug: indieml-app-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indieml-app/openapi/indieml-app-score-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Indieml App Authentication
name_suffix: Authentication
oauth_flows: []
overview: indieml-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: indieml-app
provider_slug: indieml-app
scheme_count: 1
schemes:
- description: API key authentication via X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
slug: indieml-app-authentication
source_filename: indieml-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://indieml.app/openapi.json\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key authentication via X-API-Key header.\n"
source_yaml_url: https://artifacts.apis.io/indieml-app/authentication/indieml-app-authentication.yml
summary_line: 1 scheme
tags:
- AI
- NLP
- Text-Analysis
- Machine-Learning
- API
---
