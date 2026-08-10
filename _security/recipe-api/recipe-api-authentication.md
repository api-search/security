---
api_key_in: []
api_specs:
- filename: recipe-api-discovery-api-openapi.yml
  format: yaml
  label: Recipe API Discovery API
  slug: recipe-api-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-discovery-api-openapi.yml
- filename: recipe-api-image-generation-api-openapi.yml
  format: yaml
  label: Recipe API Image Generation API
  slug: recipe-api-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-image-generation-api-openapi.yml
- filename: recipe-api-ingredients-api-openapi.yml
  format: yaml
  label: Recipe API Ingredients API
  slug: recipe-api-ingredients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-ingredients-api-openapi.yml
- filename: recipe-api-public-api-openapi.yml
  format: yaml
  label: Recipe API Public API
  slug: recipe-api-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-public-api-openapi.yml
- filename: recipe-api-recipes-api-openapi.yml
  format: yaml
  label: Recipe API Recipes API
  slug: recipe-api-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/openapi/recipe-api-recipes-api-openapi.yml
auth_types: []
description: API key in a header. Notably the API also exposes a keyless quick-start endpoint, so a developer or an agent can make a real call before signing up.
kind: authentication
layout: security
method: derived
name: Recipe Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recipe API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Recipe API
provider_slug: recipe-api
scheme_count: 1
schemes:
- description: API key issued on signup.
  format: rapi_<key>
  id: ApiKeyAuth
  in: header
  name: X-API-Key
  type: apiKey
slug: recipe-api-authentication
source_filename: recipe-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-03'\nmethod: derived\nstatus: published\nsource: openapi/recipe-api-openapi.json\ndescription: API key in a header. Notably the API also exposes a keyless quick-start\n  endpoint, so a developer or an agent can make a real call before signing up.\nverified: '2026-08-03'\nevidence:\n- url: https://recipe-api.com/openapi.json\n  status: 200\n  note: securitySchemes read from the published spec\n- url: https://recipe-api.com/api/v1/dinner\n  status: 200\n  note: documented keyless quick-start call\nschemes:\n- id: ApiKeyAuth\n  type: apiKey\n  in: header\n  name: X-API-Key\n  format: rapi_<key>\n  description: API key issued on signup.\nkeyless_access:\n  available: true\n  endpoint: https://recipe-api.com/api/v1/dinner\n  note: Documented in the spec description as a no-key quick start.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recipe-api/refs/heads/main/authentication/recipe-api-authentication.yml
summary_line: 1 scheme
tags:
- Recipes
- Food
- Nutrition
- Ingredients
- Data
- Generative AI
- MCP
- Agents
---
