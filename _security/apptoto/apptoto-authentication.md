---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apptoto-address-books-api-openapi.yml
  format: yaml
  label: Apptoto Address Books API
  slug: apptoto-address-books-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-address-books-api-openapi.yml
- filename: apptoto-availability-api-openapi.yml
  format: yaml
  label: Apptoto Availability API
  slug: apptoto-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-availability-api-openapi.yml
- filename: apptoto-book-now-api-openapi.yml
  format: yaml
  label: Apptoto Book Now API
  slug: apptoto-book-now-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-book-now-api-openapi.yml
- filename: apptoto-booking-pages-api-openapi.yml
  format: yaml
  label: Apptoto Booking Pages API
  slug: apptoto-booking-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-booking-pages-api-openapi.yml
- filename: apptoto-bookings-api-openapi.yml
  format: yaml
  label: Apptoto Bookings API
  slug: apptoto-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-bookings-api-openapi.yml
- filename: apptoto-calendars-api-openapi.yml
  format: yaml
  label: Apptoto Calendars API
  slug: apptoto-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-calendars-api-openapi.yml
- filename: apptoto-contact-api-openapi.yml
  format: yaml
  label: Apptoto Contact API
  slug: apptoto-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-contact-api-openapi.yml
- filename: apptoto-contacts-api-openapi.yml
  format: yaml
  label: Apptoto Contacts API
  slug: apptoto-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-contacts-api-openapi.yml
- filename: apptoto-conversation-messages-api-openapi.yml
  format: yaml
  label: Apptoto Conversation Messages API
  slug: apptoto-conversation-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-conversation-messages-api-openapi.yml
- filename: apptoto-conversation-reply-api-openapi.yml
  format: yaml
  label: Apptoto Conversation Reply API
  slug: apptoto-conversation-reply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-conversation-reply-api-openapi.yml
- filename: apptoto-conversation-templates-api-openapi.yml
  format: yaml
  label: Apptoto Conversation Templates API
  slug: apptoto-conversation-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-conversation-templates-api-openapi.yml
- filename: apptoto-conversations-api-openapi.yml
  format: yaml
  label: Apptoto Conversations API
  slug: apptoto-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-conversations-api-openapi.yml
- filename: apptoto-event-api-openapi.yml
  format: yaml
  label: Apptoto Event API
  slug: apptoto-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-event-api-openapi.yml
- filename: apptoto-events-api-openapi.yml
  format: yaml
  label: Apptoto Events API
  slug: apptoto-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-events-api-openapi.yml
- filename: apptoto-import-api-openapi.yml
  format: yaml
  label: Apptoto Import API
  slug: apptoto-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-import-api-openapi.yml
- filename: apptoto-lists-api-openapi.yml
  format: yaml
  label: Apptoto Lists API
  slug: apptoto-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-lists-api-openapi.yml
- filename: apptoto-participant-api-openapi.yml
  format: yaml
  label: Apptoto Participant API
  slug: apptoto-participant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-participant-api-openapi.yml
- filename: apptoto-participants-api-openapi.yml
  format: yaml
  label: Apptoto Participants API
  slug: apptoto-participants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-participants-api-openapi.yml
- filename: apptoto-start-conversation-api-openapi.yml
  format: yaml
  label: Apptoto Start Conversation API
  slug: apptoto-start-conversation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-start-conversation-api-openapi.yml
- filename: apptoto-webhooks-api-openapi.yml
  format: yaml
  label: Apptoto Webhooks API
  slug: apptoto-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-webhooks-api-openapi.yml
- filename: apptoto-user-info-api-openapi.yml
  format: yaml
  label: Apptoto User Info API
  slug: apptoto-user-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apptoto/openapi/apptoto-user-info-api-openapi.yml
auth_types: []
description: Authentication methods for Apptoto API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Apptoto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apptoto declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Apptoto
provider_slug: apptoto
scheme_count: 2
schemes:
- evidence: Apptoto's APIs currently only support HTTP Basic Authentication.
  header: Authorization
  how_to_obtain: Find your API Key in the Apptoto web portal under Settings > Integrations > API.
  location: header
  name: Basic Authentication
  type: http-basic
- authorize_url: https://www.apptoto.com/oauth/authorize
  evidence: OAuth on Apptoto uses the standard `authorization_code` flow.
  how_to_obtain: Register an OAuth Application in the Apptoto portal under Settings > Integrations > OAuth Applications to receive a Client ID and Client Secret.
  name: OAuth 2.0 Authentication
  scopes:
  - calendars:read
  - address_books:read
  - contacts:read
  - events:read
  - bookings:read
  - imports:read
  - lists:read
  - messaging:read
  - webhooks:read
  - contacts:write
  - events:write
  - bookings:write
  - imports:write
  - lists:write
  - messaging:send
  - webhooks:write
  token_url: https://api.apptoto.com/oauth/token
  type: oauth2
slug: apptoto-authentication
source_filename: apptoto-authentication.yml
source_heading: Authentication Profile
source_url: https://apidocs.apptoto.com/reference/basic-authentication.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apidocs.apptoto.com/reference/basic-authentication.md\nsources:\n- https://apidocs.apptoto.com/reference/basic-authentication.md\n- https://apidocs.apptoto.com/reference/oauth-authentication.md\n- https://apidocs.apptoto.com/reference/basic-authentication\n- https://apidocs.apptoto.com/reference/oauth-authentication\ndescription: Authentication methods for Apptoto API\nschemes:\n- type: http-basic\n  name: Basic Authentication\n  evidence: Apptoto's APIs currently only support HTTP Basic Authentication.\n  location: header\n  header: Authorization\n  how_to_obtain: Find your API Key in the Apptoto web portal under Settings > Integrations > API.\n- type: oauth2\n  name: OAuth 2.0 Authentication\n  evidence: OAuth on Apptoto uses the standard `authorization_code` flow.\n  token_url: https://api.apptoto.com/oauth/token\n  authorize_url: https://www.apptoto.com/oauth/authorize\n\
  \  scopes:\n  - calendars:read\n  - address_books:read\n  - contacts:read\n  - events:read\n  - bookings:read\n  - imports:read\n  - lists:read\n  - messaging:read\n  - webhooks:read\n  - contacts:write\n  - events:write\n  - bookings:write\n  - imports:write\n  - lists:write\n  - messaging:send\n  - webhooks:write\n  how_to_obtain: Register an OAuth Application in the Apptoto portal under Settings > Integrations > OAuth Applications to receive a Client ID\n    and Client Secret.\ndocs: https://apidocs.apptoto.com/reference/basic-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/apptoto/authentication/apptoto-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Scheduling
- Appointment-Reminders
- SMS
- Email
- Voice
---
