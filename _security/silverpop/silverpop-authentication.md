---
api_key_in: []
api_specs:
- filename: silverpop-authentication-api-openapi.yml
  format: yaml
  label: Silverpop Authentication API
  slug: silverpop-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-authentication-api-openapi.yml
- filename: silverpop-campaigns-api-openapi.yml
  format: yaml
  label: Silverpop Campaigns API
  slug: silverpop-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-campaigns-api-openapi.yml
- filename: silverpop-contacts-api-openapi.yml
  format: yaml
  label: Silverpop Contacts API
  slug: silverpop-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-contacts-api-openapi.yml
- filename: silverpop-programs-api-openapi.yml
  format: yaml
  label: Silverpop Programs API
  slug: silverpop-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-programs-api-openapi.yml
- filename: silverpop-reports-api-openapi.yml
  format: yaml
  label: Silverpop Reports API
  slug: silverpop-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-reports-api-openapi.yml
- filename: silverpop-transactional-api-openapi.yml
  format: yaml
  label: Silverpop Transactional API
  slug: silverpop-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/openapi/silverpop-transactional-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Silverpop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Silverpop secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Silverpop
provider_slug: silverpop
scheme_count: 2
schemes:
- access_token_ttl: 4 hours
  flow: refresh_token
  name: OAuth2RefreshToken
  presentation: 'Authorization: Bearer <access_token>'
  provisioning:
    client_credentials: Org Admin -> Organization Settings -> Application Account Access -> Add Application. Returns a Client Id and Client Secret, scoped to an APPLICATION.
    refresh_token: Org Admin -> Add Account Access, binding an Application to a user Account. The token is EMAILED to the user who created the request and to the principal org admin. It is never returned by an API call.
  refresh_token_ttl: Non-expiring. "Refresh tokens do not expire unless the user's access is revoked from the Organization's Settings for that application."
  request:
    content_type: application/x-www-form-urlencoded
    parameters:
    - name: grant_type
      required: true
      value: refresh_token
    - name: client_id
      required: true
    - name: client_secret
      required: true
    - name: refresh_token
      required: true
  response:
    access_token: true
    expires_in: 14400
    token_type: bearer
  reuse: Access tokens are reusable within their window and the provider explicitly wants them reused — "OAuth access tokens allow calls to re-use existing tokens if they are still valid so that a new token does not have to be generated with every call." Recommended refresh cadence is every 3 hours.
  revocation: Per refresh token, from Organization Settings. Deleting the token ends a third party's access without rotating a shared password — the provider names this as the main reason to prefer OAuth over the legacy session method.
  scopes: []
  scopes_note: 'There is no scope or consent model. Authorization is inherited wholesale from the Campaign permission set of the user the refresh token is bound to — "we connect users to the application so that we can apply our existing built-in security model as is defined for that user." The practical consequence for an agent integration is that a token cannot be narrowed: whatever that human can do in the UI, including PurgeData and ScheduleMailing, the token can do over the API. No scopes/ artifact was written because there are no scopes to enumerate.'
  sources:
  - https://developer.goacoustic.com/acoustic-campaign/reference/getting-started-with-oauth
  token_endpoint: https://api-campaign-{region}-{pod}.goacoustic.com/oauth/token
  token_endpoint_note: The token endpoint is per-tenant. region and pod come from the organization's Campaign instance (us-1, us-5, eu-1, …), not from a global host.
  type: oauth2
- constraints:
  - No more than 20 active login sessions per organization at any time.
  - Sessions not terminated with the Logout API can remain active for several minutes and block creation of new sessions.
  deprecation: Filed by the provider under "Legacy authentication method" with the instruction that "all users of the Acoustic Campaign XML API are strongly encouraged to use OAuth 2.0 authentication." No retirement date published. See lifecycle/silverpop-lifecycle.yml.
  description: The original session-based authentication for the XML API. Log in, receive a JSESSIONID, pass it on subsequent calls, and call the Logout API to release the session.
  name: JSessionId
  scheme: session-cookie
  sources:
  - https://developer.goacoustic.com/acoustic-campaign/reference/legacy-authentication-method-jsessionid-user-sessions
  - https://developer.goacoustic.com/acoustic-campaign/reference/basics
  status: legacy
  type: http
slug: silverpop-authentication
source_filename: silverpop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.goacoustic.com/acoustic-campaign/reference/getting-started-with-oauth\ndocs:\n- https://developer.goacoustic.com/acoustic-campaign/reference/getting-started-with-oauth\n- https://developer.goacoustic.com/acoustic-campaign/reference/legacy-authentication-method-jsessionid-user-sessions\n- https://developer.goacoustic.com/acoustic-campaign/reference/oauth-token-creation-in-php\n- https://developer.goacoustic.com/acoustic-campaign/reference/basics\nsupersedes: >-\n  A derived profile that read a single `BearerAuth` http/bearer scheme out of the\n  repository's scaffolded OpenAPI. Upgraded from the provider's own OAuth documentation,\n  which is materially richer and contradicts nothing.\nsummary:\n  types:\n  - oauth2\n  - http\n  primary: oauth2\n  grants:\n  - refresh_token\n  scopes: false\n  mfa_for_api: false\nschemes:\n- name: OAuth2RefreshToken\n  type: oauth2\n  flow: refresh_token\n  token_endpoint:\
  \ https://api-campaign-{region}-{pod}.goacoustic.com/oauth/token\n  token_endpoint_note: >-\n    The token endpoint is per-tenant. region and pod come from the organization's Campaign\n    instance (us-1, us-5, eu-1, …), not from a global host.\n  request:\n    content_type: application/x-www-form-urlencoded\n    parameters:\n    - name: grant_type\n      required: true\n      value: refresh_token\n    - name: client_id\n      required: true\n    - name: client_secret\n      required: true\n    - name: refresh_token\n      required: true\n  response:\n    access_token: true\n    expires_in: 14400\n    token_type: bearer\n  presentation: 'Authorization: Bearer <access_token>'\n  access_token_ttl: 4 hours\n  refresh_token_ttl: >-\n    Non-expiring. \"Refresh tokens do not expire unless the user's access is revoked from\n    the Organization's Settings for that application.\"\n  reuse: >-\n    Access tokens are reusable within their window and the provider explicitly wants them\n    reused\
  \ — \"OAuth access tokens allow calls to re-use existing tokens if they are still\n    valid so that a new token does not have to be generated with every call.\" Recommended\n    refresh cadence is every 3 hours.\n  provisioning:\n    client_credentials: >-\n      Org Admin -> Organization Settings -> Application Account Access -> Add Application.\n      Returns a Client Id and Client Secret, scoped to an APPLICATION.\n    refresh_token: >-\n      Org Admin -> Add Account Access, binding an Application to a user Account. The token\n      is EMAILED to the user who created the request and to the principal org admin. It is\n      never returned by an API call.\n  revocation: >-\n    Per refresh token, from Organization Settings. Deleting the token ends a third party's\n    access without rotating a shared password — the provider names this as the main reason\n    to prefer OAuth over the legacy session method.\n  scopes: []\n  scopes_note: >-\n    There is no scope or consent model. Authorization\
  \ is inherited wholesale from the\n    Campaign permission set of the user the refresh token is bound to — \"we connect users\n    to the application so that we can apply our existing built-in security model as is\n    defined for that user.\" The practical consequence for an agent integration is that a\n    token cannot be narrowed: whatever that human can do in the UI, including PurgeData\n    and ScheduleMailing, the token can do over the API. No scopes/ artifact was written\n    because there are no scopes to enumerate.\n  sources:\n  - https://developer.goacoustic.com/acoustic-campaign/reference/getting-started-with-oauth\n- name: JSessionId\n  type: http\n  scheme: session-cookie\n  status: legacy\n  description: >-\n    The original session-based authentication for the XML API. Log in, receive a\n    JSESSIONID, pass it on subsequent calls, and call the Logout API to release the\n    session.\n  constraints:\n  - No more than 20 active login sessions per organization at any time.\n\
  \  - >-\n    Sessions not terminated with the Logout API can remain active for several minutes and\n    block creation of new sessions.\n  deprecation: >-\n    Filed by the provider under \"Legacy authentication method\" with the instruction that\n    \"all users of the Acoustic Campaign XML API are strongly encouraged to use OAuth 2.0\n    authentication.\" No retirement date published. See lifecycle/silverpop-lifecycle.yml.\n  sources:\n  - https://developer.goacoustic.com/acoustic-campaign/reference/legacy-authentication-method-jsessionid-user-sessions\n  - https://developer.goacoustic.com/acoustic-campaign/reference/basics\nguidance:\n- >-\n  Never embed these credentials in an app distributed to end-user devices. The provider\n  states the consequences directly: credentials exposed to attackers, no control over the\n  10-concurrent-request org limit, and loss of API logs for troubleshooting. Put a service\n  you control between the app and this API.\n- >-\n  Because there are no scopes,\
  \ treat the refresh token as a full-privilege credential for\n  the bound user and gate destructive operations in your own layer. The recommended\n  execution contracts are in agentic-access/silverpop-agentic-access.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverpop/refs/heads/main/authentication/silverpop-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- Campaign Management
- Digital Marketing
- Transactional Email
- SMS
- Customer Data
- Contact Management
- Mobile Push
- Marketing Analytics
---
