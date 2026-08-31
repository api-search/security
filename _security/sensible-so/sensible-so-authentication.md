---
api_key_in: []
api_specs:
- filename: sensible-so-configuration-api-openapi.yml
  format: yaml
  label: sensible-so Configuration API
  slug: sensible-so-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-configuration-api-openapi.yml
- filename: sensible-so-document-api-openapi.yml
  format: yaml
  label: sensible-so Document API
  slug: sensible-so-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-document-api-openapi.yml
- filename: sensible-so-document-type-api-openapi.yml
  format: yaml
  label: sensible-so Document type API
  slug: sensible-so-document-type-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-document-type-api-openapi.yml
- filename: sensible-so-get-excel-from-documents-api-openapi.yml
  format: yaml
  label: sensible-so Get Excel from documents API
  slug: sensible-so-get-excel-from-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-get-excel-from-documents-api-openapi.yml
- filename: sensible-so-portfolio-api-openapi.yml
  format: yaml
  label: sensible-so Portfolio API
  slug: sensible-so-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-portfolio-api-openapi.yml
- filename: sensible-so-reference-document-api-openapi.yml
  format: yaml
  label: sensible-so Reference document API
  slug: sensible-so-reference-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-reference-document-api-openapi.yml
- filename: sensible-so-retrieve-extractions-api-openapi.yml
  format: yaml
  label: sensible-so Retrieve extractions API
  slug: sensible-so-retrieve-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-so/refs/heads/main/openapi/sensible-so-retrieve-extractions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sensible So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sensible
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
