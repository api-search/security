---
api_key_in:
- query
api_specs:
- filename: abstract-api-email-reputation.yaml
  format: yaml
  label: Email Reputation API
  slug: email-reputation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-email-reputation.yaml
- filename: abstract-api-phone-intelligence.yaml
  format: yaml
  label: Phone Intelligence API
  slug: phone-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-phone-intelligence.yaml
- filename: abstract-api-ip-geolocation.yaml
  format: yaml
  label: IP Geolocation API
  slug: ip-geolocation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-ip-geolocation.yaml
- filename: abstract-api-ip-intelligence.yaml
  format: yaml
  label: IP Intelligence API
  slug: ip-intelligence
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-ip-intelligence.yaml
- filename: abstract-api-company-enrichment.yaml
  format: yaml
  label: Company Enrichment API
  slug: company-enrichment
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-company-enrichment.yaml
- filename: abstract-api-exchange-rates.yaml
  format: yaml
  label: Exchange Rates API
  slug: exchange-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-exchange-rates.yaml
- filename: abstract-api-public-holidays.yaml
  format: yaml
  label: Public Holidays API
  slug: public-holidays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-public-holidays.yaml
- filename: abstract-api-timezones.yaml
  format: yaml
  label: Timezone API
  slug: timezones
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-timezones.yaml
- filename: abstract-api-vat-validation.yaml
  format: yaml
  label: VAT Validation API
  slug: vat-validation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-vat-validation.yaml
- filename: abstract-api-iban-validation.yaml
  format: yaml
  label: IBAN Validation API
  slug: iban-validation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-iban-validation.yaml
- filename: abstract-api-website-screenshot.yaml
  format: yaml
  label: Website Screenshot API
  slug: website-screenshot
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-website-screenshot.yaml
- filename: abstract-api-image-processing.yaml
  format: yaml
  label: Image Processing API
  slug: image-processing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-image-processing.yaml
- filename: abstract-api-web-scraping.yaml
  format: yaml
  label: Web Scraping API
  slug: web-scraping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-web-scraping.yaml
- filename: abstract-api-avatars.yaml
  format: yaml
  label: Avatars API
  slug: avatars
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/openapi/abstract-api-avatars.yaml
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
- Currencies
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
