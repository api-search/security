---
anonymous_access: false
api_key_in: []
api_specs:
- filename: globalping-io-limits-api-openapi.yml
  format: yaml
  label: Globalping Limits API
  slug: globalping-io-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-limits-api-openapi.yml
- filename: globalping-io-measurements-api-openapi.yml
  format: yaml
  label: Globalping Measurements API
  slug: globalping-io-measurements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-measurements-api-openapi.yml
- filename: globalping-io-probes-api-openapi.yml
  format: yaml
  label: Globalping Probes API
  slug: globalping-io-probes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-probes-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Globalping Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Globalping secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Globalping
provider_slug: globalping-io
scheme_count: 2
schemes:
- description: For end users - generate a token in the [Globalping Dashboard](https://dash.globalping.io/tokens) and send it with your requests to get higher limits.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/globalping-io-openapi.yaml
  type: http
- description: 'For developers building applications on top of Globalping - if you want to allow end users to sign in and run measurements under their own accounts,

    we can provide OAuth2 access. Please e-mail d@globalping.io for more information.'
  flows:
  - authorizationUrl: https://auth.globalping.io/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://auth.globalping.io/oauth/token
  name: OAuth2
  sources:
  - openapi/globalping-io-openapi.yaml
  type: oauth2
slug: globalping-io-authentication
source_filename: globalping-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/globalping-io-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: For end users - generate a token in the [Globalping Dashboard](https://dash.globalping.io/tokens)\n    and send it with your requests to get higher limits.\n  sources:\n  - openapi/globalping-io-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.globalping.io/oauth/authorize\n    tokenUrl: https://auth.globalping.io/oauth/token\n    scopes: 1\n  description: |-\n    For developers building applications on top of Globalping - if you want to allow end users to sign in and run measurements under their own accounts,\n    we can provide OAuth2 access. Please e-mail d@globalping.io for more information.\n  sources:\n  - openapi/globalping-io-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/globalping-io/authentication/globalping-io-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Networks
- Monitoring
- Open Source
- Free
---
