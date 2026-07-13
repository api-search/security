---
api_key_in: []
api_specs:
- filename: state-street-alpha-data-platform-openapi.yml
  format: yaml
  label: Alpha Data Platform API
  slug: alpha-data-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/openapi/state-street-alpha-data-platform-openapi.yml
- filename: state-street-fund-connect-openapi.yml
  format: yaml
  label: Fund Connect API
  slug: fund-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/openapi/state-street-fund-connect-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: State Street Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: State Street secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: State Street
provider_slug: state-street
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow per RFC 6749 Section 4.4.2. Requires multifactor authentication for all user access.
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: https://api.statestreet.com/oauth/token
  name: OAuth2
  sources:
  - openapi/state-street-alpha-data-platform-openapi.yml
  - openapi/state-street-fund-connect-openapi.yml
  type: oauth2
slug: state-street-authentication
source_filename: state-street-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/state-street-alpha-data-platform-openapi.yml, openapi/state-street-fund-connect-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.statestreet.com/oauth/token\n    scopes: 5\n  description: OAuth 2.0 Client Credentials flow per RFC 6749 Section 4.4.2. Requires multifactor\n    authentication for all user access.\n  sources:\n  - openapi/state-street-alpha-data-platform-openapi.yml\n  - openapi/state-street-fund-connect-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-street/refs/heads/main/authentication/state-street-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Fortune 500
---
