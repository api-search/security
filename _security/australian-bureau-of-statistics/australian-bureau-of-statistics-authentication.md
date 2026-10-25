---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: australian-bureau-of-statistics-get-data-api-openapi.yml
  format: yaml
  label: Australian Bureau of Statistics Get Data API
  slug: australian-bureau-of-statistics-get-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-bureau-of-statistics/refs/heads/main/openapi/australian-bureau-of-statistics-get-data-api-openapi.yml
- filename: australian-bureau-of-statistics-get-metadata-api-openapi.yml
  format: yaml
  label: Australian Bureau of Statistics Get Metadata API
  slug: australian-bureau-of-statistics-get-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/australian-bureau-of-statistics/refs/heads/main/openapi/australian-bureau-of-statistics-get-metadata-api-openapi.yml
auth_types:
- apiKey
- none
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Australian Bureau Of Statistics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian Bureau of Statistics secures its APIs with apiKey and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australian Bureau of Statistics
provider_slug: australian-bureau-of-statistics
scheme_count: 2
schemes:
- applies_to: ABS Indicator API (indicator.api.abs.gov.au)
  docs_quote: 'Once you have been issued an API Key, you must add it as a header in your API requests:  "x-api-key: xxxxxxxxxxxxxxx"'
  in: header
  issuance: Manual. Read the Indicator API Terms of Use, then download and complete the 'ABS Indicator API Key Request Form'; "The ABS will deliver the API Key to You via your nominated email address as soon as practicably possible following receipt your Request."
  key_request_form: https://www.abs.gov.au/system/files/documents/e229d9b19dd0be5a892fc9802c24fd74/ABS%20Indicator%20API%20Key%20Request%20Form.docx
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/australian-bureau-of-statistics-indicator-api-openapi.yml
  - https://www.abs.gov.au/statistics/application-programming-interfaces-apis/indicator-api
  terms: https://www.abs.gov.au/about/data-services/application-programming-interfaces-apis/indicator-api/terms-use
  type: apiKey
- applies_to: ABS Data API (Beta) (data.api.abs.gov.au)
  docs: https://www.abs.gov.au/statistics/application-programming-interfaces-apis/data-api-user-guide
  docs_quote: The Data API is freely accessible without the need for an API key.
  name: none
  type: none
slug: australian-bureau-of-statistics-authentication
source_filename: australian-bureau-of-statistics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://www.abs.gov.au/statistics/application-programming-interfaces-apis/indicator-api\ndocs: https://www.abs.gov.au/statistics/application-programming-interfaces-apis/indicator-api\nsummary:\n  types:\n  - apiKey\n  - none\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applies_to: ABS Indicator API (indicator.api.abs.gov.au)\n  sources:\n  - openapi/australian-bureau-of-statistics-indicator-api-openapi.yml\n  - https://www.abs.gov.au/statistics/application-programming-interfaces-apis/indicator-api\n  docs_quote: 'Once you have been issued an API Key, you must add it as a header in your API requests:  \"x-api-key: xxxxxxxxxxxxxxx\"'\n  issuance: 'Manual. Read the Indicator API Terms of Use, then download and complete the ''ABS Indicator API Key Request Form''; \"The ABS will deliver the API Key to You via your nominated email address as soon as practicably possible\
  \ following receipt your Request.\"'\n  key_request_form: https://www.abs.gov.au/system/files/documents/e229d9b19dd0be5a892fc9802c24fd74/ABS%20Indicator%20API%20Key%20Request%20Form.docx\n  terms: https://www.abs.gov.au/about/data-services/application-programming-interfaces-apis/indicator-api/terms-use\n- name: none\n  type: none\n  applies_to: ABS Data API (Beta) (data.api.abs.gov.au)\n  docs: https://www.abs.gov.au/statistics/application-programming-interfaces-apis/data-api-user-guide\n  docs_quote: The Data API is freely accessible without the need for an API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-bureau-of-statistics/refs/heads/main/authentication/australian-bureau-of-statistics-authentication.yml
summary_line: apiKey/none · 2 schemes
tags:
- Company
- Government
- Statistics
- Open Data
- SDMX
- Census
- Economic Indicators
- Australia
---
