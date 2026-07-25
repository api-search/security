---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: 8Tracks Authentication
name_suffix: Authentication
oauth_flows: []
overview: 8Tracks declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 8Tracks
provider_slug: 8tracks
scheme_count: 3
schemes:
- alt_in: query
  alt_name: api_key
  description: Per-application key that authenticates the calling client. Accepted as the X-Api-Key header or the api_key query parameter. No new keys issued since 2015-02.
  id: api_key
  in: header
  name: X-Api-Key
  required: true
  type: apiKey
- alt_in: query
  alt_name: api_version
  description: Declares the API version (3 for the latest documented surface). Must be sent on every call, as the X-Api-Version header or the api_version query parameter.
  id: api_version
  in: header
  name: X-Api-Version
  required: true
  type: apiKey
- description: Session token identifying an authenticated end user, required only for user-scoped write actions (like/unlike a mix, fav/unfav a track). Obtained by POST sessions.json with the user's login and password (HTTP Basic), and invalidated by POST logout.
  id: user_token
  in: header
  name: X-User-Token
  required: false
  type: apiKey
slug: 8tracks-authentication
source_filename: 8tracks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: >-\n  8tracks API v3 documentation (https://8tracks.com/developers/api_v3), the\n  \"includes\" reference (https://8tracks.com/developers/includes), and behavior\n  confirmed across community client libraries (dbrgn/orochi, motemen/WebService-8tracks,\n  metacpan WebService::8tracks).\napi: 8tracks API v3\nsummary: >-\n  Application access is by API key, supplied either as an api_key query parameter\n  or an X-Api-Key HTTP header. Every request must also declare the API version via\n  an api_version query parameter or an X-Api-Version header. User-scoped actions\n  (likes, favorites) additionally require a user session token obtained by posting\n  credentials to sessions.json and then sending an X-User-Token header. New API\n  keys have not been issued since February 2015.\nschemes:\n- id: api_key\n  type: apiKey\n  in: header\n  name: X-Api-Key\n  alt_in: query\n  alt_name: api_key\n  required: true\n  description: >-\n  \
  \  Per-application key that authenticates the calling client. Accepted as the\n    X-Api-Key header or the api_key query parameter. No new keys issued since\n    2015-02.\n- id: api_version\n  type: apiKey\n  in: header\n  name: X-Api-Version\n  alt_in: query\n  alt_name: api_version\n  required: true\n  description: >-\n    Declares the API version (3 for the latest documented surface). Must be sent\n    on every call, as the X-Api-Version header or the api_version query parameter.\n- id: user_token\n  type: apiKey\n  in: header\n  name: X-User-Token\n  required: false\n  description: >-\n    Session token identifying an authenticated end user, required only for\n    user-scoped write actions (like/unlike a mix, fav/unfav a track). Obtained by\n    POST sessions.json with the user's login and password (HTTP Basic), and\n    invalidated by POST logout.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nnotes: >-\n  The API predates OAuth 2.0 adoption at 8tracks; there is no documented\
  \ OAuth or\n  OpenID Connect flow. User authentication is a proprietary username/password\n  session exchange returning a user token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8tracks/refs/heads/main/authentication/8tracks-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Music
- Streaming
- Radio
- Playlists
- Audio
- Media
- Entertainment
---
