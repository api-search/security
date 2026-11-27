---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: boletinclaro-es-boletines-api-openapi.yml
  format: yaml
  label: Boletín Claro Boletines API
  slug: boletinclaro-es-boletines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-boletines-api-openapi.yml
- filename: boletinclaro-es-c-digos-api-openapi.yml
  format: yaml
  label: Boletín Claro Códigos API
  slug: boletinclaro-es-c-digos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-c-digos-api-openapi.yml
- filename: boletinclaro-es-dinero-p-blico-api-openapi.yml
  format: yaml
  label: Boletín Claro Dinero público API
  slug: boletinclaro-es-dinero-p-blico-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-dinero-p-blico-api-openapi.yml
- filename: boletinclaro-es-empresas-api-openapi.yml
  format: yaml
  label: Boletín Claro Empresas API
  slug: boletinclaro-es-empresas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-empresas-api-openapi.yml
- filename: boletinclaro-es-referencia-api-openapi.yml
  format: yaml
  label: Boletín Claro Referencia API
  slug: boletinclaro-es-referencia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boletinclaro-es/openapi/boletinclaro-es-referencia-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Boletín Claro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Boletín Claro secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Boletín Claro
provider_slug: boletinclaro-es
scheme_count: 2
schemes:
- description: Obligatoria para datos. Gratis 100, Individual 500, Pro 2.000, Mega 15.000 créditos/mes en el saldo de API, independiente del de la aplicación (en Gratis, Individual y Pro, saldo del workspace compartido con MCP y la web). Mega añade 1.500 créditos al día y 500 llamadas de cinco créditos al mes por saldo. Consultas sencillas 1; empresas 5. Gratis admite cinco perfiles/mes. Trial tiene el cupo Grat
  name: claveAPI
  scheme: bearer
  sources:
  - openapi/boletinclaro-es-openapi.json
  type: http
- description: Clave del workspace, disponible también en Gratis.
  in: header
  name: claveCabecera
  parameter: X-API-Key
  sources:
  - openapi/boletinclaro-es-openapi.json
  type: apiKey
slug: boletinclaro-es-authentication
source_filename: boletinclaro-es-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/boletinclaro-es-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: claveAPI\n  type: http\n  scheme: bearer\n  description: Obligatoria para datos. Gratis 100, Individual 500, Pro 2.000, Mega 15.000 créditos/mes\n    en el saldo de API, independiente del de la aplicación (en Gratis, Individual y Pro, saldo\n    del workspace compartido con MCP y la web). Mega añade 1.500 créditos al día y 500 llamadas\n    de cinco créditos al mes por saldo. Consultas sencillas 1; empresas 5. Gratis admite cinco\n    perfiles/mes. Trial tiene el cupo Grat\n  sources:\n  - openapi/boletinclaro-es-openapi.json\n- name: claveCabecera\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Clave del workspace, disponible también en Gratis.\n  sources:\n  - openapi/boletinclaro-es-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/boletinclaro-es/authentication/boletinclaro-es-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Software-as-a-Service
- Alerts
- Spain
- Government
---
