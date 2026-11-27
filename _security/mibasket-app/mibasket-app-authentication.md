---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: mibasket-app-estad-sticas-de-partidos-api-openapi.yml
  format: yaml
  label: Mi Basket Estadísticas de partidos API
  slug: mibasket-app-estad-sticas-de-partidos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mibasket-app/openapi/mibasket-app-estad-sticas-de-partidos-api-openapi.yml
- filename: mibasket-app-partidos-api-openapi.yml
  format: yaml
  label: Mi Basket Partidos API
  slug: mibasket-app-partidos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mibasket-app/openapi/mibasket-app-partidos-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Mi Basket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mi Basket secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mi Basket
provider_slug: mibasket-app
scheme_count: 2
schemes:
- bearerFormat: mbk_...
  description: Tu clave, en el encabezado `Authorization`.
  name: Encabezado
  scheme: bearer
  sources:
  - openapi/mibasket-app-openapi.json
  type: http
- description: 'Tu clave, en el link: para herramientas sin encabezados.'
  in: query
  name: Link
  parameter: key
  sources:
  - openapi/mibasket-app-openapi.json
  type: apiKey
slug: mibasket-app-authentication
source_filename: mibasket-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mibasket-app-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: Encabezado\n  type: http\n  scheme: bearer\n  bearerFormat: mbk_...\n  description: Tu clave, en el encabezado `Authorization`.\n  sources:\n  - openapi/mibasket-app-openapi.json\n- name: Link\n  type: apiKey\n  in: query\n  parameter: key\n  description: 'Tu clave, en el link: para herramientas sin encabezados.'\n  sources:\n  - openapi/mibasket-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mibasket-app/authentication/mibasket-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Sports
- Basketball
- Uruguay
- Live Data
- Non-Profit
---
