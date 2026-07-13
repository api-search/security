---
api_key_in: []
api_specs:
- filename: mongodb-atlas-openapi.yaml
  format: yaml
  label: MongoDB Atlas Administration API
  slug: mongodb-atlas-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mongodb/refs/heads/main/openapi/mongodb-atlas-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mongodb Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: MongoDB secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: MongoDB
provider_slug: mongodb
scheme_count: 2
schemes:
- name: DigestAuth
  scheme: digest
  sources:
  - openapi/mongodb-atlas-openapi.yaml
  type: http
- description: Learn more about [Service Accounts](https://www.mongodb.com/docs/atlas/api/service-accounts-overview).
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://cloud.mongodb.com/api/oauth/token
  name: ServiceAccounts
  sources:
  - openapi/mongodb-atlas-openapi.yaml
  type: oauth2
slug: mongodb-authentication
source_filename: mongodb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mongodb-atlas-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: DigestAuth\n  type: http\n  scheme: digest\n  sources:\n  - openapi/mongodb-atlas-openapi.yaml\n- name: ServiceAccounts\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://cloud.mongodb.com/api/oauth/token\n    scopes: 0\n  description: Learn more about [Service Accounts](https://www.mongodb.com/docs/atlas/api/service-accounts-overview).\n  sources:\n  - openapi/mongodb-atlas-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mongodb/refs/heads/main/authentication/mongodb-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud Database
- Database
- Document Database
- NoSQL
---
