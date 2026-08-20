---
api_key_in:
- query
api_specs:
- filename: abstract-api-avatars-api-openapi.yml
  format: yaml
  label: Abstract API Avatars API
  slug: abstract-api-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-avatars-api-openapi.yml
- filename: abstract-api-company-enrichment-api-openapi.yml
  format: yaml
  label: Abstract API Company Enrichment API
  slug: abstract-api-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-company-enrichment-api-openapi.yml
- filename: abstract-api-email-reputation-api-openapi.yml
  format: yaml
  label: Abstract API Email Reputation API
  slug: abstract-api-email-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-email-reputation-api-openapi.yml
- filename: abstract-api-exchange-rates-api-openapi.yml
  format: yaml
  label: Abstract API Exchange Rates API
  slug: abstract-api-exchange-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-exchange-rates-api-openapi.yml
- filename: abstract-api-iban-validation-api-openapi.yml
  format: yaml
  label: Abstract API IBAN Validation API
  slug: abstract-api-iban-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-iban-validation-api-openapi.yml
- filename: abstract-api-image-processing-api-openapi.yml
  format: yaml
  label: Abstract API Image Processing API
  slug: abstract-api-image-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-image-processing-api-openapi.yml
- filename: abstract-api-ip-geolocation-api-openapi.yml
  format: yaml
  label: Abstract API IP Geolocation API
  slug: abstract-api-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-ip-geolocation-api-openapi.yml
- filename: abstract-api-ip-intelligence-api-openapi.yml
  format: yaml
  label: Abstract API IP Intelligence API
  slug: abstract-api-ip-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-ip-intelligence-api-openapi.yml
- filename: abstract-api-phone-intelligence-api-openapi.yml
  format: yaml
  label: Abstract API Phone Intelligence API
  slug: abstract-api-phone-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-phone-intelligence-api-openapi.yml
- filename: abstract-api-public-holidays-api-openapi.yml
  format: yaml
  label: Abstract API Public Holidays API
  slug: abstract-api-public-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-public-holidays-api-openapi.yml
- filename: abstract-api-timezones-api-openapi.yml
  format: yaml
  label: Abstract API Timezones API
  slug: abstract-api-timezones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-timezones-api-openapi.yml
- filename: abstract-api-vat-validation-api-openapi.yml
  format: yaml
  label: Abstract API VAT Validation API
  slug: abstract-api-vat-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-vat-validation-api-openapi.yml
- filename: abstract-api-web-scraping-api-openapi.yml
  format: yaml
  label: Abstract API Web Scraping API
  slug: abstract-api-web-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-web-scraping-api-openapi.yml
- filename: abstract-api-website-screenshot-api-openapi.yml
  format: yaml
  label: Abstract API Website Screenshot API
  slug: abstract-api-website-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-website-screenshot-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Abstract Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Abstract API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Abstract API
provider_slug: abstract-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/abstract-api-avatars.yaml
  - openapi/abstract-api-company-enrichment.yaml
  - openapi/abstract-api-email-reputation.yaml
  - openapi/abstract-api-exchange-rates.yaml
  - openapi/abstract-api-iban-validation.yaml
  - openapi/abstract-api-image-processing.yaml
  - openapi/abstract-api-ip-geolocation.yaml
  - openapi/abstract-api-ip-intelligence.yaml
  - openapi/abstract-api-phone-intelligence.yaml
  - openapi/abstract-api-public-holidays.yaml
  - openapi/abstract-api-timezones.yaml
  - openapi/abstract-api-vat-validation.yaml
  - openapi/abstract-api-web-scraping.yaml
  - openapi/abstract-api-website-screenshot.yaml
  type: apiKey
slug: abstract-api-authentication
source_filename: abstract-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/abstract-api-avatars.yaml, openapi/abstract-api-company-enrichment.yaml, openapi/abstract-api-email-reputation.yaml,\n  openapi/abstract-api-exchange-rates.yaml, openapi/abstract-api-iban-validation.yaml, openapi/abstract-api-image-processing.yaml,\n  openapi/abstract-api-ip-geolocation.yaml, openapi/abstract-api-ip-intelligence.yaml, openapi/abstract-api-phone-intelligence.yaml,\n  openapi/abstract-api-public-holidays.yaml, openapi/abstract-api-timezones.yaml, openapi/abstract-api-vat-validation.yaml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/abstract-api-avatars.yaml\n  - openapi/abstract-api-company-enrichment.yaml\n  - openapi/abstract-api-email-reputation.yaml\n  - openapi/abstract-api-exchange-rates.yaml\n  - openapi/abstract-api-iban-validation.yaml\n  - openapi/abstract-api-image-processing.yaml\n\
  \  - openapi/abstract-api-ip-geolocation.yaml\n  - openapi/abstract-api-ip-intelligence.yaml\n  - openapi/abstract-api-phone-intelligence.yaml\n  - openapi/abstract-api-public-holidays.yaml\n  - openapi/abstract-api-timezones.yaml\n  - openapi/abstract-api-vat-validation.yaml\n  - openapi/abstract-api-web-scraping.yaml\n  - openapi/abstract-api-website-screenshot.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/authentication/abstract-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Avatars
- Company Enrichment
- Contacts
- Currency
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
---
