---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openhandle-openapi.yml
  format: yaml
  label: Openhandle API
  slug: openhandle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openhandle/refs/heads/main/openapi/openhandle-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Openhandle Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Openhandle secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Openhandle
provider_slug: openhandle
scheme_count: 2
schemes:
- description: Use an oh_test_ key for synthetic data and $0.000 actual charges, or an oh_live_ key for real public data and normal billing. Legacy oh_ keys remain Live.
  name: OpenhandleKey
  scheme: bearer
  sources:
  - openapi/openhandle-openapi.yml
  type: http
- description: OAuth grants for the MCP endpoint only. REST operations require OpenhandleKey.
  flows:
  - authorizationUrl: https://api.openhandle.dev/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.openhandle.dev/oauth/token
  name: OpenhandleMCPOAuth
  sources:
  - openapi/openhandle-openapi.yml
  type: oauth2
slug: openhandle-authentication
source_filename: openhandle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: searched\nsource: https://openhandle.dev/docs/authentication\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  note: REST operations use a Bearer API key (OpenhandleKey); the key prefix oh_test_/oh_live_ selects\n    the Test or Live environment and is immutable. OAuth 2.0 (PKCE) applies only to the MCP endpoint.\n    Keys are shown once at creation; call from a backend only.\nschemes:\n- name: OpenhandleKey\n  type: http\n  scheme: bearer\n  description: Use an oh_test_ key for synthetic data and $0.000 actual charges, or an oh_live_ key for\n    real public data and normal billing. Legacy oh_ keys remain Live.\n  sources:\n  - openapi/openhandle-openapi.yml\n- name: OpenhandleMCPOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.openhandle.dev/oauth/authorize\n    tokenUrl: https://api.openhandle.dev/oauth/token\n    scopes: 4\n  description: OAuth grants for the\
  \ MCP endpoint only. REST operations require OpenhandleKey.\n  sources:\n  - openapi/openhandle-openapi.yml\ndocs: https://openhandle.dev/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openhandle/refs/heads/main/authentication/openhandle-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Social Data
- Instagram
- TikTok
- twitter
- Reddit
- Public Data
- social-media-api
- MCP
- creator-analytics
- Social Listening
---
