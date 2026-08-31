---
api_key_in:
- header
api_specs:
- filename: splashthat-api.postman_collection.json
  format: json
  label: Splash API
  slug: splash-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/splashthat/refs/heads/main/postman/splashthat-api.postman_collection.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Splashthat Authentication
name_suffix: Authentication
oauth_flows:
- password
- refreshToken
overview: Splash secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refreshToken flow(s).
provider_name: Splash
provider_slug: splashthat
scheme_count: 2
schemes:
- applies_to: https://api.splashthat.com
  errors:
  - description: Invalid username and password combination
    error: invalid_grant
  - description: Invalid refresh token (HTTP 400 on refresh)
    error: invalid_grant
  flows:
  - body_encoding: multipart/form-data
    flow: password
    method: POST
    parameters:
    - client_id
    - client_secret
    - grant_type
    - scope
    - username
    - password
    scopes:
      user: Full user-level access to the authenticated Splash account
    tokenUrl: https://api.splashthat.com/oauth/v2/token
  - flow: refreshToken
    method: GET
    parameters:
    - client_id
    - client_secret
    - grant_type
    - scope
    - refresh_token
    tokenUrl: https://api.splashthat.com/oauth/v2/token
  name: SplashOAuth2
  token:
    alternate_transport: 'The Forms endpoint documentation notes the token may be passed either as an access_token parameter or as a Bearer Authorization header.

      '
    documented_lifetime: 8 hours
    example_expires_in: 604800
    lifetime_note: 'The Authentication folder states the access token "remains valid for the next 8 hours", while the published success example returns expires_in 604800 (7 days). Splash documents both; the conservative assumption for an integration is the 8-hour figure with a refresh flow.

      '
    response_fields:
    - access_token
    - expires_in
    - token_type
    - scope
    - refresh_token
    token_type: bearer
    transport: Authorization header
  type: oauth2
- applies_to: https://splashthat.com/api/v2/crm/events
  in: header
  name: SplashCRMKey
  note: 'Event CREATION runs through a separate CRM API with its own static key, distinct from the OAuth client credentials used everywhere else. Splash documents it as "a potent endpoint" and asks customers to consult their team before using it.

    '
  parameter_name: AUTHORIZATION
  type: apiKey
  value_format: SplashCRM <crm_api_key>
slug: splashthat-authentication
source_filename: splashthat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api-docs.splashthat.com/\ndocs: https://api-docs.splashthat.com/\nartifact_source: postman/splashthat-api.postman_collection.json\nnote: >\n  Derived from Splash's own published Postman collection (\"Splash API v2.2\",\n  public documenter at api-docs.splashthat.com, owner 6088160, published\n  2019-10-22) and its Authentication folder documentation. Splash publishes no\n  OpenAPI, so `derive-authentication.py` produces nothing here; this profile is\n  read from the provider's published request definitions instead. CORRECTION:\n  the Splash token endpoint uses the OAuth 2.0 RESOURCE OWNER PASSWORD\n  CREDENTIALS grant (client_id + client_secret + username + password), not the\n  client_credentials grant.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [password, refreshToken]\n  credential_issuance: manual\n  self_serve: false\n  issuance_note: >\n    A Client ID and Client Secret are obtained\
  \ by contacting a Splash Customer\n    Success Manager and are delivered over a secure cryptographic messaging\n    app. There is no developer self-signup for API credentials. The CRM API key\n    is a separate credential, also issued by the Customer Success Manager.\nschemes:\n  - name: SplashOAuth2\n    type: oauth2\n    applies_to: https://api.splashthat.com\n    flows:\n      - flow: password\n        tokenUrl: https://api.splashthat.com/oauth/v2/token\n        method: POST\n        body_encoding: multipart/form-data\n        parameters:\n          - client_id\n          - client_secret\n          - grant_type\n          - scope\n          - username\n          - password\n        scopes:\n          user: Full user-level access to the authenticated Splash account\n      - flow: refreshToken\n        tokenUrl: https://api.splashthat.com/oauth/v2/token\n        method: GET\n        parameters:\n          - client_id\n          - client_secret\n          - grant_type\n          - scope\n\
  \          - refresh_token\n    token:\n      transport: Authorization header\n      token_type: bearer\n      response_fields: [access_token, expires_in, token_type, scope, refresh_token]\n      documented_lifetime: 8 hours\n      example_expires_in: 604800\n      lifetime_note: >\n        The Authentication folder states the access token \"remains valid for the\n        next 8 hours\", while the published success example returns\n        expires_in 604800 (7 days). Splash documents both; the conservative\n        assumption for an integration is the 8-hour figure with a refresh flow.\n      alternate_transport: >\n        The Forms endpoint documentation notes the token may be passed either as\n        an access_token parameter or as a Bearer Authorization header.\n    errors:\n      - error: invalid_grant\n        description: Invalid username and password combination\n      - error: invalid_grant\n        description: Invalid refresh token (HTTP 400 on refresh)\n  - name: SplashCRMKey\n\
  \    type: apiKey\n    in: header\n    parameter_name: AUTHORIZATION\n    value_format: 'SplashCRM <crm_api_key>'\n    applies_to: https://splashthat.com/api/v2/crm/events\n    note: >\n      Event CREATION runs through a separate CRM API with its own static key,\n      distinct from the OAuth client credentials used everywhere else. Splash\n      documents it as \"a potent endpoint\" and asks customers to consult their\n      team before using it.\nauthorization_model:\n  - scope: user\n    note: The only scope value that appears in Splash's published token requests.\n  - privilege: organization admin\n    note: >\n      The Anonymize Contact endpoint (PUT /contacts/:contact_id/anonymize)\n      requires elevated privileges granted only to organization admins;\n      inadequate privileges surface as HTTP 403.\n  - privilege: Team Users view permission\n    note: >\n      GET /v1/team-manager/users returns 403 when the authenticated user cannot\n      view Team Users.\nunauthenticated_behavior:\n\
  \  status: 401\n  body: '{\"message\":\"Unauthorized\"}'\n  note: >\n    Every path on api.splashthat.com, including /.well-known/* and /openapi.json,\n    answers 401 with this body when no token is presented — observed\n    2026-08-13.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splashthat/refs/heads/main/authentication/splashthat-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Event
- Event Marketing
- Event Management
- Guest Registration
- Ticketing
- Check-In
- Analytics
---
