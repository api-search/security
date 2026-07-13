---
api_key_in: []
api_specs:
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Repositories API
  slug: gitee-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Issues API
  slug: gitee-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Pull Requests API
  slug: gitee-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Users and Organizations API
  slug: gitee-users-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Gists API
  slug: gitee-gists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Enterprises API
  slug: gitee-enterprises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
- filename: gitee-openapi.yml
  format: yaml
  label: Gitee Webhooks API
  slug: gitee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/openapi/gitee-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Gitee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gitee secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gitee
provider_slug: gitee
scheme_count: 3
schemes:
- description: Personal access token supplied as the `access_token` query parameter. This is the predominant auth style in the Gitee Open API v5 - it is present on 236 of 264 operations in the live Swagger definition. Create a token under Gitee account Settings > Private tokens.
  in: query
  name: accessTokenQuery
  parameterName: access_token
  sources:
  - https://gitee.com/api/v5/swagger_doc.json
  type: apiKey
- description: 'The same personal access token may be sent as an `Authorization: Bearer <token>` request header instead of a query parameter.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://gitee.com/api/v5/swagger
  type: http
- authorizationUrl: https://gitee.com/oauth/authorize
  description: Gitee OAuth2 for third-party applications. Register an application to obtain a client id and secret, direct users to the authorize endpoint, and exchange the returned code at the token endpoint (refresh tokens are issued). The authorize endpoint was confirmed live (HTTP 302) on 2026-07-12. The scope list is drawn from Gitee's OAuth documentation; the Swagger definition itself carries no securityDefinitions.
  flow: authorizationCode
  name: oauth2
  refreshUrl: https://gitee.com/oauth/token
  scopes:
  - user_info
  - projects
  - pull_requests
  - issues
  - notes
  - keys
  - hook
  - groups
  - gists
  - enterprises
  - emails
  sources:
  - https://gitee.com/api/v5/oauth_doc
  tokenUrl: https://gitee.com/oauth/token
  type: oauth2
slug: gitee-authentication
source_filename: gitee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live Swagger swagger_doc.json + Gitee OAuth documentation\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\nschemes:\n- name: accessTokenQuery\n  type: apiKey\n  in: query\n  parameterName: access_token\n  description: >-\n    Personal access token supplied as the `access_token` query parameter. This\n    is the predominant auth style in the Gitee Open API v5 - it is present on\n    236 of 264 operations in the live Swagger definition. Create a token under\n    Gitee account Settings > Private tokens.\n  sources:\n  - https://gitee.com/api/v5/swagger_doc.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    The same personal access token may be sent as an\n    `Authorization: Bearer <token>` request header instead of a query\n    parameter.\n  sources:\n  - https://gitee.com/api/v5/swagger\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://gitee.com/oauth/authorize\n\
  \  tokenUrl: https://gitee.com/oauth/token\n  refreshUrl: https://gitee.com/oauth/token\n  scopes:\n  - user_info\n  - projects\n  - pull_requests\n  - issues\n  - notes\n  - keys\n  - hook\n  - groups\n  - gists\n  - enterprises\n  - emails\n  description: >-\n    Gitee OAuth2 for third-party applications. Register an application to obtain\n    a client id and secret, direct users to the authorize endpoint, and exchange\n    the returned code at the token endpoint (refresh tokens are issued).\n    The authorize endpoint was confirmed live (HTTP 302) on 2026-07-12. The\n    scope list is drawn from Gitee's OAuth documentation; the Swagger definition\n    itself carries no securityDefinitions.\n  sources:\n  - https://gitee.com/api/v5/oauth_doc\nnotes: >-\n  Unauthenticated requests are allowed for public reads at a reduced rate limit\n  (60 requests/minute, confirmed via live X-RateLimit-Limit response header).\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitee/refs/heads/main/authentication/gitee-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Code Hosting
- Git
- Git Hosting
- Version Control
- Repositories
- Pull Requests
- Issue Tracking
- DevOps
- Open Source
- China
---
