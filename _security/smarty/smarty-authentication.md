---
api_key_in:
- query
api_specs:
- filename: smarty-lookup-api-openapi.yml
  format: yaml
  label: Smarty Lookup API
  slug: smarty-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-lookup-api-openapi.yml
- filename: smarty-reverse-geo-api-openapi.yml
  format: yaml
  label: Smarty reverse-geo API
  slug: smarty-reverse-geo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-reverse-geo-api-openapi.yml
- filename: smarty-street-address-api-openapi.yml
  format: yaml
  label: Smarty street-address API
  slug: smarty-street-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-street-address-api-openapi.yml
- filename: smarty-us-enrichment-api-openapi.yml
  format: yaml
  label: Smarty us-enrichment API
  slug: smarty-us-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-enrichment-api-openapi.yml
- filename: smarty-us-extract-api-api-openapi.yml
  format: yaml
  label: Smarty US Extract API API
  slug: smarty-us-extract-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-us-extract-api-api-openapi.yml
- filename: smarty-verify-api-openapi.yml
  format: yaml
  label: Smarty Verify API
  slug: smarty-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/openapi/smarty-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smarty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Smarty secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Smarty
provider_slug: smarty
scheme_count: 3
schemes:
- in: query
  name: auth-id
  parameter: auth-id
  sources:
  - openapi/smarty-international-address-autocomplete-api-openapi.yml
  - openapi/smarty-international-postal-code-api-openapi.yml
  - openapi/smarty-international-street-address-api-openapi.yml
  - openapi/smarty-us-address-enrichment-api-openapi.yml
  - openapi/smarty-us-autocomplete-pro-api-openapi.yml
  - openapi/smarty-us-extract-api-openapi.yml
  - openapi/smarty-us-reverse-geocode-api-openapi.yml
  - openapi/smarty-us-street-address-api-openapi.yml
  - openapi/smarty-us-zipcode-api-openapi.yml
  type: apiKey
- in: query
  name: auth-token
  parameter: auth-token
  sources:
  - openapi/smarty-international-address-autocomplete-api-openapi.yml
  - openapi/smarty-international-postal-code-api-openapi.yml
  - openapi/smarty-international-street-address-api-openapi.yml
  - openapi/smarty-us-address-enrichment-api-openapi.yml
  - openapi/smarty-us-autocomplete-pro-api-openapi.yml
  - openapi/smarty-us-extract-api-openapi.yml
  - openapi/smarty-us-reverse-geocode-api-openapi.yml
  - openapi/smarty-us-street-address-api-openapi.yml
  - openapi/smarty-us-zipcode-api-openapi.yml
  type: apiKey
- in: query
  name: embedded-key
  parameter: key
  sources:
  - openapi/smarty-international-address-autocomplete-api-openapi.yml
  - openapi/smarty-international-postal-code-api-openapi.yml
  - openapi/smarty-international-street-address-api-openapi.yml
  - openapi/smarty-us-address-enrichment-api-openapi.yml
  - openapi/smarty-us-autocomplete-pro-api-openapi.yml
  - openapi/smarty-us-extract-api-openapi.yml
  - openapi/smarty-us-reverse-geocode-api-openapi.yml
  - openapi/smarty-us-street-address-api-openapi.yml
  - openapi/smarty-us-zipcode-api-openapi.yml
  type: apiKey
slug: smarty-authentication
source_filename: smarty-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smarty-international-address-autocomplete-api-openapi.yml, openapi/smarty-international-postal-code-api-openapi.yml,\n  openapi/smarty-international-street-address-api-openapi.yml, openapi/smarty-us-address-enrichment-api-openapi.yml,\n  openapi/smarty-us-autocomplete-pro-api-openapi.yml, openapi/smarty-us-extract-api-openapi.yml,\n  openapi/smarty-us-reverse-geocode-api-openapi.yml, openapi/smarty-us-street-address-api-openapi.yml,\n  openapi/smarty-us-zipcode-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: auth-id\n  type: apiKey\n  in: query\n  parameter: auth-id\n  sources:\n  - openapi/smarty-international-address-autocomplete-api-openapi.yml\n  - openapi/smarty-international-postal-code-api-openapi.yml\n  - openapi/smarty-international-street-address-api-openapi.yml\n  - openapi/smarty-us-address-enrichment-api-openapi.yml\n  - openapi/smarty-us-autocomplete-pro-api-openapi.yml\n\
  \  - openapi/smarty-us-extract-api-openapi.yml\n  - openapi/smarty-us-reverse-geocode-api-openapi.yml\n  - openapi/smarty-us-street-address-api-openapi.yml\n  - openapi/smarty-us-zipcode-api-openapi.yml\n- name: auth-token\n  type: apiKey\n  in: query\n  parameter: auth-token\n  sources:\n  - openapi/smarty-international-address-autocomplete-api-openapi.yml\n  - openapi/smarty-international-postal-code-api-openapi.yml\n  - openapi/smarty-international-street-address-api-openapi.yml\n  - openapi/smarty-us-address-enrichment-api-openapi.yml\n  - openapi/smarty-us-autocomplete-pro-api-openapi.yml\n  - openapi/smarty-us-extract-api-openapi.yml\n  - openapi/smarty-us-reverse-geocode-api-openapi.yml\n  - openapi/smarty-us-street-address-api-openapi.yml\n  - openapi/smarty-us-zipcode-api-openapi.yml\n- name: embedded-key\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/smarty-international-address-autocomplete-api-openapi.yml\n  - openapi/smarty-international-postal-code-api-openapi.yml\n\
  \  - openapi/smarty-international-street-address-api-openapi.yml\n  - openapi/smarty-us-address-enrichment-api-openapi.yml\n  - openapi/smarty-us-autocomplete-pro-api-openapi.yml\n  - openapi/smarty-us-extract-api-openapi.yml\n  - openapi/smarty-us-reverse-geocode-api-openapi.yml\n  - openapi/smarty-us-street-address-api-openapi.yml\n  - openapi/smarty-us-zipcode-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarty/refs/heads/main/authentication/smarty-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Address Verification
- Geocoding
- Address Autocomplete
- ZIP Code
- Address Intelligence
- Location Data
- International Address
- US Address
---
