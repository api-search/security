---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: indicadores-ar-adjudicaciones-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Adjudicaciones API
  slug: indicadores-ar-adjudicaciones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-adjudicaciones-api-openapi.yml
- filename: indicadores-ar-busqueda-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Busqueda API
  slug: indicadores-ar-busqueda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-busqueda-api-openapi.yml
- filename: indicadores-ar-busqueda-personas-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Busqueda Personas API
  slug: indicadores-ar-busqueda-personas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-busqueda-personas-api-openapi.yml
- filename: indicadores-ar-convertir-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Convertir API
  slug: indicadores-ar-convertir-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-convertir-api-openapi.yml
- filename: indicadores-ar-creditos-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Creditos API
  slug: indicadores-ar-creditos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-creditos-api-openapi.yml
- filename: indicadores-ar-empresa-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Empresa API
  slug: indicadores-ar-empresa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-empresa-api-openapi.yml
- filename: indicadores-ar-empresas-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Empresas API
  slug: indicadores-ar-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-empresas-api-openapi.yml
- filename: indicadores-ar-importadores-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Importadores API
  slug: indicadores-ar-importadores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-importadores-api-openapi.yml
- filename: indicadores-ar-inflacion-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Inflacion API
  slug: indicadores-ar-inflacion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-inflacion-api-openapi.yml
- filename: indicadores-ar-llamado-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Llamado API
  slug: indicadores-ar-llamado-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-llamado-api-openapi.yml
- filename: indicadores-ar-llamados-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Llamados API
  slug: indicadores-ar-llamados-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-llamados-api-openapi.yml
- filename: indicadores-ar-migracion-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Migracion API
  slug: indicadores-ar-migracion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-migracion-api-openapi.yml
- filename: indicadores-ar-migraciones-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Migraciones API
  slug: indicadores-ar-migraciones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-migraciones-api-openapi.yml
- filename: indicadores-ar-persona-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Persona API
  slug: indicadores-ar-persona-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-persona-api-openapi.yml
- filename: indicadores-ar-seguimientos-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Seguimientos API
  slug: indicadores-ar-seguimientos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-seguimientos-api-openapi.yml
- filename: indicadores-ar-serie-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Serie API
  slug: indicadores-ar-serie-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-serie-api-openapi.yml
- filename: indicadores-ar-series-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Series API
  slug: indicadores-ar-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-series-api-openapi.yml
- filename: indicadores-ar-sugerencias-api-openapi.yml
  format: yaml
  label: Indicadores Argentina Sugerencias API
  slug: indicadores-ar-sugerencias-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indicadores-ar/openapi/indicadores-ar-sugerencias-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Indicadores Argentina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indicadores Argentina secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Indicadores Argentina
provider_slug: indicadores-ar
scheme_count: 1
schemes:
- description: API key creada en https://indicadores.ar/api-empresas
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/indicadores-ar-openapi.json
  - openapi/openapi.json
  type: apiKey
slug: indicadores-ar-authentication
source_filename: indicadores-ar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/indicadores-ar-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key creada en https://indicadores.ar/api-empresas\n  sources:\n  - openapi/indicadores-ar-openapi.json\n  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/indicadores-ar/authentication/indicadores-ar-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Argentina
- Finance
- Company Data
- Public APIs
- Government
---
