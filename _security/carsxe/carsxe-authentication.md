---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: carsxe-specifications-api-openapi.yml
  format: yaml
  label: CarsXE Specifications API
  slug: carsxe-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-specifications-api-openapi.yml
- filename: carsxe-market-value-api-openapi.yml
  format: yaml
  label: CarsXE Market Value API
  slug: carsxe-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-market-value-api-openapi.yml
- filename: carsxe-plate-api-openapi.yml
  format: yaml
  label: CarsXE Plate Decoder API
  slug: carsxe-plate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-plate-api-openapi.yml
- filename: carsxe-recalls-api-openapi.yml
  format: yaml
  label: CarsXE Recalls API
  slug: carsxe-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recalls-api-openapi.yml
- filename: carsxe-history-api-openapi.yml
  format: yaml
  label: CarsXE History API
  slug: carsxe-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-history-api-openapi.yml
- filename: carsxe-images-api-openapi.yml
  format: yaml
  label: CarsXE Images API
  slug: carsxe-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-images-api-openapi.yml
- filename: carsxe-recognition-api-openapi.yml
  format: yaml
  label: CarsXE Recognition API
  slug: carsxe-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recognition-api-openapi.yml
- filename: carsxe-year-make-model-api-openapi.yml
  format: yaml
  label: CarsXE Year Make Model API
  slug: carsxe-year-make-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-year-make-model-api-openapi.yml
- filename: carsxe-lien-theft-api-openapi.yml
  format: yaml
  label: CarsXE Lien & Theft API
  slug: carsxe-lien-theft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-lien-theft-api-openapi.yml
- filename: carsxe-auth-api-openapi.yml
  format: yaml
  label: CarsXE Auth API
  slug: carsxe-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-auth-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Carsxe Authentication
name_suffix: Authentication
oauth_flows: []
overview: CarsXE secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CarsXE
provider_slug: carsxe
scheme_count: 3
schemes:
- description: CarsXE API key from https://api.carsxe.com/dashboard
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/carsxe-auth-api-openapi.yml
  - openapi/carsxe-history-api-openapi.yml
  - openapi/carsxe-images-api-openapi.yml
  - openapi/carsxe-lien-theft-api-openapi.yml
  - openapi/carsxe-market-value-api-openapi.yml
  - openapi/carsxe-plate-api-openapi.yml
  - openapi/carsxe-recalls-api-openapi.yml
  - openapi/carsxe-recognition-api-openapi.yml
  - openapi/carsxe-specifications-api-openapi.yml
  - openapi/carsxe-year-make-model-api-openapi.yml
  type: apiKey
- description: x402 payment proof for supported operations. Start without a CarsXE key to receive HTTP 402 payment requirements, then retry the identical request with the payment header produced by your x402 client. CarsXE also accepts the legacy X-PAYMENT header.
  in: header
  name: X402Payment
  parameter: PAYMENT-SIGNATURE
  sources:
  - openapi/carsxe-history-api-openapi.yml
  - openapi/carsxe-images-api-openapi.yml
  - openapi/carsxe-lien-theft-api-openapi.yml
  - openapi/carsxe-market-value-api-openapi.yml
  - openapi/carsxe-plate-api-openapi.yml
  - openapi/carsxe-recalls-api-openapi.yml
  - openapi/carsxe-recognition-api-openapi.yml
  - openapi/carsxe-specifications-api-openapi.yml
  - openapi/carsxe-year-make-model-api-openapi.yml
  type: apiKey
- description: Batch-scoped token returned by an x402 Recalls Batch submission.
  in: header
  name: RecallsBatchToken
  parameter: X-CarsXE-Batch-Token
  sources:
  - openapi/carsxe-recalls-api-openapi.yml
  type: apiKey
slug: carsxe-authentication
source_filename: carsxe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: openapi/carsxe-auth-api-openapi.yml, openapi/carsxe-history-api-openapi.yml, openapi/carsxe-images-api-openapi.yml,\n  openapi/carsxe-lien-theft-api-openapi.yml, openapi/carsxe-market-value-api-openapi.yml, openapi/carsxe-plate-api-openapi.yml,\n  openapi/carsxe-recalls-api-openapi.yml, openapi/carsxe-recognition-api-openapi.yml, openapi/carsxe-specifications-api-openapi.yml,\n  openapi/carsxe-year-make-model-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: CarsXE API key from https://api.carsxe.com/dashboard\n  sources:\n  - openapi/carsxe-auth-api-openapi.yml\n  - openapi/carsxe-history-api-openapi.yml\n  - openapi/carsxe-images-api-openapi.yml\n  - openapi/carsxe-lien-theft-api-openapi.yml\n  - openapi/carsxe-market-value-api-openapi.yml\n  - openapi/carsxe-plate-api-openapi.yml\n  - openapi/carsxe-recalls-api-openapi.yml\n\
  \  - openapi/carsxe-recognition-api-openapi.yml\n  - openapi/carsxe-specifications-api-openapi.yml\n  - openapi/carsxe-year-make-model-api-openapi.yml\n- name: X402Payment\n  type: apiKey\n  in: header\n  parameter: PAYMENT-SIGNATURE\n  description: x402 payment proof for supported operations. Start without a CarsXE key to receive\n    HTTP 402 payment requirements, then retry the identical request with the payment header\n    produced by your x402 client. CarsXE also accepts the legacy X-PAYMENT header.\n  sources:\n  - openapi/carsxe-history-api-openapi.yml\n  - openapi/carsxe-images-api-openapi.yml\n  - openapi/carsxe-lien-theft-api-openapi.yml\n  - openapi/carsxe-market-value-api-openapi.yml\n  - openapi/carsxe-plate-api-openapi.yml\n  - openapi/carsxe-recalls-api-openapi.yml\n  - openapi/carsxe-recognition-api-openapi.yml\n  - openapi/carsxe-specifications-api-openapi.yml\n  - openapi/carsxe-year-make-model-api-openapi.yml\n- name: RecallsBatchToken\n  type: apiKey\n  in: header\n\
  \  parameter: X-CarsXE-Batch-Token\n  description: Batch-scoped token returned by an x402 Recalls Batch submission.\n  sources:\n  - openapi/carsxe-recalls-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/authentication/carsxe-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Automotive
- Vehicles
- VIN
- Vehicle Data
- License Plate
- OCR
- Automobiles
- Recalls
- Market Value
- Vehicle History
- Model Context Protocol
- Agents
---
