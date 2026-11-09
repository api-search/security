---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alshhbaa-com-auth-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Auth API
  slug: alshhbaa-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-auth-api-openapi.yml
- filename: alshhbaa-com-consultations-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Consultations API
  slug: alshhbaa-com-consultations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-consultations-api-openapi.yml
- filename: alshhbaa-com-discovery-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Discovery API
  slug: alshhbaa-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-discovery-api-openapi.yml
- filename: alshhbaa-com-projects-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Projects API
  slug: alshhbaa-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-projects-api-openapi.yml
auth_types: []
description: Authentication uses OAuth2 Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Alshhbaa Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: النحاسيات الشهباء declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: النحاسيات الشهباء
provider_slug: alshhbaa-com
scheme_count: 1
schemes:
- evidence: 'Include the access token in HTTP requests as a Bearer token:'
  header: Authorization
  how_to_obtain: Register or submit an identity assertion to the identity endpoint and then exchange it at the token endpoint.
  location: header
  name: Bearer
  scopes:
  - public
  - read:projects
  - submit:consultation
  token_url: https://alshhbaa.com/agent/token
  type: http-bearer
slug: alshhbaa-com-authentication
source_filename: alshhbaa-com-authentication.yml
source_heading: Authentication Profile
source_url: https://alshhbaa.com/auth.md
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://alshhbaa.com/auth.md\nsources:\n- https://alshhbaa.com/auth.md\ndescription: Authentication uses OAuth2 Bearer tokens.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Include the access token in HTTP requests as a Bearer token:'\n  location: header\n  header: Authorization\n  token_url: https://alshhbaa.com/agent/token\n  scopes:\n  - public\n  - read:projects\n  - submit:consultation\n  how_to_obtain: Register or submit an identity assertion to the identity endpoint and then exchange it at the token endpoint.\ndocs: https://alshhbaa.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/alshhbaa-com/authentication/alshhbaa-com-authentication.yml
summary_line: 1 scheme
tags:
- Lighting
- Chandeliers
- Saudi Arabia
- Luxury
- Manufacturing
- Company
---
