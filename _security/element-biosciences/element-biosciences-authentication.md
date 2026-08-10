---
api_key_in:
- header
api_specs:
- filename: element-biosciences-authservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Auth Service API
  slug: element-biosciences-authservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-authservice-api-openapi.yml
- filename: element-biosciences-executionservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Execution Service API
  slug: element-biosciences-executionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-executionservice-api-openapi.yml
- filename: element-biosciences-instrumentservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Instrument Service API
  slug: element-biosciences-instrumentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-instrumentservice-api-openapi.yml
- filename: element-biosciences-runservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Run Service API
  slug: element-biosciences-runservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-runservice-api-openapi.yml
- filename: element-biosciences-storageconnectionservice-api-openapi.yml
  format: yaml
  label: Element Biosciences Storage Connection Service API
  slug: element-biosciences-storageconnectionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/openapi/element-biosciences-storageconnectionservice-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Element Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Element Biosciences secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Element Biosciences
provider_slug: element-biosciences
scheme_count: 1
schemes:
- description: API key obtained from the Element Biosciences Cloud console
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/element-biosciences-cloud-api-openapi-original.yml
  type: apiKey
slug: element-biosciences-authentication
source_filename: element-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/element-biosciences-cloud-api-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key obtained from the Element Biosciences Cloud console\n  sources:\n  - openapi/element-biosciences-cloud-api-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/element-biosciences/refs/heads/main/authentication/element-biosciences-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Genomics
- DNA Sequencing
- Life Sciences
- Bioinformatics
- Multiomics
- Laboratory
- Scientific Instruments
- Cloud Storage
- Biotechnology
---
