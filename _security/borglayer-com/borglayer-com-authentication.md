---
anonymous_access: false
api_key_in: []
api_specs:
- filename: borglayer-com-balance-api-openapi.yml
  format: yaml
  label: BorgLayer Balance API
  slug: borglayer-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-balance-api-openapi.yml
- filename: borglayer-com-chains-api-openapi.yml
  format: yaml
  label: BorgLayer Chains API
  slug: borglayer-com-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-chains-api-openapi.yml
- filename: borglayer-com-domains-api-openapi.yml
  format: yaml
  label: BorgLayer Domains API
  slug: borglayer-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-domains-api-openapi.yml
- filename: borglayer-com-formation-api-openapi.yml
  format: yaml
  label: BorgLayer Formation API
  slug: borglayer-com-formation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-formation-api-openapi.yml
- filename: borglayer-com-marketplace-api-openapi.yml
  format: yaml
  label: BorgLayer Marketplace API
  slug: borglayer-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-marketplace-api-openapi.yml
- filename: borglayer-com-register-api-openapi.yml
  format: yaml
  label: BorgLayer Register API
  slug: borglayer-com-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-register-api-openapi.yml
- filename: borglayer-com-registrant-profiles-api-openapi.yml
  format: yaml
  label: BorgLayer Registrant Profiles API
  slug: borglayer-com-registrant-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-registrant-profiles-api-openapi.yml
- filename: borglayer-com-search-api-openapi.yml
  format: yaml
  label: BorgLayer Search API
  slug: borglayer-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-search-api-openapi.yml
- filename: borglayer-com-transfer-in-api-openapi.yml
  format: yaml
  label: BorgLayer Transfer In API
  slug: borglayer-com-transfer-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/borglayer-com/openapi/borglayer-com-transfer-in-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: BorgLayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: BorgLayer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BorgLayer
provider_slug: borglayer-com
scheme_count: 1
schemes:
- bearerFormat: blrk_…
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/borglayer-com-openapi.yml
  type: http
slug: borglayer-com-authentication
source_filename: borglayer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/borglayer-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: blrk_…\n  sources:\n  - openapi/borglayer-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/borglayer-com/authentication/borglayer-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Wallets
- Domains
- Hosting
- Email
---
