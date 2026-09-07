---
anonymous_access: false
api_key_in: []
api_specs:
- filename: assertible-triggers-api-openapi.yml
  format: yaml
  label: Assertible API
  slug: assertible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/openapi/assertible-triggers-api-openapi.yml
- filename: assertible-deployments-api-openapi.yml
  format: yaml
  label: Assertible Deployments API
  slug: assertible-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/openapi/assertible-deployments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Assertible Authentication
name_suffix: Authentication
oauth_flows: []
overview: Assertible secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Assertible
provider_slug: assertible
scheme_count: 3
schemes:
- applies_to:
  - POST /deployments
  - POST /apis/{serviceId}/run
  description: 'HTTP Basic auth where the username is the Assertible API token

    (`ASSERTIBLE_API_TOKEN`) and the password is left empty.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/assertible-deployments-api-openapi.yml
  - openapi/assertible-triggers-api-openapi.yml
  - https://assertible.com/docs/guide/deployments
  type: http
- applies_to:
  - POST /imports/{importId}/sync
  description: 'HTTP Basic auth where the username is the Assertible sync token

    (`ASSERTIBLE_SYNC_TOKEN`) and the password is left empty. Documented

    separately from the deployments API token in Assertible''s sync guide.'
  name: syncToken
  scheme: basic
  sources:
  - openapi/assertible-sync-api-openapi.yml
  - https://assertible.com/docs/guide/sync
  type: http
- applies_to:
  - POST /apis/{serviceId}/run
  caution: A token in a query string is logged by intermediaries. Prefer HTTP Basic where the caller controls the request.
  description: 'The API access token supplied as a query-string parameter. Documented in the

    Trigger URL Parameters table for callers that cannot send a body or header,

    for example a Heroku deploy hook URL.'
  in: query
  key_name: api_token
  name: apiTokenQuery
  sources:
  - https://assertible.com/docs/guide/automation#trigger-url-parameters
  type: apiKey
slug: assertible-authentication
source_filename: assertible-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://assertible.com/docs/guide/deployments\ndocs:\n- https://assertible.com/docs/guide/deployments\n- https://assertible.com/docs/guide/automation#trigger-url-parameters\n- https://assertible.com/docs/guide/sync\nsummary:\n  types:\n  - http\n  model: >-\n    Every documented Assertible API call authenticates with HTTP Basic, where the\n    username is an Assertible-issued token and the password is left empty. There\n    is no OAuth, no OpenID Connect and no signed-request scheme on Assertible's\n    own API. The trigger URL surface additionally accepts the token as an\n    `api_token` query parameter for callers (such as Heroku deploy hooks) that\n    cannot set a request body or an Authorization header.\n  token_delivery:\n  - HTTP Basic (token as username, empty password)\n  - api_token query parameter (trigger URLs only)\n  observed_401:\n    probed: '2026-09-04'\n    request: POST https://assertible.com/deployments\
  \ (no credentials)\n    http_status: 401\n    body: '{\"code\":\"AuthenticationError\",\"message\":\"Not logged in\"}'\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth where the username is the Assertible API token\n    (`ASSERTIBLE_API_TOKEN`) and the password is left empty.\n  applies_to:\n  - POST /deployments\n  - POST /apis/{serviceId}/run\n  sources:\n  - openapi/assertible-deployments-api-openapi.yml\n  - openapi/assertible-triggers-api-openapi.yml\n  - https://assertible.com/docs/guide/deployments\n- name: syncToken\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth where the username is the Assertible sync token\n    (`ASSERTIBLE_SYNC_TOKEN`) and the password is left empty. Documented\n    separately from the deployments API token in Assertible's sync guide.\n  applies_to:\n  - POST /imports/{importId}/sync\n  sources:\n  - openapi/assertible-sync-api-openapi.yml\n  - https://assertible.com/docs/guide/sync\n\
  - name: apiTokenQuery\n  type: apiKey\n  in: query\n  key_name: api_token\n  description: |-\n    The API access token supplied as a query-string parameter. Documented in the\n    Trigger URL Parameters table for callers that cannot send a body or header,\n    for example a Heroku deploy hook URL.\n  applies_to:\n  - POST /apis/{serviceId}/run\n  caution: >-\n    A token in a query string is logged by intermediaries. Prefer HTTP Basic\n    where the caller controls the request.\n  sources:\n  - https://assertible.com/docs/guide/automation#trigger-url-parameters\nnotes:\n- >-\n  DO NOT confuse https://assertible.com/docs/guide/auth with Assertible's own API\n  authentication. That page documents the auth types (Basic, Digest, API token,\n  OAuth 1.0a, OAuth 2.0, session/cookie, auth HTTP step) that Assertible can use\n  when calling YOUR web service under test. It says nothing about authenticating\n  to Assertible. The pipeline's earlier apis.yml Authentication pointer targeted\n  https://assertible.com/docs/guide/authentication,\
  \ which returns 404.\n- >-\n  Assertible offers encrypted variables for storing tokens, usernames and\n  passwords used by tests. Source https://assertible.com/docs/guide/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assertible/refs/heads/main/authentication/assertible-authentication.yml
summary_line: http · 3 schemes
tags:
- API Testing
- Monitoring
- Quality Assurance
- Testing
- CI/CD
---
