---
api_key_in:
- header
api_specs:
- filename: bitbucket-cloud-rest-api-openapi.json
  format: json
  label: Bitbucket Cloud REST API
  slug: bitbucket-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/openapi/bitbucket-cloud-rest-api-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Bitbucket Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Bitbucket secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Bitbucket
provider_slug: bitbucket
scheme_count: 3
schemes:
- description: Basic HTTP Authentication as per [RFC-2617](https://tools.ietf.org/html/rfc2617) (Digest not supported). Note that Basic Auth is available only with username and app password as credentials.
  name: basic
  scheme: basic
  sources:
  - openapi/bitbucket-cloud-rest-api-openapi.json
  type: http
- description: OAuth 2 as per [RFC-6749](https://tools.ietf.org/html/rfc6749).
  flows:
  - authorizationUrl: https://bitbucket.org/site/oauth2/authorize
    flow: authorizationCode
    scopes: 26
    tokenUrl: https://bitbucket.org/site/oauth2/access_token
  name: oauth2
  sources:
  - openapi/bitbucket-cloud-rest-api-openapi.json
  type: oauth2
- description: API Keys can be used as Basic HTTP Authentication credentials and provide a substitute for the account's actual username and password. API Keys are only available to team accounts and there is only 1 key per account. API Keys do not support scopes and have therefore access to all contents of the account.
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/bitbucket-cloud-rest-api-openapi.json
  type: apiKey
slug: bitbucket-authentication
source_filename: bitbucket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bitbucket-cloud-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic HTTP Authentication as per [RFC-2617](https://tools.ietf.org/html/rfc2617)\n    (Digest not supported). Note that Basic Auth is available only with username and app password\n    as credentials.\n  sources:\n  - openapi/bitbucket-cloud-rest-api-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bitbucket.org/site/oauth2/authorize\n    tokenUrl: https://bitbucket.org/site/oauth2/access_token\n    scopes: 26\n  description: OAuth 2 as per [RFC-6749](https://tools.ietf.org/html/rfc6749).\n  sources:\n  - openapi/bitbucket-cloud-rest-api-openapi.json\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n\
  \  description: API Keys can be used as Basic HTTP Authentication credentials and provide a substitute\n    for the account's actual username and password. API Keys are only available to team accounts\n    and there is only 1 key per account. API Keys do not support scopes and have therefore access\n    to all contents of the account.\n  sources:\n  - openapi/bitbucket-cloud-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/authentication/bitbucket-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Atlassian
- CI/CD
- Code Collaboration
- Code Review
- DevOps
- Git
- Pull Requests
- Repository Hosting
- Version Control
---
