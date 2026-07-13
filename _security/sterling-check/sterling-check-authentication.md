---
api_key_in: []
api_specs:
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Screenings API
  slug: sterling-check-screenings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Candidates API
  slug: sterling-check-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Packages API
  slug: sterling-check-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Reports API
  slug: sterling-check-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Invites API
  slug: sterling-check-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
- filename: sterling-check-openapi.yml
  format: yaml
  label: Sterling Webhooks API
  slug: sterling-check-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/openapi/sterling-check-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sterling Check Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sterling secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sterling
provider_slug: sterling-check
scheme_count: 2
schemes:
- description: OAuth2 client credentials grant using your Client ID and Client Secret.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.sterlingcheck.app/oauth/token
  name: oAuth2ClientCredentials
  sources:
  - openapi/sterling-check-openapi.yml
  type: oauth2
- description: The access token returned from the OAuth token exchange, sent as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sterling-check-openapi.yml
  type: http
slug: sterling-check-authentication
source_filename: sterling-check-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sterling-check-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sterlingcheck.app/oauth/token\n    scopes: 0\n  description: OAuth2 client credentials grant using your Client ID and Client Secret.\n  sources:\n  - openapi/sterling-check-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: The access token returned from the OAuth token exchange, sent as a Bearer token.\n  sources:\n  - openapi/sterling-check-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sterling-check/refs/heads/main/authentication/sterling-check-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Background Screening
- Identity Verification
- Background Check
- HR Tech
- Compliance
- Gated API
---
