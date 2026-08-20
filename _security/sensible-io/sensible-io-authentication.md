---
api_key_in: []
api_specs:
- filename: sensible-io-account-api-openapi.yml
  format: yaml
  label: Sensible Account API
  slug: sensible-io-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-account-api-openapi.yml
- filename: sensible-io-classify-api-openapi.yml
  format: yaml
  label: Sensible Classify API
  slug: sensible-io-classify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-classify-api-openapi.yml
- filename: sensible-io-configs-api-openapi.yml
  format: yaml
  label: Sensible Configs API
  slug: sensible-io-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-configs-api-openapi.yml
- filename: sensible-io-document-types-api-openapi.yml
  format: yaml
  label: Sensible Document Types API
  slug: sensible-io-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-document-types-api-openapi.yml
- filename: sensible-io-documents-api-openapi.yml
  format: yaml
  label: Sensible Documents API
  slug: sensible-io-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-documents-api-openapi.yml
- filename: sensible-io-extract-api-openapi.yml
  format: yaml
  label: Sensible Extract API
  slug: sensible-io-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-extract-api-openapi.yml
- filename: sensible-io-reference-documents-api-openapi.yml
  format: yaml
  label: Sensible Reference Documents API
  slug: sensible-io-reference-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-reference-documents-api-openapi.yml
- filename: sensible-io-upload-api-openapi.yml
  format: yaml
  label: Sensible Upload API
  slug: sensible-io-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/openapi/sensible-io-upload-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sensible Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sensible secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sensible
provider_slug: sensible-io
scheme_count: 1
schemes:
- bearerFormat: API Key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sensible-io-openapi.yml
  type: http
slug: sensible-io-authentication
source_filename: sensible-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sensible-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  sources:\n  - openapi/sensible-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensible-io/refs/heads/main/authentication/sensible-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Document AI
- IDP
- Extraction
- LLM
- SenseML
- PDF
---
