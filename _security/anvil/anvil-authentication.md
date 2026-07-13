---
api_key_in: []
api_specs:
- filename: anvil-pdf-filling-api-openapi.yml
  format: yaml
  label: Anvil PDF Filling API
  slug: pdf-filling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anvil/refs/heads/main/openapi/anvil-pdf-filling-api-openapi.yml
- filename: anvil-pdf-generation-api-openapi.yml
  format: yaml
  label: Anvil PDF Generation API
  slug: pdf-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anvil/refs/heads/main/openapi/anvil-pdf-generation-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Anvil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anvil secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anvil
provider_slug: anvil
scheme_count: 1
schemes:
- description: HTTP Basic Auth using your Anvil API key as the username and an empty string as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/anvil-pdf-filling-api-openapi.yml
  - openapi/anvil-pdf-generation-api-openapi.yml
  type: http
slug: anvil-authentication
source_filename: anvil-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anvil-pdf-filling-api-openapi.yml, openapi/anvil-pdf-generation-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using your Anvil API key as the username and an empty string\n    as the password.\n  sources:\n  - openapi/anvil-pdf-filling-api-openapi.yml\n  - openapi/anvil-pdf-generation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anvil/refs/heads/main/authentication/anvil-authentication.yml
summary_line: http · 1 scheme
tags:
- PDF
- PDF Filling
- PDF Generation
- E-Signatures
- Document Automation
- OCR
- Document AI
- GraphQL
- REST
- Workflows
- Web Forms
- Paperwork Automation
---
