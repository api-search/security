---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: getapi-nl-bag-addresses-and-buildings-register-api-openapi.yml
  format: yaml
  label: getapi-nl BAG – Addresses and Buildings Register API
  slug: getapi-nl-bag-addresses-and-buildings-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-bag-addresses-and-buildings-register-api-openapi.yml
- filename: getapi-nl-cbs-sbi-codes-api-openapi.yml
  format: yaml
  label: getapi-nl CBS - SBI Codes API
  slug: getapi-nl-cbs-sbi-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-cbs-sbi-codes-api-openapi.yml
- filename: getapi-nl-dns-lookup-api-openapi.yml
  format: yaml
  label: getapi-nl DNS Lookup API
  slug: getapi-nl-dns-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-dns-lookup-api-openapi.yml
- filename: getapi-nl-dnsbl-spam-blacklist-api-openapi.yml
  format: yaml
  label: getapi-nl DNSBL / Spam Blacklist API
  slug: getapi-nl-dnsbl-spam-blacklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-dnsbl-spam-blacklist-api-openapi.yml
- filename: getapi-nl-dso-environmental-information-api-openapi.yml
  format: yaml
  label: getapi-nl DSO - Environmental information API
  slug: getapi-nl-dso-environmental-information-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-dso-environmental-information-api-openapi.yml
- filename: getapi-nl-email-validation-api-openapi.yml
  format: yaml
  label: getapi-nl Email Validation API
  slug: getapi-nl-email-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-email-validation-api-openapi.yml
- filename: getapi-nl-geolocation-services-api-openapi.yml
  format: yaml
  label: getapi-nl Geolocation services API
  slug: getapi-nl-geolocation-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-geolocation-services-api-openapi.yml
- filename: getapi-nl-iban-bic-validation-api-openapi.yml
  format: yaml
  label: getapi-nl IBAN / BIC Validation API
  slug: getapi-nl-iban-bic-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-iban-bic-validation-api-openapi.yml
- filename: getapi-nl-ip-location-lookup-api-openapi.yml
  format: yaml
  label: getapi-nl IP Location Lookup API
  slug: getapi-nl-ip-location-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ip-location-lookup-api-openapi.yml
- filename: getapi-nl-ndw-charging-points-api-openapi.yml
  format: yaml
  label: getapi-nl NDW - Charging points API
  slug: getapi-nl-ndw-charging-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ndw-charging-points-api-openapi.yml
- filename: getapi-nl-ndw-emission-zones-api-openapi.yml
  format: yaml
  label: getapi-nl NDW - Emission zones API
  slug: getapi-nl-ndw-emission-zones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ndw-emission-zones-api-openapi.yml
- filename: getapi-nl-ndw-truckparking-api-openapi.yml
  format: yaml
  label: getapi-nl NDW - Truckparking API
  slug: getapi-nl-ndw-truckparking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-ndw-truckparking-api-openapi.yml
- filename: getapi-nl-property-data-api-openapi.yml
  format: yaml
  label: getapi-nl Property data API
  slug: getapi-nl-property-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-property-data-api-openapi.yml
- filename: getapi-nl-rdw-api-openapi.yml
  format: yaml
  label: getapi-nl RDW API
  slug: getapi-nl-rdw-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-rdw-api-openapi.yml
- filename: getapi-nl-rvo-api-openapi.yml
  format: yaml
  label: getapi-nl RVO API
  slug: getapi-nl-rvo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-rvo-api-openapi.yml
- filename: getapi-nl-site-scraping-api-openapi.yml
  format: yaml
  label: getapi-nl Site Scraping API
  slug: getapi-nl-site-scraping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-site-scraping-api-openapi.yml
- filename: getapi-nl-vat-validation-api-openapi.yml
  format: yaml
  label: getapi-nl VAT Validation API
  slug: getapi-nl-vat-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getapi-nl/openapi/getapi-nl-vat-validation-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Getapi Nl Authentication
name_suffix: Authentication
oauth_flows: []
overview: getapi-nl secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: getapi-nl
provider_slug: getapi-nl
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/getapi-nl-openapi.json
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/getapi-nl-openapi.json
  type: http
slug: getapi-nl-authentication
source_filename: getapi-nl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/getapi-nl-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/getapi-nl-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/getapi-nl-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getapi-nl/authentication/getapi-nl-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- API
- Dutch
- WebScraping
- DataValidation
---
