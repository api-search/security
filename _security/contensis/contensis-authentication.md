---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contensis-content-types-api-openapi.yml
  format: yaml
  label: Contensis Content Types API
  slug: contensis-content-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-content-types-api-openapi.yml
- filename: contensis-entries-api-openapi.yml
  format: yaml
  label: Contensis Entries API
  slug: contensis-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-entries-api-openapi.yml
- filename: contensis-projects-api-openapi.yml
  format: yaml
  label: Contensis Projects API
  slug: contensis-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-projects-api-openapi.yml
- filename: contensis-taxonomy-api-openapi.yml
  format: yaml
  label: Contensis Taxonomy API
  slug: contensis-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/openapi/contensis-taxonomy-api-openapi.yml
auth_types: []
description: Contensis runs two different authentication models across its two HTTP APIs, and the gap between them matters. The read-only Delivery API takes a single long-lived, environment-wide access token with no scoping and no expiry documented. The Management API runs OAuth 2.0 client credentials against a per-tenant authorization server, with named scopes and one-hour bearer tokens. The captured OpenAPI declares no securitySchemes at all, so everything here is read from the docs, not derived.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Contensis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contensis declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Contensis
provider_slug: contensis
scheme_count: 3
schemes:
- alternative:
    in: query
    name: accessToken
    note: 'The same token may be passed as an `accessToken` query parameter. That is a real published option and a real risk surface: the credential lands in access logs, referrer headers and browser history.'
  api: Contensis Delivery API
  example_request: 'GET /api/delivery/projects/movieDb/entries/{entryId}

    Authorization: your-access-token-here

    '
  expiry: none documented
  granularity: Environment-wide. One token authorises read access to every project in that environment — there is no per-project or per-content-type read credential.
  id: delivery-access-token
  in: header
  name: Authorization
  rotation: Issued and viewed by a System Administrator from the environment settings screen. No programmatic rotation endpoint is documented.
  scheme_note: The token is sent as the raw Authorization header value — there is no Bearer prefix in the documented example.
  scoped: false
  type: apiKey
- api: Contensis Management API
  content_type: application/x-www-form-urlencoded
  credential_source: client_id and client_secret ("shared secret") are created in the API Management screen of the Contensis management console.
  failures:
  - error: invalid_client
    meaning: Bad client_id / client_secret pair at the token endpoint.
    status: 400
  - meaning: Missing, expired or insufficiently scoped token on a Management API call.
    status: 401
  flow: clientCredentials
  id: management-oauth2-client-credentials
  lifetime_note: Returned as `expires_in`; the documented example value is 3600.
  parameters:
  - grant_type=client_credentials
  - client_id
  - client_secret
  - scope
  presentation: HTTP Authorization header on each Management API request.
  refresh: No refresh token is documented. The guidance is to cache the access token locally and re-request when it expires.
  scopes_artifact: scopes/contensis-scopes.yml
  token_endpoint: https://cms-{alias}.cloud.contensis.com/authenticate/connect/token
  token_endpoint_note: Per-tenant. The docs render it as https://cms-yourcontensis.com/authenticate/connect/token; the real cloud host pattern is cms-{alias}.cloud.contensis.com, as used in Contensis' own CLI documentation.
  token_lifetime_seconds: 3600
  token_type: Bearer
  type: oauth2
- api: Contensis CLI
  id: cli-credentials
  note: The first-party CLI accepts either a user/password pair or the same client-id / shared-secret pair as the Management API, supplied per command or cached per environment. It is not a third scheme, it is a client for the two above.
  type: passthrough
slug: contensis-authentication
source_filename: contensis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Contensis\nproviderId: contensis\ngenerated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.contensis.com/help-and-docs/apis/delivery-http/security/authentication and\n  https://www.contensis.com/help-and-docs/apis/management-http/security/authentication,\n  cross-read against the markdown mirror the provider publishes at\n  https://github.com/contensis/contensis-docs.\ndocs:\n  - https://www.contensis.com/help-and-docs/apis/delivery-http/security/authentication\n  - https://www.contensis.com/help-and-docs/apis/management-http/security/authentication\n  - https://www.contensis.com/help-and-docs/apis/management-http/security/scopes\n  - https://www.contensis.com/help-and-docs/guides/managing-your-environment/environment-access-token\ndescription: >-\n  Contensis runs two different authentication models across its two HTTP APIs, and the gap\n  between them matters. The read-only Delivery\
  \ API takes a single long-lived,\n  environment-wide access token with no scoping and no expiry documented. The Management\n  API runs OAuth 2.0 client credentials against a per-tenant authorization server, with\n  named scopes and one-hour bearer tokens. The captured OpenAPI declares no\n  securitySchemes at all, so everything here is read from the docs, not derived.\nschemes:\n  - id: delivery-access-token\n    api: Contensis Delivery API\n    type: apiKey\n    in: header\n    name: Authorization\n    scheme_note: >-\n      The token is sent as the raw Authorization header value — there is no Bearer prefix\n      in the documented example.\n    alternative:\n      in: query\n      name: accessToken\n      note: >-\n        The same token may be passed as an `accessToken` query parameter. That is a real\n        published option and a real risk surface: the credential lands in access logs,\n        referrer headers and browser history.\n    scoped: false\n    expiry: none documented\n\
  \    rotation: >-\n      Issued and viewed by a System Administrator from the environment settings screen.\n      No programmatic rotation endpoint is documented.\n    granularity: >-\n      Environment-wide. One token authorises read access to every project in that\n      environment — there is no per-project or per-content-type read credential.\n    example_request: |\n      GET /api/delivery/projects/movieDb/entries/{entryId}\n      Authorization: your-access-token-here\n  - id: management-oauth2-client-credentials\n    api: Contensis Management API\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: https://cms-{alias}.cloud.contensis.com/authenticate/connect/token\n    token_endpoint_note: >-\n      Per-tenant. The docs render it as https://cms-yourcontensis.com/authenticate/connect/token;\n      the real cloud host pattern is cms-{alias}.cloud.contensis.com, as used in Contensis'\n      own CLI documentation.\n    content_type: application/x-www-form-urlencoded\n\
  \    parameters:\n      - grant_type=client_credentials\n      - client_id\n      - client_secret\n      - scope\n    credential_source: >-\n      client_id and client_secret (\"shared secret\") are created in the API Management\n      screen of the Contensis management console.\n    token_type: Bearer\n    token_lifetime_seconds: 3600\n    lifetime_note: Returned as `expires_in`; the documented example value is 3600.\n    refresh: >-\n      No refresh token is documented. The guidance is to cache the access token locally and\n      re-request when it expires.\n    presentation: HTTP Authorization header on each Management API request.\n    failures:\n      - status: 400\n        error: invalid_client\n        meaning: Bad client_id / client_secret pair at the token endpoint.\n      - status: 401\n        meaning: Missing, expired or insufficiently scoped token on a Management API call.\n    scopes_artifact: scopes/contensis-scopes.yml\n  - id: cli-credentials\n    api: Contensis CLI\n\
  \    type: passthrough\n    note: >-\n      The first-party CLI accepts either a user/password pair or the same client-id /\n      shared-secret pair as the Management API, supplied per command or cached per\n      environment. It is not a third scheme, it is a client for the two above.\nmtls: not documented\nopenid_connect:\n  discovery: not served\n  note: >-\n    The token path (/authenticate/connect/token) is IdentityServer-shaped, which normally\n    implies a sibling /.well-known/openid-configuration on the tenant host. Contensis does\n    not advertise one from its public domain, and the tenant host is per-customer, so no\n    anonymous discovery document was reachable to probe — see\n    well-known/contensis-well-known.yml.\nfindings:\n  - >-\n    The Delivery API credential is unscoped and environment-wide, with no documented\n    expiry. Anything holding it can read every project in that environment for as long as\n    the token exists. For an agent integration that is the whole\
  \ read surface behind one\n    unrotatable string.\n  - >-\n    Passing the Delivery token as a query parameter is documented as a first-class option.\n    That is the kind of thing an agent will do because it is the easiest path, and it\n    leaks the credential into logs.\n  - >-\n    Management API scopes exist but are few — the published table covers projects and\n    entries only. See scopes/contensis-scopes.yml.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contensis/refs/heads/main/authentication/contensis-authentication.yml
summary_line: 3 schemes
tags:
- CMS
- Content
- Headless CMS
- Content Management
- Digital Experience Platform
- Content Delivery
- Webhooks
- Higher Education
---
