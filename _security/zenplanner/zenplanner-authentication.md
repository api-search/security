---
api_key_in: []
api_specs:
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner People API
  slug: zenplanner-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Memberships API
  slug: zenplanner-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Classes API
  slug: zenplanner-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Locations API
  slug: zenplanner-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Programs API
  slug: zenplanner-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Prospects API
  slug: zenplanner-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Groups API
  slug: zenplanner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zenplanner Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zen Planner secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zen Planner
provider_slug: zenplanner
scheme_count: 1
schemes:
- description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens from https://operations.oauth2.partners.daxko.com/token.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token
  name: oauth2
  sources:
  - openapi/zenplanner-openapi.yml
  type: oauth2
slug: zenplanner-authentication
source_filename: zenplanner-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zenplanner-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.partners.daxko.com/v3/partners/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 against the Daxko Partners token service. Partner/API access tokens\n    are obtained from https://api.partners.daxko.com/v3/partners/oauth2/token and member tokens\n    from https://operations.oauth2.partners.daxko.com/token.\n  sources:\n  - openapi/zenplanner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/authentication/zenplanner-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fitness
- Gym Management
- Studio Management
- Martial Arts
- Membership
- Scheduling
- Class Booking
- Daxko
---
