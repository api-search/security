---
api_key_in: []
api_specs:
- filename: spiceworks-cloud-apps-openapi.yml
  format: yaml
  label: Spiceworks Cloud Apps API
  slug: spiceworks-cloud-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spiceworks/refs/heads/main/openapi/spiceworks-cloud-apps-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Spiceworks Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Spiceworks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Spiceworks
provider_slug: spiceworks
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication via the Spiceworks Cloud Apps platform. Applications receive an implicit grant token through the JS SDK postMessage bridge when running inside the Spiceworks UI.
  flows:
  - authorizationUrl: https://community.spiceworks.com/oauth/authorize
    flow: implicit
    scopes: 3
  name: oauth2
  sources:
  - openapi/spiceworks-cloud-apps-openapi.yml
  type: oauth2
slug: spiceworks-authentication
source_filename: spiceworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spiceworks-cloud-apps-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://community.spiceworks.com/oauth/authorize\n    scopes: 3\n  description: OAuth 2.0 authentication via the Spiceworks Cloud Apps platform. Applications\n    receive an implicit grant token through the JS SDK postMessage bridge when running inside\n    the Spiceworks UI.\n  sources:\n  - openapi/spiceworks-cloud-apps-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spiceworks/refs/heads/main/authentication/spiceworks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Community
- Enterprise IT
- IT Management
---
