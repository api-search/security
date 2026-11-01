---
anonymous_access: false
api_key_in: []
api_specs:
- filename: autohost-accounts-api-openapi.yml
  format: yaml
  label: Autohost Accounts API
  slug: autohost-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-accounts-api-openapi.yml
- filename: autohost-background-check-api-openapi.yml
  format: yaml
  label: Autohost Background Check API
  slug: autohost-background-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-background-check-api-openapi.yml
- filename: autohost-fraud-api-openapi.yml
  format: yaml
  label: Autohost Fraud API
  slug: autohost-fraud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-fraud-api-openapi.yml
- filename: autohost-idcheck-api-openapi.yml
  format: yaml
  label: Autohost Idcheck API
  slug: autohost-idcheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-idcheck-api-openapi.yml
- filename: autohost-listings-api-openapi.yml
  format: yaml
  label: Autohost Listings API
  slug: autohost-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-listings-api-openapi.yml
- filename: autohost-lookup-api-openapi.yml
  format: yaml
  label: Autohost Lookup API
  slug: autohost-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-lookup-api-openapi.yml
- filename: autohost-reservations-api-openapi.yml
  format: yaml
  label: Autohost Reservations API
  slug: autohost-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-reservations-api-openapi.yml
- filename: autohost-validate-api-openapi.yml
  format: yaml
  label: Autohost Validate API
  slug: autohost-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-validate-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Autohost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autohost declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Autohost
provider_slug: autohost
scheme_count: 1
schemes:
- description: API Authentication Key
  in: header
  name: x-api-key
  type: apiKey
slug: autohost-authentication
source_filename: autohost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.autohost.ai/docs/api/reference/api-accounts\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: API Authentication Key"
source_yaml_url: https://artifacts.apis.io/autohost/authentication/autohost-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IdentityVerification
- BackgroundCheck
- FraudDetection
- Hospitality
- RealEstate
---
