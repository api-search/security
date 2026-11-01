---
anonymous_access: false
api_key_in: []
api_specs:
- filename: invidious-invidious-api-api-openapi.yml
  format: yaml
  label: Invidious API
  slug: invidious-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invidious/openapi/invidious-invidious-api-api-openapi.yml
- filename: invidious-openapi-generated.yml
  format: yaml
  label: Invidious API
  slug: invidious-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invidious/openapi/_ae-authored/invidious-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Invidious Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invidious declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Invidious
provider_slug: invidious
scheme_count: 2
schemes:
- description: Session cookie for logged-in users
  location: header
  name: SID
  type: cookie
- description: Recommended token authentication
  format: Bearer <TOKEN>
  location: header
  name: Authorization
  type: bearer
slug: invidious-authentication
source_filename: invidious-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.invidious.io/api/authenticated-endpoints/\nschemes:\n  - type: cookie\n    name: SID\n    description: Session cookie for logged-in users\n    location: header\n  - type: bearer\n    name: Authorization\n    format: Bearer <TOKEN>\n    description: Recommended token authentication\n    location: header\n"
source_yaml_url: https://artifacts.apis.io/invidious/authentication/invidious-authentication.yml
summary_line: 2 schemes
tags:
- video
- open-source
- privacy
- api
- frontend
- youtube
---
