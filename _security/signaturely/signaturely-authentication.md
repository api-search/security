---
api_key_in:
- header
api_specs:
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Signature Requests API
  slug: signaturely-signature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Documents API
  slug: signaturely-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Templates API
  slug: signaturely-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Folders API
  slug: signaturely-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Team API
  slug: signaturely-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely Webhooks API
  slug: signaturely-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
- filename: signaturely-openapi.yml
  format: yaml
  label: Signaturely User API
  slug: signaturely-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/openapi/signaturely-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Signaturely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Signaturely secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Signaturely
provider_slug: signaturely
scheme_count: 1
schemes:
- description: 'API key sent as: Authorization: Api-Key {API_KEY}'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/signaturely-openapi.yml
  type: apiKey
slug: signaturely-authentication
source_filename: signaturely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/signaturely-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key sent as: Authorization: Api-Key {API_KEY}'\n  sources:\n  - openapi/signaturely-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signaturely/refs/heads/main/authentication/signaturely-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Electronic Signature
- eSignature
- Document Signing
- E-Signature API
- Contracts
- Signature Requests
- SaaS
---
