---
api_key_in: []
api_specs:
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Locations API
  slug: shellrecharge-public-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge EV Public Charge Sessions API
  slug: shellrecharge-public-charge-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge OCPI API
  slug: shellrecharge-ocpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tariffs API
  slug: shellrecharge-tariffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
- filename: shellrecharge-openapi.yml
  format: yaml
  label: ShellRecharge Tokens API
  slug: shellrecharge-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/openapi/shellrecharge-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Shellrecharge Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: ShellRecharge secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: ShellRecharge
provider_slug: shellrecharge
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret pair is also required on functional requests.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.shell.com/v1/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/shellrecharge-openapi.yml
  type: oauth2
slug: shellrecharge-authentication
source_filename: shellrecharge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/shellrecharge-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.shell.com/v1/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials grant. A bearer access token is obtained from the\n    Shell SSO token endpoint and sent in the Authorization header; a separate API client id/secret\n    pair is also required on functional requests.\n  sources:\n  - openapi/shellrecharge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shellrecharge/refs/heads/main/authentication/shellrecharge-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- EV Charging
- Electric Vehicles
- Mobility
- Charge Points
- OCPI
- Energy
---
