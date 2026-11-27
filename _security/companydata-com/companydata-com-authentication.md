---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: companydata-com-company-api-openapi.yml
  format: yaml
  label: CompanyData Company API
  slug: companydata-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-company-api-openapi.yml
- filename: companydata-com-corporate-structure-api-openapi.yml
  format: yaml
  label: CompanyData Corporate Structure API
  slug: companydata-com-corporate-structure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-corporate-structure-api-openapi.yml
- filename: companydata-com-domain-enrichment-api-openapi.yml
  format: yaml
  label: CompanyData Domain Enrichment API
  slug: companydata-com-domain-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-domain-enrichment-api-openapi.yml
- filename: companydata-com-lookup-api-openapi.yml
  format: yaml
  label: CompanyData Lookup API
  slug: companydata-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/companydata-com/openapi/companydata-com-lookup-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CompanyData Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompanyData secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CompanyData
provider_slug: companydata-com
scheme_count: 1
schemes:
- description: API key for the CompanyData API. Required on all endpoints.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/companydata-com-openapi.yml
  - https://companydata.com/api-docs/authentication/
  type: apiKey
slug: companydata-com-authentication
source_filename: companydata-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://companydata.com/api-docs/authentication/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for the CompanyData API. Required on all endpoints.\n  sources:\n  - openapi/companydata-com-openapi.yml\n  - https://companydata.com/api-docs/authentication/\ndocs: https://companydata.com/api-docs/authentication/\nkey_issuance: https://app.companydata.com/signup-api/\nfailure:\n  status: 401\n  body:\n    message: Unauthorized\n    statusCode: 401\n  text: 'Missing or invalid key: HTTP 401'\nguidance: Never expose API keys in client-side code or public repositories. Use environment variables or a secrets manager in production.\ntrial: New accounts get a 7-day free trial (500 searches and 10 exports, card at signup)\n"
source_yaml_url: https://artifacts.apis.io/companydata-com/authentication/companydata-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Company Data
- Business Registry
- B2B Data
- Data Enrichment
- KYC
- KYB
- Lead Generation
- MCP
---
