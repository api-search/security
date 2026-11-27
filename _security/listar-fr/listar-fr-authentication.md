---
anonymous_access: false
api_key_in: []
api_specs:
- filename: listar-fr-api-keys-api-openapi.yml
  format: yaml
  label: Listar API Keys API
  slug: listar-fr-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-api-keys-api-openapi.yml
- filename: listar-fr-company-enrichment-api-openapi.yml
  format: yaml
  label: Listar Company Enrichment API
  slug: listar-fr-company-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-company-enrichment-api-openapi.yml
- filename: listar-fr-company-search-api-openapi.yml
  format: yaml
  label: Listar Company Search API
  slug: listar-fr-company-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-company-search-api-openapi.yml
- filename: listar-fr-credit-api-openapi.yml
  format: yaml
  label: Listar Credit API
  slug: listar-fr-credit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-credit-api-openapi.yml
- filename: listar-fr-people-search-api-openapi.yml
  format: yaml
  label: Listar People Search API
  slug: listar-fr-people-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-people-search-api-openapi.yml
- filename: listar-fr-person-enrichment-api-openapi.yml
  format: yaml
  label: Listar Person Enrichment API
  slug: listar-fr-person-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-person-enrichment-api-openapi.yml
- filename: listar-fr-webhooks-api-openapi.yml
  format: yaml
  label: Listar Webhooks API
  slug: listar-fr-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listar-fr/openapi/listar-fr-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Listar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Listar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Listar
provider_slug: listar-fr
scheme_count: 1
schemes:
- description: 'Clé API Listar. En-tête : `Authorization: Bearer sk_live_...`'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/listar-fr-openapi.yml
  type: http
slug: listar-fr-authentication
source_filename: listar-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/listar-fr-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'Clé API Listar. En-tête : `Authorization: Bearer sk_live_...`'\n  sources:\n  - openapi/listar-fr-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/listar-fr/authentication/listar-fr-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B
- Data Enrichment
- Sales
- Marketing
- Data
---
