---
api_key_in:
- header
api_specs:
- filename: calyptia-cloud-openapi-original.yml
  format: yaml
  label: Calyptia Cloud API
  slug: calyptia-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calyptia/refs/heads/main/openapi/calyptia-cloud-openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Calyptia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Calyptia secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Calyptia
provider_slug: calyptia
scheme_count: 3
schemes:
- name: user
  scheme: bearer
  sources:
  - openapi/calyptia-cloud-openapi-original.yml
  type: http
- in: header
  name: project
  parameter: X-Project-Token
  sources:
  - openapi/calyptia-cloud-openapi-original.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sso.calyptia.com/oauth/token
  - authorizationUrl: https://sso.calyptia.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sso.calyptia.com/oauth/token
  name: auth0
  sources:
  - openapi/calyptia-cloud-openapi-original.yml
  type: oauth2
slug: calyptia-authentication
source_filename: calyptia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/calyptia-cloud-openapi-original.yml\ndocs: https://docs.chronosphere.io/pipeline-cli/authenticate\nnotes: >-\n  Primary auth is the project API token sent as the X-Project-Token header,\n  generated in the Calyptia Cloud UI (core.calyptia.com) / project Settings.\n  User bearer JWTs cover interactive user-scoped calls; the auth0 oauth2 scheme\n  (Auth0 tenant sso.calyptia.com) backs SSO/login. OAuth2 scope maps are empty\n  (coarse-grained authorization) — see scopes/calyptia-scopes.yml.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: user\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/calyptia-cloud-openapi-original.yml\n- name: project\n  type: apiKey\n  in: header\n  parameter: X-Project-Token\n  sources:\n  - openapi/calyptia-cloud-openapi-original.yml\n- name: auth0\n  type: oauth2\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: https://sso.calyptia.com/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: https://sso.calyptia.com/authorize\n    tokenUrl: https://sso.calyptia.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/calyptia-cloud-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calyptia/refs/heads/main/authentication/calyptia-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Infrastructure
- Observability
- Telemetry
- Logging
- Fluent Bit
- Data Pipeline
- Kubernetes
- DevOps
---
