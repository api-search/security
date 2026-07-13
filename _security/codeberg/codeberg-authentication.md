---
api_key_in: []
api_specs:
- filename: codeberg-openapi.yml
  format: yaml
  label: Codeberg Repositories API
  slug: codeberg-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-openapi.yml
- filename: codeberg-openapi.yml
  format: yaml
  label: Codeberg Issues API
  slug: codeberg-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-openapi.yml
- filename: codeberg-openapi.yml
  format: yaml
  label: Codeberg Pull Requests API
  slug: codeberg-pull-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-openapi.yml
- filename: codeberg-openapi.yml
  format: yaml
  label: Codeberg Users and Organizations API
  slug: codeberg-users-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-openapi.yml
- filename: codeberg-openapi.yml
  format: yaml
  label: Codeberg Releases API
  slug: codeberg-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-openapi.yml
- filename: codeberg-openapi.yml
  format: yaml
  label: Codeberg Git Content API
  slug: codeberg-git-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/openapi/codeberg-openapi.yml
auth_types:
- apiKey
- basic
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Codeberg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codeberg secures its APIs with apiKey, basic, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Codeberg
provider_slug: codeberg
scheme_count: 3
schemes:
- description: 'Personal access token (PAT). Must be prepended with the word "token" followed by a space, e.g. `Authorization: token YOUR_TOKEN`. Create tokens in Codeberg account settings under Applications.'
  in: header
  name: AuthorizationHeaderToken
  parameterName: Authorization
  sources:
  - https://codeberg.org/swagger.v1.json
  - https://docs.codeberg.org/advanced/api-usage/
  type: apiKey
- description: Codeberg (Forgejo) can act as an OAuth2 provider so third-party applications can obtain access on a user's behalf. Register an OAuth2 application under the user or organization settings.
  name: OAuth2
  sources:
  - https://docs.codeberg.org/advanced/api-usage/
  type: oauth2
- description: HTTP Basic authentication with username and password. When two-factor authentication is enabled it must be combined with a one-time password sent in the `X-FORGEJO-OTP` header.
  name: BasicAuth
  sources:
  - https://codeberg.org/swagger.v1.json
  type: basic
slug: codeberg-authentication
source_filename: codeberg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: https://codeberg.org/swagger.v1.json\nsummary:\n  types:\n  - apiKey\n  - basic\n  - oauth2\nschemes:\n- name: AuthorizationHeaderToken\n  type: apiKey\n  in: header\n  parameterName: Authorization\n  description: 'Personal access token (PAT). Must be prepended with the word \"token\"\n    followed by a space, e.g. `Authorization: token YOUR_TOKEN`. Create tokens in\n    Codeberg account settings under Applications.'\n  sources:\n  - https://codeberg.org/swagger.v1.json\n  - https://docs.codeberg.org/advanced/api-usage/\n- name: OAuth2\n  type: oauth2\n  description: Codeberg (Forgejo) can act as an OAuth2 provider so third-party\n    applications can obtain access on a user's behalf. Register an OAuth2\n    application under the user or organization settings.\n  sources:\n  - https://docs.codeberg.org/advanced/api-usage/\n- name: BasicAuth\n  type: basic\n  description: HTTP Basic authentication with username and password.\
  \ When two-factor\n    authentication is enabled it must be combined with a one-time password sent in\n    the `X-FORGEJO-OTP` header.\n  sources:\n  - https://codeberg.org/swagger.v1.json\nnotes: >-\n  Token auth (Authorization header, prefixed with \"token\") is the recommended\n  method for API access. Public repository reads are largely available\n  unauthenticated. The Sudo header/param and admin-only schemes documented in the\n  Forgejo Swagger are omitted here as they require instance-admin privileges not\n  available to general Codeberg users.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codeberg/refs/heads/main/authentication/codeberg-authentication.yml
summary_line: apiKey/basic/oauth2 · 3 schemes
tags:
- Code Hosting
- Git
- Git Hosting
- Version Control
- Repositories
- Pull Requests
- Issue Tracking
- Open Source
- Forgejo
- Non-Profit
---
