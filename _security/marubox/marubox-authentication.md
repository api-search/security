---
anonymous_access: false
api_key_in: []
api_specs:
- filename: marubox-account-api-openapi.yml
  format: yaml
  label: Business Box Account API
  slug: marubox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-account-api-openapi.yml
- filename: marubox-bookings-api-openapi.yml
  format: yaml
  label: Business Box Bookings API
  slug: marubox-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-bookings-api-openapi.yml
- filename: marubox-event-types-api-openapi.yml
  format: yaml
  label: Business Box Event types API
  slug: marubox-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-event-types-api-openapi.yml
- filename: marubox-invites-api-openapi.yml
  format: yaml
  label: Business Box Invites API
  slug: marubox-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-invites-api-openapi.yml
- filename: marubox-webhooks-api-openapi.yml
  format: yaml
  label: Business Box Webhooks API
  slug: marubox-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for Business Box API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Marubox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Business Box declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Business Box
provider_slug: marubox
scheme_count: 1
schemes:
- evidence: One personal API key per thing you connect, sent as a bearer token.
  header: Authorization
  how_to_obtain: 'Create a key under Settings → API keys and webhooks in the app, then copy the displayed key (shown once) and use it as Authorization: Bearer <key>.'
  location: header
  name: API key
  scopes:
  - event_types:read
  - bookings:read
  - bookings:write
  - webhooks:manage
  type: http-bearer
slug: marubox-authentication
source_filename: marubox-authentication.yml
source_heading: Authentication Profile
source_url: https://marubox.jp/developers/authentication/
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://marubox.jp/developers/authentication/\nsources:\n- https://marubox.jp/developers/authentication/\n- https://marubox.jp/guide/getting-started\n- https://marubox.jp/developers/quickstart/\ndescription: Authentication methods for Business Box API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: One personal API key per thing you connect, sent as a bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - event_types:read\n  - bookings:read\n  - bookings:write\n  - webhooks:manage\n  how_to_obtain: 'Create a key under Settings → API keys and webhooks in the app, then copy the displayed key (shown once) and use it as Authorization:\n    Bearer <key>.'\nnote: OAuth 2.1 with PKCE is announced for future use but not yet live; therefore no OAuth flows are currently available.\ndocs: https://marubox.jp/developers/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/authentication/marubox-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Booking
- Payments
- Calendar
- Japan
---
