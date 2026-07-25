---
api_key_in:
- header
api_specs:
- filename: highlightly-catalog-api-openapi.yml
  format: yaml
  label: Highlightly Catalog API
  slug: highlightly-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-catalog-api-openapi.yml
- filename: highlightly-highlights-api-openapi.yml
  format: yaml
  label: Highlightly Highlights API
  slug: highlightly-highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-highlights-api-openapi.yml
- filename: highlightly-matches-api-openapi.yml
  format: yaml
  label: Highlightly Matches API
  slug: highlightly-matches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-matches-api-openapi.yml
- filename: highlightly-odds-api-openapi.yml
  format: yaml
  label: Highlightly Odds API
  slug: highlightly-odds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-odds-api-openapi.yml
- filename: highlightly-standings-api-openapi.yml
  format: yaml
  label: Highlightly Standings API
  slug: highlightly-standings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-standings-api-openapi.yml
- filename: highlightly-statistics-api-openapi.yml
  format: yaml
  label: Highlightly Statistics API
  slug: highlightly-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-statistics-api-openapi.yml
- filename: highlightly-teams-api-openapi.yml
  format: yaml
  label: Highlightly Teams API
  slug: highlightly-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/openapi/highlightly-teams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Highlightly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Highlightly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Highlightly
provider_slug: highlightly
scheme_count: 1
schemes:
- description: API key issued by Highlightly. Sent in the x-rapidapi-key header. When calling via RapidAPI, also send x-rapidapi-host with the relevant RapidAPI host (for example sport-highlights-api.p.rapidapi.com).
  in: header
  name: ApiKeyAuth
  parameter: x-rapidapi-key
  sources:
  - openapi/highlightly-openapi.yml
  type: apiKey
slug: highlightly-authentication
source_filename: highlightly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/highlightly-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-rapidapi-key\n  description: API key issued by Highlightly. Sent in the x-rapidapi-key header. When calling\n    via RapidAPI, also send x-rapidapi-host with the relevant RapidAPI host (for example sport-highlights-api.p.rapidapi.com).\n  sources:\n  - openapi/highlightly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highlightly/refs/heads/main/authentication/highlightly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sports
- Sports Data
- Live Scores
- Odds
- Highlights
---
