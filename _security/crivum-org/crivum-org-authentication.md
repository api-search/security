---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crivum-org-avaliacoes-api-openapi.yml
  format: yaml
  label: Crivum Avaliacoes API
  slug: crivum-org-avaliacoes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-avaliacoes-api-openapi.yml
- filename: crivum-org-criterios-api-openapi.yml
  format: yaml
  label: Crivum Criterios API
  slug: crivum-org-criterios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-criterios-api-openapi.yml
- filename: crivum-org-records-api-openapi.yml
  format: yaml
  label: Crivum Records API
  slug: crivum-org-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-records-api-openapi.yml
- filename: crivum-org-saldo-api-openapi.yml
  format: yaml
  label: Crivum Saldo API
  slug: crivum-org-saldo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-saldo-api-openapi.yml
- filename: crivum-org-triagem-api-openapi.yml
  format: yaml
  label: Crivum Triagem API
  slug: crivum-org-triagem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-triagem-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crivum Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crivum secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crivum
provider_slug: crivum-org
scheme_count: 1
schemes:
- description: 'Chave de API da conta, enviada como Authorization: Bearer <chave>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/crivum-org-openapi.json
  type: http
slug: crivum-org-authentication
source_filename: crivum-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/crivum-org-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Chave de API da conta, enviada como Authorization: Bearer <chave>.'\n  sources:\n  - openapi/crivum-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/crivum-org/authentication/crivum-org-authentication.yml
summary_line: http · 1 scheme
tags:
- Platform
- Evaluation
- Publishing
- Artificial Intelligence
- Portuguese
---
