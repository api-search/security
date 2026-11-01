---
anonymous_access: false
api_key_in: []
api_specs:
- filename: randnext-draws-api-openapi.yml
  format: yaml
  label: RandNext Draws API
  slug: randnext-draws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-draws-api-openapi.yml
- filename: randnext-health-api-openapi.yml
  format: yaml
  label: RandNext Health API
  slug: randnext-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-health-api-openapi.yml
- filename: randnext-jokes-api-openapi.yml
  format: yaml
  label: RandNext Jokes API
  slug: randnext-jokes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-jokes-api-openapi.yml
- filename: randnext-questions-api-openapi.yml
  format: yaml
  label: RandNext Questions API
  slug: randnext-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-questions-api-openapi.yml
- filename: randnext-quotes-api-openapi.yml
  format: yaml
  label: RandNext Quotes API
  slug: randnext-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-quotes-api-openapi.yml
- filename: randnext-tools-api-openapi.yml
  format: yaml
  label: RandNext Tools API
  slug: randnext-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-tools-api-openapi.yml
- filename: randnext-words-api-openapi.yml
  format: yaml
  label: RandNext Words API
  slug: randnext-words-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/randnext/openapi/randnext-words-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Randnext Authentication
name_suffix: Authentication
oauth_flows: []
overview: RandNext secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RandNext
provider_slug: randnext
scheme_count: 1
schemes:
- description: The manage token returned once when the draw was created.
  name: manageToken
  scheme: bearer
  sources:
  - openapi/randnext-openapi.json
  type: http
slug: randnext-authentication
source_filename: randnext-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/randnext-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: manageToken\n  type: http\n  scheme: bearer\n  description: The manage token returned once when the draw was created.\n  sources:\n  - openapi/randnext-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/randnext/authentication/randnext-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Random
- Generator
- API
- Fun
---
