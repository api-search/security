---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Encurate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Encurate declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Encurate
provider_slug: encurate
scheme_count: 2
schemes:
- applies_to:
  - Encurate Keto Diet API
  - Encurate AirplanesDB API
  - Encurate CatBreedDB API
  - Encurate DogBreedDB API
  - Encurate Weed Strain API
  description: RapidAPI subscription key issued to the consumer, not to Encurate. Required on every request to every Encurate dataset API.
  evidence: HTTP 401 {"message":"Invalid API key. Go to https://docs.rapidapi.com/docs/keys for more info."} from https://keto-diet.p.rapidapi.com/ on 2026-09-06
  in: header
  name: RapidAPIKey
  parameterName: X-RapidAPI-Key
  type: apiKey
- applies_to:
  - Encurate Keto Diet API
  - Encurate AirplanesDB API
  - Encurate CatBreedDB API
  - Encurate DogBreedDB API
  - Encurate Weed Strain API
  description: RapidAPI proxy routing header naming the target API host, e.g. keto-diet.p.rapidapi.com. Required alongside X-RapidAPI-Key.
  evidence: RapidAPI proxy contract; the listing pages route through <api>.p.rapidapi.com
  in: header
  name: RapidAPIHost
  parameterName: X-RapidAPI-Host
  type: apiKey
slug: encurate-authentication
source_filename: encurate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource:\n- https://rapidapi.com/encurateapi-api/api/keto-diet (HTTP 200)\n- live probe https://keto-diet.p.rapidapi.com/ -> HTTP 401 {\"message\":\"Invalid API key...\"}\n- live probe https://encurate.app/meta/keto/ -> HTTP 401 {\"detail\":\"Authentication credentials were not provided.\"}\ndocs: https://docs.rapidapi.com/docs/keys\nnote: Encurate publishes no authentication documentation of its own. All five dataset APIs are consumed through\n  the RapidAPI marketplace proxy, so the auth contract is RapidAPI's standard two-header API-key scheme. The origin\n  behind the proxy, https://encurate.app/meta/<project>/, is a Django REST Framework service that returns 401 with\n  a DRF-shaped body to anonymous callers; it is not documented for direct public use.\nsummary:\n  schemes: 2\n  oauth2: false\n  openid_connect: false\n  mtls: false\n  api_key: true\n  scopes_documented: false\nschemes:\n- name: RapidAPIKey\n  type: apiKey\n  in:\
  \ header\n  parameterName: X-RapidAPI-Key\n  description: RapidAPI subscription key issued to the consumer, not to Encurate. Required on every request to every\n    Encurate dataset API.\n  applies_to:\n  - Encurate Keto Diet API\n  - Encurate AirplanesDB API\n  - Encurate CatBreedDB API\n  - Encurate DogBreedDB API\n  - Encurate Weed Strain API\n  evidence: HTTP 401 {\"message\":\"Invalid API key. Go to https://docs.rapidapi.com/docs/keys for more info.\"} from\n    https://keto-diet.p.rapidapi.com/ on 2026-09-06\n- name: RapidAPIHost\n  type: apiKey\n  in: header\n  parameterName: X-RapidAPI-Host\n  description: RapidAPI proxy routing header naming the target API host, e.g. keto-diet.p.rapidapi.com. Required\n    alongside X-RapidAPI-Key.\n  applies_to:\n  - Encurate Keto Diet API\n  - Encurate AirplanesDB API\n  - Encurate CatBreedDB API\n  - Encurate DogBreedDB API\n  - Encurate Weed Strain API\n  evidence: RapidAPI proxy contract; the listing pages route through <api>.p.rapidapi.com\n\
  origin:\n  host: encurate.app\n  base: https://encurate.app/meta/keto/\n  framework: Django REST Framework (inferred from the 401 response envelope)\n  status: 401\n  body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n  note: 'Auth-gated and undocumented. No public schema endpoint: /api/schema/, /schema/, /swagger.json, /redoc/,\n    /openapi/ and /docs/ all returned 404 on 2026-09-06.'\ngaps:\n- No first-party authentication page on encurate.app.\n- No OAuth 2.0 or OpenID Connect surface on any host.\n- No scopes or permissions model published — the key is all-or-nothing per subscription.\n- No key-rotation, expiry or revocation policy published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/encurate/refs/heads/main/authentication/encurate-authentication.yml
summary_line: 2 schemes
tags:
- Diet
- Food
- Keto
- Nutrition
- Recipes
- Health
- Fitness
- Datasets
- Reference Data
- Content Management
- Mobile
- Animals
- Aviation
- Cannabis
- RapidAPI
---
