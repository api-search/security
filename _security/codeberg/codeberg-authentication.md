---
anonymous_access: false
api_key_in: []
api_specs:
- filename: codeberg-miscellaneous-api-openapi.yml
  format: yaml
  label: Codeberg Miscellaneous API
  slug: codeberg-miscellaneous-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-miscellaneous-api-openapi.yml
- filename: codeberg-activitypub-api-openapi.yml
  format: yaml
  label: Codeberg Activitypub API
  slug: codeberg-activitypub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-activitypub-api-openapi.yml
- filename: codeberg-admin-api-openapi.yml
  format: yaml
  label: Codeberg Admin API
  slug: codeberg-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-admin-api-openapi.yml
- filename: codeberg-issue-api-openapi.yml
  format: yaml
  label: Codeberg Issue API
  slug: codeberg-issue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-issue-api-openapi.yml
- filename: codeberg-notification-api-openapi.yml
  format: yaml
  label: Codeberg Notification API
  slug: codeberg-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-notification-api-openapi.yml
- filename: codeberg-organization-api-openapi.yml
  format: yaml
  label: Codeberg Organization API
  slug: codeberg-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-organization-api-openapi.yml
- filename: codeberg-package-api-openapi.yml
  format: yaml
  label: Codeberg Package API
  slug: codeberg-package-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-package-api-openapi.yml
- filename: codeberg-repository-api-openapi.yml
  format: yaml
  label: Codeberg Repository API
  slug: codeberg-repository-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-repository-api-openapi.yml
- filename: codeberg-settings-api-openapi.yml
  format: yaml
  label: Codeberg Settings API
  slug: codeberg-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-settings-api-openapi.yml
- filename: codeberg-user-api-openapi.yml
  format: yaml
  label: Codeberg User API
  slug: codeberg-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/codeberg/openapi/codeberg-user-api-openapi.yml
auth_types:
- apiKey
- basic
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
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
source_yaml_url: https://artifacts.apis.io/codeberg/authentication/codeberg-authentication.yml
summary_line: apiKey/basic/oauth2 · 3 schemes
tags:
- Code Hosting
- Version Control
- Git Hosting
- Repositories
- Pull Requests
- Issue Tracking
- Open Source
- Forgejo
- Non-Profit
---
