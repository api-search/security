---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: trello-webhooks-asyncapi.yml
  format: yaml
  label: Trello Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/asyncapi/trello-webhooks-asyncapi.yml
- filename: trello-actions-api-openapi.yml
  format: yaml
  label: trello Actions API
  slug: trello-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-actions-api-openapi.yml
- filename: trello-boards-api-openapi.yml
  format: yaml
  label: trello Boards API
  slug: trello-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-boards-api-openapi.yml
- filename: trello-cards-api-openapi.yml
  format: yaml
  label: trello Cards API
  slug: trello-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-cards-api-openapi.yml
- filename: trello-checklists-api-openapi.yml
  format: yaml
  label: trello Checklists API
  slug: trello-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-checklists-api-openapi.yml
- filename: trello-labels-api-openapi.yml
  format: yaml
  label: trello Labels API
  slug: trello-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-labels-api-openapi.yml
- filename: trello-lists-api-openapi.yml
  format: yaml
  label: trello Lists API
  slug: trello-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-lists-api-openapi.yml
- filename: trello-members-api-openapi.yml
  format: yaml
  label: trello Members API
  slug: trello-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-members-api-openapi.yml
- filename: trello-notifications-api-openapi.yml
  format: yaml
  label: trello Notifications API
  slug: trello-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-notifications-api-openapi.yml
- filename: trello-organizations-api-openapi.yml
  format: yaml
  label: trello Organizations API
  slug: trello-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-organizations-api-openapi.yml
- filename: trello-plugins-api-openapi.yml
  format: yaml
  label: trello Plugins API
  slug: trello-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-plugins-api-openapi.yml
- filename: trello-search-api-openapi.yml
  format: yaml
  label: trello Search API
  slug: trello-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-search-api-openapi.yml
- filename: trello-tokens-api-openapi.yml
  format: yaml
  label: trello Tokens API
  slug: trello-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-tokens-api-openapi.yml
- filename: trello-webhooks-api-openapi.yml
  format: yaml
  label: trello Webhooks API
  slug: trello-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-webhooks-api-openapi.yml
- filename: trello-custom-fields-api-openapi.yml
  format: yaml
  label: Trello Custom Fields API
  slug: trello-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-custom-fields-api-openapi.yml
- filename: trello-rest-api-openapi.json
  format: json
  label: Trello REST API
  slug: trello-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/openapi/trello-rest-api-openapi.json
auth_types:
- apiKey
- oauth2
description: Trello runs two authorization systems side by side. The legacy Trello Auth system passes an API key and a user token, by default as QUERY PARAMETERS - which is what both apiKey schemes in the OpenAPI declare, and which puts credentials in logs, proxies and browser history. Trello also documents an Authorization header form (OAuth oauth_consumer_key="{key}", oauth_token="{token}") and a request-body form, and an agent should prefer the header. OAuth 2.0 3LO reached GA on 2026-09-15 with ten granular scopes, short-lived refreshable tokens and resource restrictions; see scopes/trello-scopes.yml. OAuth 1.0a is also still supported. Tokens are user-revocable at https://trello.com/u/{username}/account and via DELETE /1/tokens/{token}; a revoked token returns HTTP 401 with the plain-text body "invalid token".
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Trello Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Trello secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Trello
provider_slug: trello
scheme_count: 3
schemes:
- description: Your Trello API key, obtained from the Power-Ups admin page at https://trello.com/power-ups/admin.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/trello-actions-api-openapi.yml
  - openapi/trello-boards-api-openapi.yml
  - openapi/trello-cards-api-openapi.yml
  - openapi/trello-checklists-api-openapi.yml
  - openapi/trello-custom-fields-api-openapi.yml
  - openapi/trello-labels-api-openapi.yml
  - openapi/trello-lists-api-openapi.yml
  - openapi/trello-members-api-openapi.yml
  - openapi/trello-notifications-api-openapi.yml
  - openapi/trello-organizations-api-openapi.yml
  - openapi/trello-plugins-api-openapi.yml
  - openapi/trello-rest-api-openapi.json
  - openapi/trello-search-api-openapi.yml
  - openapi/trello-tokens-api-openapi.yml
  - openapi/trello-webhooks-api-openapi.yml
  type: apiKey
- description: A user token that grants access to Trello resources. Obtained by authorizing via the /1/authorize route or OAuth 1.0.
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/trello-actions-api-openapi.yml
  - openapi/trello-boards-api-openapi.yml
  - openapi/trello-cards-api-openapi.yml
  - openapi/trello-checklists-api-openapi.yml
  - openapi/trello-custom-fields-api-openapi.yml
  - openapi/trello-labels-api-openapi.yml
  - openapi/trello-lists-api-openapi.yml
  - openapi/trello-members-api-openapi.yml
  - openapi/trello-notifications-api-openapi.yml
  - openapi/trello-organizations-api-openapi.yml
  - openapi/trello-plugins-api-openapi.yml
  - openapi/trello-rest-api-openapi.json
  - openapi/trello-search-api-openapi.yml
  - openapi/trello-tokens-api-openapi.yml
  - openapi/trello-webhooks-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://auth.atlassian.com/authorize
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://auth.atlassian.com/authorize/oauth/token
  name: OAuth2
  sources:
  - openapi/trello-rest-api-openapi.json
  type: oauth2
slug: trello-authentication
source_filename: trello-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\ndocs: https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/\noauth2_docs: https://developer.atlassian.com/cloud/trello/guides/rest-api/oauth-2-getting-started/\ndescription: >-\n  Trello runs two authorization systems side by side. The legacy Trello Auth system passes an\n  API key and a user token, by default as QUERY PARAMETERS - which is what both apiKey schemes\n  in the OpenAPI declare, and which puts credentials in logs, proxies and browser history.\n  Trello also documents an Authorization header form\n  (OAuth oauth_consumer_key=\"{key}\", oauth_token=\"{token}\") and a request-body form, and an\n  agent should prefer the header. OAuth 2.0 3LO reached GA on 2026-09-15 with ten granular\n  scopes, short-lived refreshable tokens and resource restrictions; see\n  scopes/trello-scopes.yml. OAuth 1.0a is also still supported. Tokens are user-revocable at\n  https://trello.com/u/{username}/account and via DELETE\
  \ /1/tokens/{token}; a revoked token\n  returns HTTP 401 with the plain-text body \"invalid token\".\nsource: openapi/trello-actions-api-openapi.yml, openapi/trello-boards-api-openapi.yml, openapi/trello-cards-api-openapi.yml,\n  openapi/trello-checklists-api-openapi.yml, openapi/trello-custom-fields-api-openapi.yml, openapi/trello-labels-api-openapi.yml,\n  openapi/trello-lists-api-openapi.yml, openapi/trello-members-api-openapi.yml, openapi/trello-notifications-api-openapi.yml,\n  openapi/trello-organizations-api-openapi.yml, openapi/trello-plugins-api-openapi.yml, openapi/trello-rest-api-openapi.json\n  ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: Your Trello API key, obtained from the Power-Ups admin page at https://trello.com/power-ups/admin.\n  sources:\n  - openapi/trello-actions-api-openapi.yml\n  - openapi/trello-boards-api-openapi.yml\n\
  \  - openapi/trello-cards-api-openapi.yml\n  - openapi/trello-checklists-api-openapi.yml\n  - openapi/trello-custom-fields-api-openapi.yml\n  - openapi/trello-labels-api-openapi.yml\n  - openapi/trello-lists-api-openapi.yml\n  - openapi/trello-members-api-openapi.yml\n  - openapi/trello-notifications-api-openapi.yml\n  - openapi/trello-organizations-api-openapi.yml\n  - openapi/trello-plugins-api-openapi.yml\n  - openapi/trello-rest-api-openapi.json\n  - openapi/trello-search-api-openapi.yml\n  - openapi/trello-tokens-api-openapi.yml\n  - openapi/trello-webhooks-api-openapi.yml\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: A user token that grants access to Trello resources. Obtained by authorizing\n    via the /1/authorize route or OAuth 1.0.\n  sources:\n  - openapi/trello-actions-api-openapi.yml\n  - openapi/trello-boards-api-openapi.yml\n  - openapi/trello-cards-api-openapi.yml\n  - openapi/trello-checklists-api-openapi.yml\n  - openapi/trello-custom-fields-api-openapi.yml\n\
  \  - openapi/trello-labels-api-openapi.yml\n  - openapi/trello-lists-api-openapi.yml\n  - openapi/trello-members-api-openapi.yml\n  - openapi/trello-notifications-api-openapi.yml\n  - openapi/trello-organizations-api-openapi.yml\n  - openapi/trello-plugins-api-openapi.yml\n  - openapi/trello-rest-api-openapi.json\n  - openapi/trello-search-api-openapi.yml\n  - openapi/trello-tokens-api-openapi.yml\n  - openapi/trello-webhooks-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.atlassian.com/authorize\n    tokenUrl: https://auth.atlassian.com/authorize/oauth/token\n    scopes: 10\n  sources:\n  - openapi/trello-rest-api-openapi.json\napi_key:\n  issuance: https://trello.com/apps/admin\n  note: >-\n    An API key is tied to a Power-Up. Trello states the key may be public but the user token\n    must never be, and that a key with no allowed origins configured will have every redirect\n    blocked.\n  allowed_origins:\n\
  \    required: true\n    wildcards: true\n    note: >-\n      Allowed origins constrain where Trello will redirect after consent, preventing a third\n      party from reusing your key and redirecting users elsewhere.\noauth1:\n  supported: true\n  request_token_url: https://trello.com/1/OAuthGetRequestToken\n  authorize_url: https://trello.com/1/OAuthAuthorizeToken\n  access_token_url: https://trello.com/1/OAuthGetAccessToken\nrevocation:\n  user_surface: https://trello.com/u/{username}/account\n  api: DELETE /1/tokens/{token}\n  on_revoked_status: 401\n  on_revoked_body: invalid token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trello/refs/heads/main/authentication/trello-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Project Management
- Kanban
- Task Management
- Collaboration
- Productivity
- Workflows
- Boards
- Atlassian
---
