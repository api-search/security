---
api_key_in:
- header
api_specs:
- filename: celcoin-annotationcompetencecalendar-api-openapi.yml
  format: yaml
  label: Celcoin AnnotationCompetenceCalendar API
  slug: celcoin-annotationcompetencecalendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-annotationcompetencecalendar-api-openapi.yml
- filename: celcoin-bankcorrespondentagent-api-openapi.yml
  format: yaml
  label: Celcoin BankCorrespondentAgent API
  slug: celcoin-bankcorrespondentagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-bankcorrespondentagent-api-openapi.yml
- filename: celcoin-consignee-api-openapi.yml
  format: yaml
  label: Celcoin Consignee API
  slug: celcoin-consignee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-consignee-api-openapi.yml
- filename: celcoin-files-api-openapi.yml
  format: yaml
  label: Celcoin Files API
  slug: celcoin-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-files-api-openapi.yml
- filename: celcoin-guarantee-api-openapi.yml
  format: yaml
  label: Celcoin Guarantee API
  slug: celcoin-guarantee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-guarantee-api-openapi.yml
- filename: celcoin-legacyguarantee-api-openapi.yml
  format: yaml
  label: Celcoin LegacyGuarantee API
  slug: celcoin-legacyguarantee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-legacyguarantee-api-openapi.yml
- filename: celcoin-legalperson-api-openapi.yml
  format: yaml
  label: Celcoin LegalPerson API
  slug: celcoin-legalperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-legalperson-api-openapi.yml
- filename: celcoin-naturalperson-api-openapi.yml
  format: yaml
  label: Celcoin NaturalPerson API
  slug: celcoin-naturalperson-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-naturalperson-api-openapi.yml
- filename: celcoin-outstandingbalance-api-openapi.yml
  format: yaml
  label: Celcoin OutstandingBalance API
  slug: celcoin-outstandingbalance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-outstandingbalance-api-openapi.yml
- filename: celcoin-proposal-api-openapi.yml
  format: yaml
  label: Celcoin Proposal API
  slug: celcoin-proposal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-proposal-api-openapi.yml
- filename: celcoin-settlement-api-openapi.yml
  format: yaml
  label: Celcoin Settlement API
  slug: celcoin-settlement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-settlement-api-openapi.yml
- filename: celcoin-taggingjourney-api-openapi.yml
  format: yaml
  label: Celcoin TaggingJourney API
  slug: celcoin-taggingjourney-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-taggingjourney-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Celcoin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celcoin secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Celcoin
provider_slug: celcoin
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Autenticação utilizando JTW Bearer Token
  name: Bearer
  scheme: Bearer
  sources:
  - openapi/celcoin-billissuance-settlement-openapi.json
  type: http
- bearerFormat: JWT
  description: 'JWT Authorization header using the Bearer scheme. Example: "Authorization: Bearer {token}"'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/celcoin-credit-openapi.json
  type: http
- description: '[API V5] - Please enter into field the word ''Bearer'' following by space and the access_token (JWT)'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/celcoin-onboarding-openapi.json
  type: apiKey
slug: celcoin-authentication
source_filename: celcoin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/celcoin-billissuance-settlement-openapi.json, openapi/celcoin-credit-openapi.json,\n  openapi/celcoin-onboarding-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: Bearer\n  bearerFormat: JWT\n  description: Autenticação utilizando JTW Bearer Token\n  sources:\n  - openapi/celcoin-billissuance-settlement-openapi.json\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'JWT Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {token}\"'\n  sources:\n  - openapi/celcoin-credit-openapi.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '[API V5] - Please enter into field the word ''Bearer'' following by space and\n    the access_token (JWT)'\n  sources:\n  - openapi/celcoin-onboarding-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/authentication/celcoin-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Banking as a Service
- BaaS
- Pix
- Boleto
- TED
- Bill Payments
- Prepaid Cards
- Digital Accounts
- Open Banking
- Open Finance
- Credit
- Fintech
- Brazil
- Financial Infrastructure
---
