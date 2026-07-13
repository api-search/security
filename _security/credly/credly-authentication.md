---
api_key_in: []
api_specs:
- filename: credly-openapi.yml
  format: yaml
  label: Credly Badge Templates API
  slug: credly-badge-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Issued Badges API
  slug: credly-issued-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Organizations API
  slug: credly-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly Events and Webhooks API
  slug: credly-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
- filename: credly-openapi.yml
  format: yaml
  label: Credly OBI Recipients API
  slug: credly-obi-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/openapi/credly-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Credly Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Credly secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Credly
provider_slug: credly
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using the organization's authorization_token as the username and a blank password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/credly-openapi.yml
  type: http
- description: OAuth 2.0 client_credentials grant. Tokens are short-lived (2 hours) and sent as a Bearer token.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://api.credly.com/oauth/token
  name: oauth2
  sources:
  - openapi/credly-openapi.yml
  type: oauth2
slug: credly-authentication
source_filename: credly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/credly-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using the organization's authorization_token as the\n    username and a blank password.\n  sources:\n  - openapi/credly-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.credly.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 client_credentials grant. Tokens are short-lived (2 hours) and sent\n    as a Bearer token.\n  sources:\n  - openapi/credly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credly/refs/heads/main/authentication/credly-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Digital Credentials
- Open Badges
- Badging
- Certifications
- Verifiable Credentials
- Pearson
---
