---
api_key_in:
- header
api_specs:
- filename: medialab-ai-imgur-api.postman_collection.json
  format: json
  label: Imgur API
  slug: imgur-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/medialab-ai/refs/heads/main/postman/medialab-ai-imgur-api.postman_collection.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Medialab Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- clientCredentials-style
overview: MediaLab.AI secures its APIs with oauth2 and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, and clientCredentials-style flow(s).
provider_name: MediaLab.AI
provider_slug: medialab-ai
scheme_count: 4
schemes:
- api: Genius API
  flows:
  - authorizationUrl: https://api.genius.com/oauth/authorize
    flow: authorizationCode
    grant_type: authorization_code
    response_type: code
    scopes_documented: 4
    tokenUrl: https://api.genius.com/oauth/token
  - authorizationUrl: https://api.genius.com/oauth/authorize
    flow: implicit
    note: Genius documents this browser-only flow but explicitly warns against it - "This mechanism is much less secure than the full code exchange process and should only be used by applications without a server or native platform".
    response_type: token
  name: GeniusOAuth2
  source: https://docs.genius.com/#authentication
  token_presentation:
  - form: 'Authorization: Bearer ACCESS_TOKEN'
    location: header
    preferred: true
  - location: query
    note: supported for GET requests
    parameter: access_token
    preferred: false
  - location: body
    note: supported as a POST body element
    parameter: access_token
    preferred: false
  transport_required: HTTPS
  type: oauth2
- api: Genius API
  description: A per-client access token generated from the Genius API Client management page. Valid only for read-only endpoints that are not restricted by a required scope - it cannot create or manage annotations, vote, or read /account.
  name: GeniusClientAccessToken
  scheme: bearer
  scoped: false
  source: https://docs.genius.com/#access-for-apps-without-users
  type: http
- api: Imgur API
  description: Application-level credential for public read-only and anonymous resources - reading image info, looking up user comments, anonymous image upload, anonymous album creation. Identifies the calling application; grants no account access.
  format: 'Authorization: Client-ID YOUR_CLIENT_ID'
  in: header
  name: ImgurClientID
  name_in_request: Authorization
  source: https://apidocs.imgur.com/#authorization-and-oauth
  type: apiKey
- api: Imgur API
  deprecated_flows:
  - response_type: code
  - response_type: pin
  flows:
  - authorizationUrl: https://api.imgur.com/oauth2/authorize
    flow: implicit
    note: Imgur documents token as the only supported response_type - "Only token should be used, as the other methods have been deprecated." The code and pin response types are deprecated.
    response_type: token
  - flow: refreshToken
    grant_type: refresh_token
    parameters:
    - refresh_token
    - client_id
    - client_secret
    - grant_type
    tokenUrl: https://api.imgur.com/oauth2/token
  name: ImgurOAuth2
  registration_endpoint: https://api.imgur.com/oauth2/addclient
  scopes: none
  scopes_note: Imgur's OAuth 2.0 implementation documents no scope parameter - an authorized access token carries full account access for the granting user.
  source: https://apidocs.imgur.com/#authorization-and-oauth
  token_introspection: https://api.imgur.com/oauth2/secret
  token_lifetimes:
    access_token: 1 month (documented); expires_in returned as 3600 in the example response
    refresh_token: does not expire
  token_presentation:
  - form: 'Authorization: Bearer YOUR_ACCESS_TOKEN'
    location: header
    preferred: true
  transport_required: HTTPS
  type: oauth2
slug: medialab-ai-authentication
source_filename: medialab-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://docs.genius.com/#authentication\ndocs:\n- https://docs.genius.com/#authentication\n- https://apidocs.imgur.com/#authorization-and-oauth\nnote: >-\n  Derived from the providers' published authentication documentation, not from an\n  OpenAPI securitySchemes block - neither Genius nor Imgur publishes an OpenAPI or\n  Swagger definition, so 0-working/derive-authentication.py had no spec to read.\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refreshToken\n  - clientCredentials-style\nschemes:\n- name: GeniusOAuth2\n  api: Genius API\n  type: oauth2\n  source: https://docs.genius.com/#authentication\n  transport_required: HTTPS\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.genius.com/oauth/authorize\n    tokenUrl: https://api.genius.com/oauth/token\n    response_type: code\n    grant_type: authorization_code\n   \
  \ scopes_documented: 4\n  - flow: implicit\n    authorizationUrl: https://api.genius.com/oauth/authorize\n    response_type: token\n    note: >-\n      Genius documents this browser-only flow but explicitly warns against it -\n      \"This mechanism is much less secure than the full code exchange process and\n      should only be used by applications without a server or native platform\".\n  token_presentation:\n  - location: header\n    form: 'Authorization: Bearer ACCESS_TOKEN'\n    preferred: true\n  - location: query\n    parameter: access_token\n    preferred: false\n    note: supported for GET requests\n  - location: body\n    parameter: access_token\n    preferred: false\n    note: supported as a POST body element\n- name: GeniusClientAccessToken\n  api: Genius API\n  type: http\n  scheme: bearer\n  source: https://docs.genius.com/#access-for-apps-without-users\n  description: >-\n    A per-client access token generated from the Genius API Client management page.\n    Valid only\
  \ for read-only endpoints that are not restricted by a required scope -\n    it cannot create or manage annotations, vote, or read /account.\n  scoped: false\n- name: ImgurClientID\n  api: Imgur API\n  type: apiKey\n  in: header\n  name_in_request: Authorization\n  format: 'Authorization: Client-ID YOUR_CLIENT_ID'\n  source: https://apidocs.imgur.com/#authorization-and-oauth\n  description: >-\n    Application-level credential for public read-only and anonymous resources -\n    reading image info, looking up user comments, anonymous image upload, anonymous\n    album creation. Identifies the calling application; grants no account access.\n- name: ImgurOAuth2\n  api: Imgur API\n  type: oauth2\n  source: https://apidocs.imgur.com/#authorization-and-oauth\n  transport_required: HTTPS\n  registration_endpoint: https://api.imgur.com/oauth2/addclient\n  token_introspection: https://api.imgur.com/oauth2/secret\n  flows:\n  - flow: implicit\n    authorizationUrl: https://api.imgur.com/oauth2/authorize\n\
  \    response_type: token\n    note: >-\n      Imgur documents token as the only supported response_type - \"Only token should\n      be used, as the other methods have been deprecated.\" The code and pin response\n      types are deprecated.\n  - flow: refreshToken\n    tokenUrl: https://api.imgur.com/oauth2/token\n    grant_type: refresh_token\n    parameters:\n    - refresh_token\n    - client_id\n    - client_secret\n    - grant_type\n  deprecated_flows:\n  - response_type: code\n  - response_type: pin\n  token_lifetimes:\n    access_token: 1 month (documented); expires_in returned as 3600 in the example response\n    refresh_token: does not expire\n  token_presentation:\n  - location: header\n    form: 'Authorization: Bearer YOUR_ACCESS_TOKEN'\n    preferred: true\n  scopes: none\n  scopes_note: >-\n    Imgur's OAuth 2.0 implementation documents no scope parameter - an authorized\n    access token carries full account access for the granting user.\ncommercial_auth:\n- api: Imgur API\n\
  \  requirement: >-\n    Commercial use must be registered with RapidAPI. The base URL changes to\n    https://imgur-apiv3.p.rapidapi.com/ and an X-Mashape-Key request header carrying\n    the RapidAPI key must be set in addition to the Imgur credential.\n  source: https://apidocs.imgur.com/#commercial-usage\n- api: Genius API\n  requirement: >-\n    \"Commercial use of the Genius API is not allowed without a license.\" Licensing is\n    arranged by contacting api-sales@genius.com.\n  source: https://docs.genius.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medialab-ai/refs/heads/main/authentication/medialab-ai-authentication.yml
summary_line: oauth2/http · 4 schemes
tags:
- Company
- Media
- Social
- Advertising
- Content
- Images
- Music
- Messaging
- Communities
- Holding Company
---
