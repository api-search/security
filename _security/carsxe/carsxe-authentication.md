---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Carsxe Authentication
name_suffix: Authentication
oauth_flows: []
overview: CarsXE secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CarsXE
provider_slug: carsxe
scheme_count: 1
schemes:
- description: CarsXE API key from https://api.carsxe.com/dashboard
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/carsxe-openapi.yml
  type: apiKey
slug: carsxe-authentication
source_filename: carsxe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/carsxe-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: CarsXE API key from https://api.carsxe.com/dashboard\n  sources:\n  - openapi/carsxe-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/authentication/carsxe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Automotive
- Vehicles
- VIN
- Vehicle Data
- License Plate
- OCR
- Automobiles
---
