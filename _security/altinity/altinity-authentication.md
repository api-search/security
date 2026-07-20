---
api_key_in:
- header
api_specs:
- filename: altinity-acm-openapi-original.json
  format: json
  label: Altinity Cloud Manager API
  slug: altinity-cloud-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/altinity/refs/heads/main/openapi/altinity-acm-openapi-original.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Altinity Authentication
name_suffix: Authentication
oauth_flows:
- auth0-sso
overview: Altinity secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the auth0-sso flow(s).
provider_name: Altinity
provider_slug: altinity
scheme_count: 2
schemes:
- in: header
  key_types:
  - ACM API key (My Account > API Access; default 24h expiry, adjustable)
  - Login token (POST /login)
  - Anywhere API token (single per account)
  name: ApiKeyAuth
  parameter: X-Auth-Token
  sources:
  - openapi/altinity-acm-openapi-original.json
  type: apiKey
- flow: token-exchange
  name: Auth0SSO
  operations:
  - GetSingleAuth
  - DoSingleAuth
  provider: Auth0
  sources:
  - docs.altinity.com
  type: oauth2
slug: altinity-authentication
source_filename: altinity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/altinity-acm-openapi-original.json\ndocs: https://docs.altinity.com/altinitycloud/administratorguide/acm-api-quickstart/\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - auth0-sso\n  notes: >-\n    Primary auth is an ACM API key (or login token) passed in the X-Auth-Token\n    header. Single sign-on is available via Auth0 oAuth token exchange\n    (GetSingleAuth / DoSingleAuth). 2FA is supported via LoginVerify.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  key_types:\n  - ACM API key (My Account > API Access; default 24h expiry, adjustable)\n  - Login token (POST /login)\n  - Anywhere API token (single per account)\n  sources:\n  - openapi/altinity-acm-openapi-original.json\n- name: Auth0SSO\n  type: oauth2\n  provider: Auth0\n  flow: token-exchange\n  operations:\n  - GetSingleAuth\n  - DoSingleAuth\n  sources:\n  - docs.altinity.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altinity/refs/heads/main/authentication/altinity-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Big Data
- ClickHouse
- Analytics
- Database
- Managed Cloud
- Kubernetes
- Real-Time Analytics
- Open Source
---
