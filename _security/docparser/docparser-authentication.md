---
api_key_in:
- header
- query
api_specs:
- filename: docparser-rest-api-openapi.yml
  format: yaml
  label: Docparser REST API
  slug: docparser-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docparser/refs/heads/main/openapi/docparser-rest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docparser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Docparser secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Docparser
provider_slug: docparser
scheme_count: 3
schemes:
- description: HTTP Basic Authentication. Use your API key as the username and leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/docparser-rest-api-openapi.yml
  type: http
- description: API key passed as a custom request header.
  in: header
  name: apiKeyHeader
  parameter: api_key
  sources:
  - openapi/docparser-rest-api-openapi.yml
  type: apiKey
- description: API key passed as a URL query parameter.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/docparser-rest-api-openapi.yml
  type: apiKey
slug: docparser-authentication
source_filename: docparser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docparser-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. Use your API key as the username and leave the password\n    blank.\n  sources:\n  - openapi/docparser-rest-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: API key passed as a custom request header.\n  sources:\n  - openapi/docparser-rest-api-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a URL query parameter.\n  sources:\n  - openapi/docparser-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docparser/refs/heads/main/authentication/docparser-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Document Parsing
- Data Extraction
- PDF
- OCR
- Document Automation
- Invoices
- Contracts
- REST API
---
