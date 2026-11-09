---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buckybuild-com-addresses-api-openapi.yml
  format: yaml
  label: Bucky Addresses API
  slug: buckybuild-com-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-addresses-api-openapi.yml
- filename: buckybuild-com-citations-api-openapi.yml
  format: yaml
  label: Bucky Citations API
  slug: buckybuild-com-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-citations-api-openapi.yml
- filename: buckybuild-com-coverage-api-openapi.yml
  format: yaml
  label: Bucky Coverage API
  slug: buckybuild-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-coverage-api-openapi.yml
- filename: buckybuild-com-credentials-api-openapi.yml
  format: yaml
  label: Bucky Credentials API
  slug: buckybuild-com-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-credentials-api-openapi.yml
- filename: buckybuild-com-feasibility-api-openapi.yml
  format: yaml
  label: Bucky Feasibility API
  slug: buckybuild-com-feasibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-feasibility-api-openapi.yml
- filename: buckybuild-com-marketplace-api-openapi.yml
  format: yaml
  label: Bucky Marketplace API
  slug: buckybuild-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-marketplace-api-openapi.yml
- filename: buckybuild-com-sites-api-openapi.yml
  format: yaml
  label: Bucky Sites API
  slug: buckybuild-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-sites-api-openapi.yml
- filename: buckybuild-com-usage-api-openapi.yml
  format: yaml
  label: Bucky Usage API
  slug: buckybuild-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buckybuild-com/openapi/buckybuild-com-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Buckybuild Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bucky secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bucky
provider_slug: buckybuild-com
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Supabase-issued user JWT: a signed-in session, or one an agent with no browser gets from https://buckybuild.com/auth.md (exchange without `resource`).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/buckybuild-com-openapi.json
  type: http
slug: buckybuild-com-authentication
source_filename: buckybuild-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buckybuild-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Supabase-issued user JWT: a signed-in session, or one an agent with no browser\n    gets from https://buckybuild.com/auth.md (exchange without `resource`).'\n  sources:\n  - openapi/buckybuild-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/buckybuild-com/authentication/buckybuild-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- Zoning
- Mapping
- Data API
- Visualization
- Company
---
