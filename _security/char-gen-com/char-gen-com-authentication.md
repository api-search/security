---
anonymous_access: false
api_key_in: []
api_specs:
- filename: char-gen-com-account-catalog-api-openapi.yml
  format: yaml
  label: CharGen Account & catalog API
  slug: char-gen-com-account-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-account-catalog-api-openapi.yml
- filename: char-gen-com-billing-api-openapi.yml
  format: yaml
  label: CharGen Billing API
  slug: char-gen-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-billing-api-openapi.yml
- filename: char-gen-com-entities-api-openapi.yml
  format: yaml
  label: CharGen Entities API
  slug: char-gen-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-entities-api-openapi.yml
- filename: char-gen-com-generations-api-openapi.yml
  format: yaml
  label: CharGen Generations API
  slug: char-gen-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-generations-api-openapi.yml
- filename: char-gen-com-ping-api-openapi.yml
  format: yaml
  label: CharGen Ping API
  slug: char-gen-com-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-ping-api-openapi.yml
- filename: char-gen-com-public-pricing-api-openapi.yml
  format: yaml
  label: CharGen Public pricing API
  slug: char-gen-com-public-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/char-gen-com/openapi/char-gen-com-public-pricing-api-openapi.yml
auth_types: []
description: Authentication schemes for CharGen API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CharGen Authentication
name_suffix: Authentication
oauth_flows: []
overview: CharGen declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CharGen
provider_slug: char-gen-com
scheme_count: 1
schemes:
- evidence: 'Every endpoint except the public pricing list requires an API key in the Authorization header:'
  header: Authorization
  how_to_obtain: Keys are minted in the developer portal and shown once when minted.
  location: header
  name: Authorization
  type: http-bearer
slug: char-gen-com-authentication
source_filename: char-gen-com-authentication.yml
source_heading: Authentication Profile
source_url: https://char-gen.com/developers?tab=keys
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://char-gen.com/developers?tab=keys\nsources:\n- https://char-gen.com/developers?tab=keys\n- https://char-gen.com/token-maker\n- https://char-gen.com/developers/docs\ndescription: Authentication schemes for CharGen API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Every endpoint except the public pricing list requires an API key in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are minted in the developer portal and shown once when minted.\nnote: No OAuth2 flows are documented on the provided pages.\ndocs: https://char-gen.com/developers?tab=keys\n"
source_yaml_url: https://artifacts.apis.io/char-gen-com/authentication/char-gen-com-authentication.yml
summary_line: 1 scheme
tags:
- AI Art
- RPG Tools
- Character Generation
- Map Generation
- Campaign Building
- Audio Generation
---
