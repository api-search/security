---
api_key_in: []
api_specs:
- filename: upwork-authentication-api-openapi.yml
  format: yaml
  label: Upwork Authentication API
  slug: upwork-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-authentication-api-openapi.yml
- filename: upwork-contracts-api-openapi.yml
  format: yaml
  label: Upwork Contracts API
  slug: upwork-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-contracts-api-openapi.yml
- filename: upwork-jobs-api-openapi.yml
  format: yaml
  label: Upwork Jobs API
  slug: upwork-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-jobs-api-openapi.yml
- filename: upwork-messages-api-openapi.yml
  format: yaml
  label: Upwork Messages API
  slug: upwork-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-messages-api-openapi.yml
- filename: upwork-organizations-api-openapi.yml
  format: yaml
  label: Upwork Organizations API
  slug: upwork-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-organizations-api-openapi.yml
- filename: upwork-profiles-api-openapi.yml
  format: yaml
  label: Upwork Profiles API
  slug: upwork-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-profiles-api-openapi.yml
- filename: upwork-reports-api-openapi.yml
  format: yaml
  label: Upwork Reports API
  slug: upwork-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/openapi/upwork-reports-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Upwork Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Upwork secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Upwork
provider_slug: upwork
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow for Upwork API access. Obtain an authorization code by redirecting users to the Upwork OAuth consent page, then exchange for access and refresh tokens.
  flows:
  - authorizationUrl: https://www.upwork.com/ab/account-security/oauth2/authorize
    flow: authorizationCode
    scopes: 9
    tokenUrl: https://www.upwork.com/api/v3/oauth2/token
  name: oauth2AuthCode
  sources:
  - openapi/upwork-graphql-api-openapi.yml
  - openapi/upwork-rest-api-openapi.yml
  type: oauth2
slug: upwork-authentication
source_filename: upwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/upwork-graphql-api-openapi.yml, openapi/upwork-rest-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.upwork.com/ab/account-security/oauth2/authorize\n    tokenUrl: https://www.upwork.com/api/v3/oauth2/token\n    scopes: 9\n  description: OAuth 2.0 authorization code flow for Upwork API access. Obtain an authorization\n    code by redirecting users to the Upwork OAuth consent page, then exchange for access and\n    refresh tokens.\n  sources:\n  - openapi/upwork-graphql-api-openapi.yml\n  - openapi/upwork-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwork/refs/heads/main/authentication/upwork-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Freelancing
- Jobs
- Talent
- Marketplace
- Contracts
- Hiring
---
