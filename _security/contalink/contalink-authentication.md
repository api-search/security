---
api_key_in:
- header
api_specs:
- filename: contalink-balanza-de-comprobaci-n-api-openapi.yml
  format: yaml
  label: Contalink Balanza de comprobación API
  slug: contalink-balanza-de-comprobaci-n-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-balanza-de-comprobaci-n-api-openapi.yml
- filename: contalink-cargar-un-documento-fiscal-api-openapi.yml
  format: yaml
  label: Contalink Cargar un documento fiscal API
  slug: contalink-cargar-un-documento-fiscal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-cargar-un-documento-fiscal-api-openapi.yml
- filename: contalink-conciliaci-n-api-openapi.yml
  format: yaml
  label: Contalink Conciliación API
  slug: contalink-conciliaci-n-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-conciliaci-n-api-openapi.yml
- filename: contalink-listado-de-documentos-fiscales-api-openapi.yml
  format: yaml
  label: Contalink Listado de documentos fiscales API
  slug: contalink-listado-de-documentos-fiscales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-listado-de-documentos-fiscales-api-openapi.yml
- filename: contalink-movimientos-bancarios-api-openapi.yml
  format: yaml
  label: Contalink Movimientos bancarios API
  slug: contalink-movimientos-bancarios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-movimientos-bancarios-api-openapi.yml
- filename: contalink-p-lizas-manuales-api-openapi.yml
  format: yaml
  label: Contalink Pólizas manuales API
  slug: contalink-p-lizas-manuales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-p-lizas-manuales-api-openapi.yml
- filename: contalink-saldo-de-una-cuenta-api-openapi.yml
  format: yaml
  label: Contalink Saldo de una cuenta API
  slug: contalink-saldo-de-una-cuenta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-saldo-de-una-cuenta-api-openapi.yml
- filename: contalink-status-de-documentos-fiscales-api-openapi.yml
  format: yaml
  label: Contalink Status de documentos fiscales API
  slug: contalink-status-de-documentos-fiscales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/openapi/contalink-status-de-documentos-fiscales-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Contalink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contalink secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contalink
provider_slug: contalink
scheme_count: 1
schemes:
- description: Llave de API relacionada al usuario que hace la petición.
  in: header
  name: APIKey
  parameter: Authorization
  sources:
  - openapi/contalink-openapi-original.json
  type: apiKey
slug: contalink-authentication
source_filename: contalink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/contalink-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Llave de API relacionada al usuario que hace la petición.\n  sources:\n  - openapi/contalink-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contalink/refs/heads/main/authentication/contalink-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Accounting
- Bookkeeping
- Payroll
- Tax
- Fintech
- Invoicing
- CFDI
- Mexico
- SaaS
---
