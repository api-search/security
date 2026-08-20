---
api_key_in:
- header
- query
api_specs:
- filename: apex27-crm-api-openapi.yml
  format: yaml
  label: Apex27 CRM API
  slug: apex27-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apex27/refs/heads/main/openapi/apex27-crm-api-openapi.yml
- filename: apex27-portal-api-openapi.yml
  format: yaml
  label: Apex27 Portal API
  slug: apex27-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apex27/refs/heads/main/openapi/apex27-portal-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apex27 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apex27 secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apex27
provider_slug: apex27
scheme_count: 2
schemes:
- description: API key issued to a paying Apex27 tenant from the CRM admin panel. No self-serve issuance.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/apex27-crm-api-openapi.yml
  type: apiKey
- description: Portal API key from Admin Panel > Websites > [Your Website] > Integrations tab > Portal API section.
  in: query
  name: PortalApiKey
  parameter: api_key
  sources:
  - openapi/apex27-portal-api-openapi.yml
  type: apiKey
slug: apex27-authentication
source_filename: apex27-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/apex27-crm-api-openapi.yml, openapi/apex27-portal-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key issued to a paying Apex27 tenant from the CRM admin panel. No self-serve\n    issuance.\n  sources:\n  - openapi/apex27-crm-api-openapi.yml\n- name: PortalApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Portal API key from Admin Panel > Websites > [Your Website] > Integrations tab\n    > Portal API section.\n  sources:\n  - openapi/apex27-portal-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apex27/refs/heads/main/authentication/apex27-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Listings
- CRM
- Estate Agency
- Lettings
- Rentals
- Property Management
- Valuation
- Tenancy
- Conveyancing
---
