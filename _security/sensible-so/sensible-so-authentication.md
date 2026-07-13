---
api_key_in: []
api_specs:
- filename: sensible-extractions-api-openapi.yml
  format: yaml
  label: Sensible Extractions API
  slug: sensible-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-extractions-api-openapi.yml
- filename: sensible-classification-api-openapi.yml
  format: yaml
  label: Sensible Classification API
  slug: sensible-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-classification-api-openapi.yml
- filename: sensible-document-types-api-openapi.yml
  format: yaml
  label: Sensible Document Types and Configurations API
  slug: sensible-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-document-types-api-openapi.yml
- filename: sensible-reference-documents-api-openapi.yml
  format: yaml
  label: Sensible Reference Documents API
  slug: sensible-reference-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-reference-documents-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sensible So Authentication
name_suffix: Authentication
oauth_flows: []
overview: sensible-so secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: sensible-so
provider_slug: sensible-so
scheme_count: 1
schemes:
- description: Bearer token using a Sensible API key. Create keys at https://app.sensible.so/account/.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sensible-classification-api-openapi.yml
  - openapi/sensible-document-types-api-openapi.yml
  - openapi/sensible-extractions-api-openapi.yml
  - openapi/sensible-reference-documents-api-openapi.yml
  type: http
slug: sensible-so-authentication
source_filename: sensible-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sensible-classification-api-openapi.yml, openapi/sensible-document-types-api-openapi.yml,\n  openapi/sensible-extractions-api-openapi.yml, openapi/sensible-reference-documents-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token using a Sensible API key. Create keys at https://app.sensible.so/account/.\n  sources:\n  - openapi/sensible-classification-api-openapi.yml\n  - openapi/sensible-document-types-api-openapi.yml\n  - openapi/sensible-extractions-api-openapi.yml\n  - openapi/sensible-reference-documents-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/authentication/sensible-so-authentication.yml
summary_line: http · 1 scheme
tags: []
---
