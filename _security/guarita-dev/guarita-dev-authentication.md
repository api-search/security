---
anonymous_access: false
api_key_in: []
api_specs:
- filename: guarita-dev-apps-api-openapi.yml
  format: yaml
  label: Guarita Apps API
  slug: guarita-dev-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-apps-api-openapi.yml
- filename: guarita-dev-conta-api-openapi.yml
  format: yaml
  label: Guarita Conta API
  slug: guarita-dev-conta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-conta-api-openapi.yml
- filename: guarita-dev-relat-rio-api-openapi.yml
  format: yaml
  label: Guarita Relatório API
  slug: guarita-dev-relat-rio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-relat-rio-api-openapi.yml
- filename: guarita-dev-rondas-api-openapi.yml
  format: yaml
  label: Guarita Rondas API
  slug: guarita-dev-rondas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guarita-dev/openapi/guarita-dev-rondas-api-openapi.yml
auth_types: []
description: Authentication uses an API key prefixed with gsk_ sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Guarita Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guarita declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Guarita
provider_slug: guarita-dev
scheme_count: 1
schemes:
- evidence: Toda chamada leva a chave no header Authorization , esquema Bearer .
  header: Authorization
  how_to_obtain: Create a key in Configurações → Desenvolvedores; the secret appears once and is used as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: guarita-dev-authentication
source_filename: guarita-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://www.guarita.dev/docs/api/authentication
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.guarita.dev/docs/api/authentication\nsources:\n- https://www.guarita.dev/docs/api/authentication\n- https://www.guarita.dev/docs/integrations/lovable\n- https://www.guarita.dev/docs/api/quickstart\ndescription: Authentication uses an API key prefixed with gsk_ sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Toda chamada leva a chave no header Authorization , esquema Bearer .\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Configurações → Desenvolvedores; the secret appears once and is used as the Bearer token.\ndocs: https://www.guarita.dev/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/guarita-dev/authentication/guarita-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
