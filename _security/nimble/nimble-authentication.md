---
api_key_in:
- header
api_specs:
- filename: nimble-activities-api-openapi.yml
  format: yaml
  label: Nimble Activities API
  slug: nimble-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-activities-api-openapi.yml
- filename: nimble-contacts-api-openapi.yml
  format: yaml
  label: Nimble Contacts API
  slug: nimble-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-api-openapi.yml
- filename: nimble-contacts-fields-api-openapi.yml
  format: yaml
  label: Nimble Contacts Fields API
  slug: nimble-contacts-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-fields-api-openapi.yml
- filename: nimble-contacts-pipelines-api-openapi.yml
  format: yaml
  label: Nimble Contacts Pipelines API
  slug: nimble-contacts-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-contacts-pipelines-api-openapi.yml
- filename: nimble-deals-api-openapi.yml
  format: yaml
  label: Nimble Deals API
  slug: nimble-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-api-openapi.yml
- filename: nimble-deals-fields-api-openapi.yml
  format: yaml
  label: Nimble Deals Fields API
  slug: nimble-deals-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-fields-api-openapi.yml
- filename: nimble-deals-pipelines-api-openapi.yml
  format: yaml
  label: Nimble Deals Pipelines API
  slug: nimble-deals-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-pipelines-api-openapi.yml
- filename: nimble-deals-pipelines-fields-api-openapi.yml
  format: yaml
  label: Nimble Deals Pipelines Fields API
  slug: nimble-deals-pipelines-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-deals-pipelines-fields-api-openapi.yml
- filename: nimble-leads-api-openapi.yml
  format: yaml
  label: Nimble Leads API
  slug: nimble-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-leads-api-openapi.yml
- filename: nimble-messages-api-openapi.yml
  format: yaml
  label: Nimble Messages API
  slug: nimble-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-messages-api-openapi.yml
- filename: nimble-tasks-api-openapi.yml
  format: yaml
  label: Nimble Tasks API
  slug: nimble-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-tasks-api-openapi.yml
- filename: nimble-users-api-openapi.yml
  format: yaml
  label: Nimble Users API
  slug: nimble-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/openapi/nimble-users-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nimble Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nimble secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nimble
provider_slug: nimble
scheme_count: 3
schemes:
- declared_in_spec: true
  in: header
  name: ApiKey
  parameter: X-Nimble-Token
  sources:
  - openapi/_original/nimble-openapi-original.yml
  type: apiKey
- declared_in_spec: false
  description: '"The only form of accepted authentication is through the HTTP header. Your API request must have an Authorization header with a value like this: Bearer API-KEY." The per-account API key is generated from the Nimble account settings surface.'
  name: BearerToken
  scheme: bearer
  sources:
  - https://support.nimble.com/en/articles/502755-nimble-api-access
  type: http
- audience: third-party developers and older accounts
  client_registration:
    contact: api-support@nimble.com
    process: OAuth client credentials are not self-service. Nimble issues Client ID and Client Secret by email — send App Name, App Description and the OAuth callback Redirect URL to api-support@nimble.com.
    reference: https://support.nimble.com/en/articles/502755-nimble-api-access
    self_service: false
  declared_in_spec: false
  flows:
  - authorizationUrl: https://app.nimble.com/oauth/authorize
    flow: authorizationCode
    refreshUrl: https://app.nimble.com/api/oauth/token
    scopes:
      basic: User and Company info
      contacts: Contacts access
      deals: Deals access
    tokenUrl: https://app.nimble.com/api/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  implicit_note: '"We don''t support Implicit Flow, so `code` is the only available option now."'
  implicit_supported: false
  name: OAuth2
  redirect_uri_note: The authoritative redirect URL is set in the application settings on the developer portal; the redirect_uri request parameter may only overwrite the path portion and must otherwise match exactly.
  response_types:
  - code
  rfc_references:
  - https://tools.ietf.org/html/rfc6749
  - https://tools.ietf.org/html/rfc6750
  scope_delimiter: 'Comma or plus sign: "basic,contacts,deals" or "basic+contacts+deals".'
  sources:
  - https://www.nimble.com/developers/docs/#tag/Authentication
  token_endpoint_auth: client_secret_post
  token_request_content_type: application/x-www-form-urlencoded
  token_response:
    expires_in_seconds: 599
    note: Access tokens are short-lived — roughly 10 minutes — so any long-running agent integration must implement the refresh_token grant rather than caching an access token.
    refresh_token: true
    token_type: bearer
  type: oauth2
slug: nimble-authentication
source_filename: nimble-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/nimble-openapi-original.yml\ndocs: https://www.nimble.com/developers/docs/#tag/Authentication\ndocs_secondary: https://support.nimble.com/en/articles/502755-nimble-api-access\nsummary:\n  types:\n    - apiKey\n    - http\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n  note: >-\n    Nimble runs two parallel authentication models. The machine-readable\n    securitySchemes block declares only the apiKey (X-Nimble-Token header),\n    but the narrative Authentication reference and the support article\n    document a full OAuth 2.0 authorization_code flow with refresh tokens\n    plus a plain Authorization: Bearer <API-KEY> form. The spec under-declares\n    what the API actually accepts; this file is the superset, upgraded from\n    the derived baseline by reading the docs.\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    parameter: X-Nimble-Token\n    declared_in_spec:\
  \ true\n    sources:\n      - openapi/_original/nimble-openapi-original.yml\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    declared_in_spec: false\n    description: >-\n      \"The only form of accepted authentication is through the HTTP header.\n      Your API request must have an Authorization header with a value like\n      this: Bearer API-KEY.\" The per-account API key is generated from the\n      Nimble account settings surface.\n    sources:\n      - https://support.nimble.com/en/articles/502755-nimble-api-access\n  - name: OAuth2\n    type: oauth2\n    declared_in_spec: false\n    audience: third-party developers and older accounts\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.nimble.com/oauth/authorize\n        tokenUrl: https://app.nimble.com/api/oauth/token\n        refreshUrl: https://app.nimble.com/api/oauth/token\n        scopes:\n          basic: User and Company info\n          contacts: Contacts access\n          deals:\
  \ Deals access\n    grant_types:\n      - authorization_code\n      - refresh_token\n    response_types:\n      - code\n    implicit_supported: false\n    implicit_note: >-\n      \"We don't support Implicit Flow, so `code` is the only available\n      option now.\"\n    token_endpoint_auth: client_secret_post\n    token_request_content_type: application/x-www-form-urlencoded\n    token_response:\n      token_type: bearer\n      expires_in_seconds: 599\n      refresh_token: true\n      note: >-\n        Access tokens are short-lived — roughly 10 minutes — so any\n        long-running agent integration must implement the refresh_token grant\n        rather than caching an access token.\n    scope_delimiter: >-\n      Comma or plus sign: \"basic,contacts,deals\" or \"basic+contacts+deals\".\n    redirect_uri_note: >-\n      The authoritative redirect URL is set in the application settings on the\n      developer portal; the redirect_uri request parameter may only overwrite\n      the path\
  \ portion and must otherwise match exactly.\n    client_registration:\n      self_service: false\n      process: >-\n        OAuth client credentials are not self-service. Nimble issues Client ID\n        and Client Secret by email — send App Name, App Description and the\n        OAuth callback Redirect URL to api-support@nimble.com.\n      contact: api-support@nimble.com\n      reference: https://support.nimble.com/en/articles/502755-nimble-api-access\n    rfc_references:\n      - https://tools.ietf.org/html/rfc6749\n      - https://tools.ietf.org/html/rfc6750\n    sources:\n      - https://www.nimble.com/developers/docs/#tag/Authentication\ndiscovery:\n  oauth_metadata_published: false\n  openid_connect: false\n  note: >-\n    No /.well-known/oauth-authorization-server and no\n    /.well-known/openid-configuration on any Nimble host (all 404 — see\n    well-known/nimble-well-known.yml). Endpoints are documented in prose only.\nscopes_reference: scopes/nimble-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble/refs/heads/main/authentication/nimble-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- CRM
- Sales
- Contact Management
- Relationship Management
- Marketing Automation
- Pipeline Management
- Small Business
- Email Marketing
- Sales Automation
- Lead Management
---
