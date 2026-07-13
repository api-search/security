---
api_key_in:
- header
- query
api_specs:
- filename: api-spec
  format: yaml
  label: CMS Marketplace API
  slug: cms-marketplace-api
  spec_type: OpenAPI
  url: https://developer.cms.gov/marketplace-api/api-spec
- filename: openapi
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: cms-blue-button-20-api
  spec_type: OpenAPI
  url: https://sandbox.bluebutton.cms.gov/docs/openapi
- filename: api-spec
  format: yaml
  label: CMS Procedure Price Lookup (PPL) API
  slug: cms-procedure-price-lookup-ppl-api
  spec_type: OpenAPI
  url: https://developer.cms.gov/ppl-api/api-spec
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centers for Medicare and Medicaid Services secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Centers for Medicare and Medicaid Services
provider_slug: cms
scheme_count: 3
schemes:
- description: Your API key should be included as a query parameter with the request. You can [fill out this form](https://cms.gov1.qualtrics.com/jfe/form/SV_4N2GHCJfNuX7n8x) to request an API key.
  in: query
  name: API Key
  parameter: apikey
  sources:
  - openapi/marketplace-openapi.json
  type: apiKey
- description: All requests must include the `apiKey` header containing your API Key.
  in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/ppl-openapi.json
  type: apiKey
- description: All requests must include the `amaLicense` header containing your AMA License.
  in: header
  name: amaLicense
  parameter: amaLicense
  sources:
  - openapi/ppl-openapi.json
  type: apiKey
slug: cms-authentication
source_filename: cms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/marketplace-openapi.json, openapi/ppl-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: API Key\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Your API key should be included as a query parameter with the request. You can\n    [fill out this form](https://cms.gov1.qualtrics.com/jfe/form/SV_4N2GHCJfNuX7n8x) to request\n    an API key.\n  sources:\n  - openapi/marketplace-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: All requests must include the `apiKey` header containing your API Key.\n  sources:\n  - openapi/ppl-openapi.json\n- name: amaLicense\n  type: apiKey\n  in: header\n  parameter: amaLicense\n  description: All requests must include the `amaLicense` header containing your AMA License.\n  sources:\n  - openapi/ppl-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms/refs/heads/main/authentication/cms-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Medicare
- Medicaid
- Healthcare
- Health Insurance
- FHIR
- Federal Government
- Drug Spending
- Provider Data
- Quality Measures
- Claims Data
---
