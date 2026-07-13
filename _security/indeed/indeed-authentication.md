---
api_key_in: []
api_specs:
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Job Sync API
  slug: job-sync
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
- filename: indeed-employer-api-openapi.yml
  format: yaml
  label: Indeed Employer API
  slug: employer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/openapi/indeed-employer-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Indeed Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Indeed secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Indeed
provider_slug: indeed
scheme_count: 2
schemes:
- description: OAuth 2.0 Bearer Token authentication. Obtain access tokens through the Indeed OAuth 2.0 authorization flow using your partner client credentials.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/indeed-employer-api-openapi.yml
  type: http
- description: Indeed OAuth 2.0 authentication for partner applications.
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://apis.indeed.com/oauth/v2/tokens
  name: OAuth2
  sources:
  - openapi/indeed-employer-api-openapi.yml
  type: oauth2
slug: indeed-authentication
source_filename: indeed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/indeed-employer-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer Token authentication. Obtain access tokens through the Indeed\n    OAuth 2.0 authorization flow using your partner client credentials.\n  sources:\n  - openapi/indeed-employer-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.indeed.com/oauth/v2/tokens\n    scopes: 3\n  description: Indeed OAuth 2.0 authentication for partner applications.\n  sources:\n  - openapi/indeed-employer-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/authentication/indeed-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
---
