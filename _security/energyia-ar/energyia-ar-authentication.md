---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EnergyIA Authentication
name_suffix: Authentication
oauth_flows: []
overview: EnergyIA declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EnergyIA
provider_slug: energyia-ar
scheme_count: 1
schemes:
- bearerMethodsSupported:
  - header
  description: OAuth2 implicit flow for EnergyIA AR MCP
  flows:
    clientCredentials:
      tokenUrl: https://energyia.ar/oauth/token
  scopesSupported:
  - catalogo
  - vigia
  - mineria
  - oilgas
  - comercio
  - buques
  - rigi
  - oportunidades
  - geo
  - notas
  - mercados
  - combustibles
  - red
  type: oauth2
slug: energyia-ar-authentication
source_filename: energyia-ar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://energyia.ar/.well-known/oauth-protected-resource\nschemes:\n  - type: oauth2\n    description: OAuth2 implicit flow for EnergyIA AR MCP\n    flows:\n      clientCredentials:\n        tokenUrl: https://energyia.ar/oauth/token\n    bearerMethodsSupported:\n      - header\n    scopesSupported:\n      - catalogo\n      - vigia\n      - mineria\n      - oilgas\n      - comercio\n      - buques\n      - rigi\n      - oportunidades\n      - geo\n      - notas\n      - mercados\n      - combustibles\n      - red\n"
source_yaml_url: https://artifacts.apis.io/energyia-ar/authentication/energyia-ar-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Data
- Argentina
- Oil
- Mining
- Artificial Intelligence
---
