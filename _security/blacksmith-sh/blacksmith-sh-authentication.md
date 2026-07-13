---
api_key_in: []
api_specs:
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith GitHub Actions Runners
  slug: github-actions-runners
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith Docker Builds
  slug: docker-builds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
- filename: blacksmith-sh-openapi.yml
  format: yaml
  label: Blacksmith Cache
  slug: cache
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/openapi/blacksmith-sh-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Blacksmith Sh Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Blacksmith secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Blacksmith
provider_slug: blacksmith-sh
scheme_count: 1
schemes:
- description: Access to Blacksmith is authorized through the Blacksmith GitHub App installed on a GitHub organization, not via a public API key or bearer token. There is no documented machine-to-machine API auth scheme.
  flows:
  - authorizationUrl: https://github.com/apps/blacksmith
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://github.com/login/oauth/access_token
  name: githubApp
  sources:
  - openapi/blacksmith-sh-openapi.yml
  type: oauth2
slug: blacksmith-sh-authentication
source_filename: blacksmith-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blacksmith-sh-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: githubApp\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://github.com/apps/blacksmith\n    tokenUrl: https://github.com/login/oauth/access_token\n    scopes: 0\n  description: Access to Blacksmith is authorized through the Blacksmith GitHub App installed\n    on a GitHub organization, not via a public API key or bearer token. There is no documented\n    machine-to-machine API auth scheme.\n  sources:\n  - openapi/blacksmith-sh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blacksmith-sh/refs/heads/main/authentication/blacksmith-sh-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CI/CD
- GitHub Actions
- Runners
- Caching
- Docker
---
