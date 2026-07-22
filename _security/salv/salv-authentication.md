---
api_key_in: []
api_specs:
- filename: salv-aml-openapi-original.yml
  format: yaml
  label: Salv AML API
  slug: salv-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/openapi/salv-aml-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salv Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Salv secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Salv
provider_slug: salv
scheme_count: 1
schemes:
- description: 'In order to use the API, you need to generate client credentials using [Salv UI](https://demo.salv.com/credentials).

    Never share your secret keys. Keep them guarded and secure.


    We use OAuth2 client credentials flow to issue our API tokens.

    By default our API tokens have expiration time of 50 years, so effectively they never expire.

    Please do not make any assumptions about the content of the acces'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://app.salv.com/oauth/token
  name: OAuth2
  sources:
  - openapi/salv-aml-openapi-original.yml
  type: oauth2
slug: salv-authentication
source_filename: salv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/salv-aml-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.salv.com/oauth/token\n    scopes: 1\n  description: |-\n    In order to use the API, you need to generate client credentials using [Salv UI](https://demo.salv.com/credentials).\n    Never share your secret keys. Keep them guarded and secure.\n\n    We use OAuth2 client credentials flow to issue our API tokens.\n    By default our API tokens have expiration time of 50 years, so effectively they never expire.\n    Please do not make any assumptions about the content of the acces\n  sources:\n  - openapi/salv-aml-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salv/refs/heads/main/authentication/salv-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Anti-Money Laundering
- Financial Crime
- Compliance
- RegTech
- Sanctions Screening
- Transaction Monitoring
- Fraud Prevention
---
