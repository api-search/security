---
api_key_in: []
api_specs:
- filename: lever-data-api-openapi.yml
  format: yaml
  label: Lever Data API
  slug: lever-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-data-api-openapi.yml
- filename: lever-postings-api-openapi.yml
  format: yaml
  label: Lever Postings API
  slug: lever-postings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-postings-api-openapi.yml
- filename: lever-webhooks-asyncapi.yml
  format: yaml
  label: Lever Webhooks
  slug: lever-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/openapi/lever-webhooks-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lever Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lever secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lever
provider_slug: lever-co
scheme_count: 2
schemes:
- description: HTTP Basic authentication using a Lever API key as the username and an empty password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/lever-data-api-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://auth.lever.co/authorize
    flow: authorizationCode
    scopes: 22
    tokenUrl: https://auth.lever.co/oauth/token
  name: OAuth2
  sources:
  - openapi/lever-data-api-openapi.yml
  type: oauth2
slug: lever-co-authentication
source_filename: lever-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lever-data-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a Lever API key as the username and an empty\n    password.\n  sources:\n  - openapi/lever-data-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.lever.co/authorize\n    tokenUrl: https://auth.lever.co/oauth/token\n    scopes: 22\n  sources:\n  - openapi/lever-data-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lever-co/refs/heads/main/authentication/lever-co-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Applicant Tracking
- ATS
- CRM
- Recruiting
- Hiring
- Talent Acquisition
- Human Resources
- HR Tech
- Postings
- Webhooks
- OAuth
---
