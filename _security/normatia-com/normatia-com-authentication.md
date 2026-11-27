---
anonymous_access: false
api_key_in: []
api_specs:
- filename: normatia-com-capas-y-cobertura-api-openapi.yml
  format: yaml
  label: Normatia Capas y cobertura API
  slug: normatia-com-capas-y-cobertura-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-capas-y-cobertura-api-openapi.yml
- filename: normatia-com-comprobaciones-api-openapi.yml
  format: yaml
  label: Normatia Comprobaciones API
  slug: normatia-com-comprobaciones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-comprobaciones-api-openapi.yml
- filename: normatia-com-consultas-api-openapi.yml
  format: yaml
  label: Normatia Consultas API
  slug: normatia-com-consultas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-consultas-api-openapi.yml
- filename: normatia-com-cuenta-api-openapi.yml
  format: yaml
  label: Normatia Cuenta API
  slug: normatia-com-cuenta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-cuenta-api-openapi.yml
- filename: normatia-com-entorno-de-pruebas-api-openapi.yml
  format: yaml
  label: Normatia Entorno de pruebas API
  slug: normatia-com-entorno-de-pruebas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-entorno-de-pruebas-api-openapi.yml
- filename: normatia-com-municipios-api-openapi.yml
  format: yaml
  label: Normatia Municipios API
  slug: normatia-com-municipios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-municipios-api-openapi.yml
- filename: normatia-com-normativa-anterior-api-openapi.yml
  format: yaml
  label: Normatia Normativa (anterior) API
  slug: normatia-com-normativa-anterior-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-normativa-anterior-api-openapi.yml
- filename: normatia-com-normativa-api-openapi.yml
  format: yaml
  label: Normatia Normativa API
  slug: normatia-com-normativa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-normativa-api-openapi.yml
- filename: normatia-com-parcelas-api-openapi.yml
  format: yaml
  label: Normatia Parcelas API
  slug: normatia-com-parcelas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-parcelas-api-openapi.yml
- filename: normatia-com-proyectos-api-openapi.yml
  format: yaml
  label: Normatia Proyectos API
  slug: normatia-com-proyectos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-proyectos-api-openapi.yml
- filename: normatia-com-territorio-anterior-api-openapi.yml
  format: yaml
  label: Normatia Territorio (anterior) API
  slug: normatia-com-territorio-anterior-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/normatia-com/openapi/normatia-com-territorio-anterior-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Normatia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Normatia declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Normatia
provider_slug: normatia-com
scheme_count: 1
schemes:
- evidence: 'Todos los endpoints piden una clave de API en la cabecera Authorization , con el esquema Bearer : Authorization: Bearer sk-normatia-...'
  header: Authorization
  how_to_obtain: Se crean en normatia.com, en Mi cuenta, apartado Claves API, con el botón Nueva clave o, las de prueba, Clave de prueba.
  location: header
  name: API Key
  type: http-bearer
slug: normatia-com-authentication
source_filename: normatia-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.normatia.com/api-reference/authentication/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.normatia.com/api-reference/authentication/\nsources:\n- https://docs.normatia.com/api-reference/authentication/\ndescription: Authentication schemes as published on the page.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Todos los endpoints piden una clave de API en la cabecera Authorization , con el esquema Bearer : Authorization: Bearer sk-normatia-...'\n  location: header\n  header: Authorization\n  how_to_obtain: Se crean en normatia.com, en Mi cuenta, apartado Claves API, con el botón Nueva clave o, las de prueba, Clave de prueba.\nnote: No OAuth2 or other authentication schemes are described on the page.\ndocs: https://docs.normatia.com/api-reference/authentication/\n"
source_yaml_url: https://artifacts.apis.io/normatia-com/authentication/normatia-com-authentication.yml
summary_line: 1 scheme
tags:
- Architecture
- Engineering
- Construction
- Regulatory
- Artificial Intelligence
---
