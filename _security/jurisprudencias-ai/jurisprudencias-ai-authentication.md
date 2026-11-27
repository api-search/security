---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jurisprudencias-ai-courts-api-openapi.yml
  format: yaml
  label: Jurisprudências.ai Courts API
  slug: jurisprudencias-ai-courts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jurisprudencias-ai/openapi/jurisprudencias-ai-courts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Jurisprudências.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jurisprudências.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Jurisprudências.ai
provider_slug: jurisprudencias-ai
scheme_count: 1
schemes:
- description: Token de API com prefixo jur_. Obtenha em https://jurisprudencias.ai/api-tokens
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/jurisprudencias-ai-openapi.json
  type: http
slug: jurisprudencias-ai-authentication
source_filename: jurisprudencias-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/jurisprudencias-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Token de API com prefixo jur_. Obtenha em https://jurisprudencias.ai/api-tokens\n  sources:\n  - openapi/jurisprudencias-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/jurisprudencias-ai/authentication/jurisprudencias-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
