---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-onenote-groups-site-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Groups.site API
  slug: microsoft-onenote-groups-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-groups-site-api-openapi.yml
- filename: microsoft-onenote-me-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Me.onenote API
  slug: microsoft-onenote-me-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-me-onenote-api-openapi.yml
- filename: microsoft-onenote-notebooks-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Notebooks API
  slug: microsoft-onenote-notebooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-notebooks-api-openapi.yml
- filename: microsoft-onenote-pages-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Pages API
  slug: microsoft-onenote-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-pages-api-openapi.yml
- filename: microsoft-onenote-sectiongroups-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Section Groups API
  slug: microsoft-onenote-sectiongroups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-sectiongroups-api-openapi.yml
- filename: microsoft-onenote-sections-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Sections API
  slug: microsoft-onenote-sections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-sections-api-openapi.yml
- filename: microsoft-onenote-groups-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Groups.onenote API
  slug: microsoft-onenote-groups-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-groups-onenote-api-openapi.yml
- filename: microsoft-onenote-sites-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Sites.onenote API
  slug: microsoft-onenote-sites-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-sites-onenote-api-openapi.yml
- filename: microsoft-onenote-users-onenote-api-openapi.yml
  format: yaml
  label: Microsoft OneNote Users.onenote API
  slug: microsoft-onenote-users-onenote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onenote/openapi/microsoft-onenote-users-onenote-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Microsoft OneNote Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Microsoft OneNote secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Microsoft OneNote
provider_slug: microsoft-onenote
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-onenote-notebooks-api-openapi.yml
  - openapi/_superseded/microsoft-onenote-pages-api-openapi.yml
  - openapi/_superseded/microsoft-onenote-sectiongroups-api-openapi.yml
  - openapi/_superseded/microsoft-onenote-sections-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  name: azureaadv2
  sources:
  - openapi/microsoft-onenote-openapi.yml
  type: oauth2
slug: microsoft-onenote-authentication
source_filename: microsoft-onenote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-onenote-notebooks-api-openapi.yml, openapi/microsoft-onenote-openapi.yml,\n  openapi/_superseded/microsoft-onenote-pages-api-openapi.yml, openapi/_superseded/microsoft-onenote-sectiongroups-api-openapi.yml,\n  openapi/_superseded/microsoft-onenote-sections-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_superseded/microsoft-onenote-notebooks-api-openapi.yml\n  - openapi/_superseded/microsoft-onenote-pages-api-openapi.yml\n  - openapi/_superseded/microsoft-onenote-sectiongroups-api-openapi.yml\n  - openapi/_superseded/microsoft-onenote-sections-api-openapi.yml\n- name: azureaadv2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n\
  \    scopes: 0\n  sources:\n  - openapi/microsoft-onenote-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-onenote/authentication/microsoft-onenote-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Microsoft
- Microsoft 365
- Notebooks
- Notes
- Productivity
---
