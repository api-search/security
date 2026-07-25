---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Attendease Authentication
name_suffix: Authentication
oauth_flows: []
overview: Attendease declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Attendease
provider_slug: attendease
scheme_count: 4
schemes:
- api: Attendease Organization API
  format: APIAuth <access_key>:<signature>
  header: Authorization
  id: org_api_hmac
  scheme: hmac-sha1
  signing:
    algorithm: HMAC-SHA1
    canonical_string: content-type,content-MD5,request-URI,timestamp
    content_md5: base64 MD5 of request body (PUT/POST only; empty for GET)
    encoding: base64
    notes: Query strings are part of the request URI but are not factored into the Content-MD5. Signature = Base64.strict_encode64(HMAC-SHA1(secret_key, canonical_string)).
    timestamp_format: RFC 1123
    timestamp_header: Date
    timestamp_skew_minutes: 15
  type: http
- alt_in: query
  alt_name: attendee_token
  api: Attendease Event API
  description: Per-attendee access token scoped to a single event.
  id: event_attendee_token
  in: header
  name: X-Attendee-Token
  type: apiKey
- api: Attendease Event API
  description: Event-level access token scoped to a single event subdomain.
  id: event_token
  in: header
  name: X-Event-Token
  type: apiKey
- api: Attendease Event API
  description: HTTP Basic auth with email/password (also accepted as query params).
  id: event_basic
  scheme: basic
  type: http
slug: attendease-authentication
source_filename: attendease-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developer.attendease.com/\ndocs: https://developer.attendease.com/\nsummary: >-\n  Attendease exposes two authentication models. The Organization API (/api/v2/)\n  uses HMAC-SHA1 request signing with an Access Key ID and Secret Access Token.\n  The Event API uses per-event attendee/event tokens (query params or headers)\n  and also accepts HTTP Basic auth. All requests must use HTTPS.\nschemes:\n- id: org_api_hmac\n  api: Attendease Organization API\n  type: http\n  scheme: hmac-sha1\n  header: Authorization\n  format: 'APIAuth <access_key>:<signature>'\n  signing:\n    algorithm: HMAC-SHA1\n    encoding: base64\n    canonical_string: content-type,content-MD5,request-URI,timestamp\n    timestamp_header: Date\n    timestamp_format: RFC 1123\n    timestamp_skew_minutes: 15\n    content_md5: base64 MD5 of request body (PUT/POST only; empty for GET)\n    notes: >-\n      Query strings are part of the request URI but are\
  \ not factored into the\n      Content-MD5. Signature = Base64.strict_encode64(HMAC-SHA1(secret_key,\n      canonical_string)).\n- id: event_attendee_token\n  api: Attendease Event API\n  type: apiKey\n  in: header\n  name: X-Attendee-Token\n  alt_in: query\n  alt_name: attendee_token\n  description: Per-attendee access token scoped to a single event.\n- id: event_token\n  api: Attendease Event API\n  type: apiKey\n  in: header\n  name: X-Event-Token\n  description: Event-level access token scoped to a single event subdomain.\n- id: event_basic\n  api: Attendease Event API\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with email/password (also accepted as query params).\ncredentials:\n  org_api: >-\n    Access Key ID + Secret Access Token issued at the organization level.\n  event_api: >-\n    Attendee tokens managed per event at\n    https://attendease.com/events/<event-subdomain>/access_tokens\ntransport: HTTPS required for all requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attendease/refs/heads/main/authentication/attendease-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Events
- Event Management
- Event Marketing
- Conferences
- Webinars
- Attendees
- Registration
- SaaS
---
