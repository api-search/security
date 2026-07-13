---
api_key_in:
- header
api_specs:
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Cards API
  slug: pokemon-tcg-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Sets API
  slug: pokemon-tcg-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
- filename: pokemon-tcg-openapi.yml
  format: yaml
  label: Pokémon TCG Metadata API
  slug: pokemon-tcg-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/openapi/pokemon-tcg-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pokemon Tcg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pokémon TCG API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pokémon TCG API
provider_slug: pokemon-tcg
scheme_count: 1
schemes:
- description: Optional API key from the Pokémon TCG Developer Portal (https://dev.pokemontcg.io). Requests without a key still work but are rate limited to 1,000 requests/day (max 30/minute); a free key raises the default limit to 20,000 requests/day.
  in: header
  name: apiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/pokemon-tcg-openapi.yml
  type: apiKey
slug: pokemon-tcg-authentication
source_filename: pokemon-tcg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pokemon-tcg-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Optional API key from the Pokémon TCG Developer Portal (https://dev.pokemontcg.io).\n    Requests without a key still work but are rate limited to 1,000 requests/day (max 30/minute);\n    a free key raises the default limit to 20,000 requests/day.\n  sources:\n  - openapi/pokemon-tcg-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokemon-tcg/refs/heads/main/authentication/pokemon-tcg-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Pokemon
- Trading Cards
- TCG
- Gaming
- Card Games
- Collectibles
- Card Prices
---
