---
api_key_in: []
api_specs:
- filename: heroku-account-api-openapi.yml
  format: yaml
  label: Heroku Account API
  slug: heroku-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-account-api-openapi.yml
- filename: heroku-add-ons-api-openapi.yml
  format: yaml
  label: Heroku Add-ons API
  slug: heroku-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-add-ons-api-openapi.yml
- filename: heroku-apps-api-openapi.yml
  format: yaml
  label: Heroku Apps API
  slug: heroku-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-apps-api-openapi.yml
- filename: heroku-builds-api-openapi.yml
  format: yaml
  label: Heroku Builds API
  slug: heroku-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-builds-api-openapi.yml
- filename: heroku-collaborators-api-openapi.yml
  format: yaml
  label: Heroku Collaborators API
  slug: heroku-collaborators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-collaborators-api-openapi.yml
- filename: heroku-config-vars-api-openapi.yml
  format: yaml
  label: Heroku Config Vars API
  slug: heroku-config-vars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-config-vars-api-openapi.yml
- filename: heroku-domains-api-openapi.yml
  format: yaml
  label: Heroku Domains API
  slug: heroku-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-domains-api-openapi.yml
- filename: heroku-dynos-api-openapi.yml
  format: yaml
  label: Heroku Dynos API
  slug: heroku-dynos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-dynos-api-openapi.yml
- filename: heroku-formation-api-openapi.yml
  format: yaml
  label: Heroku Formation API
  slug: heroku-formation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-formation-api-openapi.yml
- filename: heroku-log-sessions-api-openapi.yml
  format: yaml
  label: Heroku Log Sessions API
  slug: heroku-log-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-log-sessions-api-openapi.yml
- filename: heroku-pipelines-api-openapi.yml
  format: yaml
  label: Heroku Pipelines API
  slug: heroku-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-pipelines-api-openapi.yml
- filename: heroku-regions-api-openapi.yml
  format: yaml
  label: Heroku Regions API
  slug: heroku-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-regions-api-openapi.yml
- filename: heroku-releases-api-openapi.yml
  format: yaml
  label: Heroku Releases API
  slug: heroku-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-releases-api-openapi.yml
- filename: heroku-stacks-api-openapi.yml
  format: yaml
  label: Heroku Stacks API
  slug: heroku-stacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/openapi/heroku-stacks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Heroku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Heroku secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Heroku
provider_slug: heroku
scheme_count: 1
schemes:
- description: Heroku API key or OAuth token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/heroku-platform-api.yml
  type: http
slug: heroku-authentication
source_filename: heroku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heroku-platform-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Heroku API key or OAuth token\n  sources:\n  - openapi/heroku-platform-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heroku/refs/heads/main/authentication/heroku-authentication.yml
summary_line: http · 1 scheme
tags:
- Application Deployment
- Cloud Platform
- DevOps
- PaaS
---
