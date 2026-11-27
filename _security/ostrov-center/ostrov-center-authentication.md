---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ostrov-center-access-md-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Access.md API
  slug: ostrov-center-access-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-access-md-api-openapi.yml
- filename: ostrov-center-applications-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Applications API
  slug: ostrov-center-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-applications-api-openapi.yml
- filename: ostrov-center-calendar-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Calendar API
  slug: ostrov-center-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-calendar-api-openapi.yml
- filename: ostrov-center-catalog-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Catalog API
  slug: ostrov-center-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-catalog-api-openapi.yml
- filename: ostrov-center-center-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Center API
  slug: ostrov-center-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-center-api-openapi.yml
- filename: ostrov-center-estimates-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Estimates API
  slug: ostrov-center-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-estimates-api-openapi.yml
- filename: ostrov-center-events-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Events API
  slug: ostrov-center-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-events-api-openapi.yml
- filename: ostrov-center-examples-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Examples API
  slug: ostrov-center-examples-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-examples-api-openapi.yml
- filename: ostrov-center-objects-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Objects API
  slug: ostrov-center-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-objects-api-openapi.yml
- filename: ostrov-center-openapi-json-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Openapi.json API
  slug: ostrov-center-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-openapi-json-api-openapi.yml
- filename: ostrov-center-quickstart-md-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Quickstart.md API
  slug: ostrov-center-quickstart-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-quickstart-md-api-openapi.yml
- filename: ostrov-center-quotes-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Quotes API
  slug: ostrov-center-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-quotes-api-openapi.yml
- filename: ostrov-center-readme-md-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Readme.md API
  slug: ostrov-center-readme-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-readme-md-api-openapi.yml
- filename: ostrov-center-sessions-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Sessions API
  slug: ostrov-center-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-sessions-api-openapi.yml
- filename: ostrov-center-skill-md-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Skill.md API
  slug: ostrov-center-skill-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-skill-md-api-openapi.yml
- filename: ostrov-center-suggestions-api-openapi.yml
  format: yaml
  label: Ретритный центр «Остров» Suggestions API
  slug: ostrov-center-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ostrov-center/openapi/ostrov-center-suggestions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ретритный центр «Остров» Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ретритный центр «Остров» secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ретритный центр «Остров»
provider_slug: ostrov-center
scheme_count: 1
schemes:
- description: Token from POST sessions. Never send in a URL. Expires after 30 days; signup and private center keys are not required.
  name: GuestSession
  scheme: bearer
  sources:
  - openapi/ostrov-center-openapi.yml
  type: http
slug: ostrov-center-authentication
source_filename: ostrov-center-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/ostrov-center-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: GuestSession\n  type: http\n  scheme: bearer\n  description: Token from POST sessions. Never send in a URL. Expires after 30 days; signup\n    and private center keys are not required.\n  sources:\n  - openapi/ostrov-center-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ostrov-center/authentication/ostrov-center-authentication.yml
summary_line: http · 1 scheme
tags:
- Retreat
- Yoga
- Wellness
- Russia
- Karjala
---
