---
anonymous_access: false
api_key_in: []
api_specs:
- filename: drivings-com-discovery-api-openapi.yml
  format: yaml
  label: Drivings Discovery API
  slug: drivings-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-discovery-api-openapi.yml
- filename: drivings-com-planning-api-openapi.yml
  format: yaml
  label: Drivings Planning API
  slug: drivings-com-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/drivings-com/openapi/drivings-com-planning-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Drivings Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Drivings secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Drivings
provider_slug: drivings-com
scheme_count: 1
schemes:
- description: Not required by any operation in this document. It gates one MCP tool, the learner's own progress, and is listed so an agent can see the whole permission surface in one place.
  flows:
  - authorizationUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/token
  name: drivingsOAuth
  sources:
  - openapi/drivings-com-openapi.json
  type: oauth2
slug: drivings-com-authentication
source_filename: drivings-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/drivings-com-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: drivingsOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/authorize\n    tokenUrl: https://xqvjkpkownkftsdofpbb.supabase.co/auth/v1/token\n    scopes: 3\n  description: Not required by any operation in this document. It gates one MCP tool, the learner's\n    own progress, and is listed so an agent can see the whole permission surface in one place.\n  sources:\n  - openapi/drivings-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/drivings-com/authentication/drivings-com-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Driving
- Education
- United Kingdom
- US
---
