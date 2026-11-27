---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lexiel-ai-agenda-api-openapi.yml
  format: yaml
  label: Lexiel Agenda API
  slug: lexiel-ai-agenda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-agenda-api-openapi.yml
- filename: lexiel-ai-anal-tica-api-openapi.yml
  format: yaml
  label: Lexiel Analítica API
  slug: lexiel-ai-anal-tica-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-anal-tica-api-openapi.yml
- filename: lexiel-ai-chat-ia-api-openapi.yml
  format: yaml
  label: Lexiel Chat IA API
  slug: lexiel-ai-chat-ia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-chat-ia-api-openapi.yml
- filename: lexiel-ai-clientes-api-openapi.yml
  format: yaml
  label: Lexiel Clientes API
  slug: lexiel-ai-clientes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-clientes-api-openapi.yml
- filename: lexiel-ai-documentos-api-openapi.yml
  format: yaml
  label: Lexiel Documentos API
  slug: lexiel-ai-documentos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-documentos-api-openapi.yml
- filename: lexiel-ai-expedientes-api-openapi.yml
  format: yaml
  label: Lexiel Expedientes API
  slug: lexiel-ai-expedientes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-expedientes-api-openapi.yml
- filename: lexiel-ai-facturaci-n-api-openapi.yml
  format: yaml
  label: Lexiel Facturación API
  slug: lexiel-ai-facturaci-n-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexiel-ai/openapi/lexiel-ai-facturaci-n-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lexiel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lexiel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lexiel
provider_slug: lexiel-ai
scheme_count: 1
schemes:
- bearerFormat: lx_… (clave de API) o JWT
  description: 'Clave de API (`Authorization: Bearer lx_…`) creada en Ajustes > API, o el JWT de una sesión de Lexiel. Cada operación indica en `x-required-scope` el ámbito que necesita la clave.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/lexiel-ai-openapi.yml
  type: http
slug: lexiel-ai-authentication
source_filename: lexiel-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lexiel-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: lx_… (clave de API) o JWT\n  description: 'Clave de API (`Authorization: Bearer lx_…`) creada en Ajustes > API, o el JWT\n    de una sesión de Lexiel. Cada operación indica en `x-required-scope` el ámbito que necesita\n    la clave.'\n  sources:\n  - openapi/lexiel-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/lexiel-ai/authentication/lexiel-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal Tech
- Artificial Intelligence
- Automation
- Spain
- Latin America
---
