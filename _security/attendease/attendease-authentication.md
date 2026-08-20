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
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.attendease.com/, https://eventupplanner.zendesk.com/hc/en-us/articles/27101295757207-Event-and-Organization-API-Keys, https://eventupplanner.zendesk.com/hc/en-us/articles/27101962543383-How-do-I-add-or-remove-access-tokens\ndocs: https://developer.attendease.com/\nsummary: >-\n  Attendease exposes two authentication models. The Organization API (/api/v2/)\n  uses HMAC-SHA1 request signing with an Access Key ID and Secret Access Token.\n  The Event API uses per-event attendee/event tokens (query params or headers)\n  and also accepts HTTP Basic auth. All requests must use HTTPS.\nschemes:\n- id: org_api_hmac\n  api: Attendease Organization API\n  type: http\n  scheme: hmac-sha1\n  header: Authorization\n  format: 'APIAuth <access_key>:<signature>'\n  signing:\n    algorithm: HMAC-SHA1\n    encoding: base64\n    canonical_string: content-type,content-MD5,request-URI,timestamp\n    timestamp_header: Date\n  \
  \  timestamp_format: RFC 1123\n    timestamp_skew_minutes: 15\n    content_md5: base64 MD5 of request body (PUT/POST only; empty for GET)\n    notes: >-\n      Query strings are part of the request URI but are not factored into the\n      Content-MD5. Signature = Base64.strict_encode64(HMAC-SHA1(secret_key,\n      canonical_string)).\n- id: event_attendee_token\n  api: Attendease Event API\n  type: apiKey\n  in: header\n  name: X-Attendee-Token\n  alt_in: query\n  alt_name: attendee_token\n  description: Per-attendee access token scoped to a single event.\n- id: event_token\n  api: Attendease Event API\n  type: apiKey\n  in: header\n  name: X-Event-Token\n  description: Event-level access token scoped to a single event subdomain.\n- id: event_basic\n  api: Attendease Event API\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with email/password (also accepted as query params).\ncredentials:\n  org_api: >-\n    Access Key ID + Secret Access Token issued at the organization\
  \ level.\n  event_api: >-\n    Attendee tokens managed per event at\n    https://attendease.com/events/<event-subdomain>/access_tokens\ncredential_management:\n  event_api:\n    self_serve: true\n    console_path: Event -> Integrate -> Access Tokens\n    default_token: >-\n      A token named \"default\" is created automatically for every event. It is a\n      randomly generated UUID (128-bit value).\n    multiple_tokens: true\n    naming: Each token carries its own name for reference.\n    rotation: Self-serve — add a new token, remove the old one.\n    revocation: Deleting a token immediately prevents authenticating with it.\n    private_events: >-\n      If an event is marked \"private\", ALL API calls require an access token.\n      Marking an event private requires contacting support.\n    source: https://eventupplanner.zendesk.com/hc/en-us/articles/27101962543383-How-do-I-add-or-remove-access-tokens\n  org_api:\n    self_serve: false\n    rotation: >-\n      Organization API credentials\
  \ cannot be created, deleted or regenerated from\n      the dashboard. Every change requires contacting support.\n    entitlement: >-\n      The Organization API is offered to ENTERPRISE customers only (\"For\n      Enterprise customers, we also offer an Organization API to access all events\n      and attendees at the organization level\"). See\n      plans/attendease-plans-pricing.yml.\n    source: https://eventupplanner.zendesk.com/hc/en-us/articles/27101295757207-Event-and-Organization-API-Keys\n  guidance_published:\n    never_share_keys: true\n    delete_unused_keys: true\n    periodic_rotation: true\n    note: >-\n      The help center publishes explicit API-key hygiene guidance: keys act as\n      passwords, delete them when no longer needed, and regenerate them\n      periodically when access must be maintained over long periods.\nsso:\n  available: true\n  scope: Attendee and dashboard SSO\n  plans:\n  - Enterprise\n  protocol_published: false\n  note: >-\n    SSO is listed as\
  \ an Enterprise entitlement on the plans page but no protocol\n    (SAML/OIDC) or metadata endpoint is documented publicly. The GitHub org\n    carries a fork of saml_idp, which suggests SAML, but that is not a provider\n    statement and is not recorded as fact.\n  source: https://eventupplanner.com/plans-and-pricing/\nmfa:\n  available: true\n  scope: dashboard users (not API)\n  source: https://eventupplanner.zendesk.com/hc/en-us/articles/27102025968919-How-do-I-set-up-two-factor-authentication\ntransport: HTTPS required for all requests. Calls made over plain HTTP will fail.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attendease/refs/heads/main/authentication/attendease-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Event
- Event Management
- Event Marketing
- Conferences
- Webinars
- Attendees
- Registration
- Software-as-a-Service
---
