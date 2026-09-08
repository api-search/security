---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cvent-registration-attendees-api-openapi.yml
  format: yaml
  label: Cvent Registration Attendees API
  slug: cvent-registration-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-attendees-api-openapi.yml
- filename: cvent-registration-contacts-api-openapi.yml
  format: yaml
  label: Cvent Registration Contacts API
  slug: cvent-registration-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-contacts-api-openapi.yml
- filename: cvent-registration-events-api-openapi.yml
  format: yaml
  label: Cvent Registration Events API
  slug: cvent-registration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-events-api-openapi.yml
- filename: cvent-registration-exhibitors-api-openapi.yml
  format: yaml
  label: Cvent Registration Exhibitors API
  slug: cvent-registration-exhibitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-exhibitors-api-openapi.yml
- filename: cvent-registration-oauth-api-openapi.yml
  format: yaml
  label: Cvent Registration OAuth API
  slug: cvent-registration-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-oauth-api-openapi.yml
- filename: cvent-registration-sessions-api-openapi.yml
  format: yaml
  label: Cvent Registration Sessions API
  slug: cvent-registration-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-sessions-api-openapi.yml
- filename: cvent-registration-webhooks-api-openapi.yml
  format: yaml
  label: Cvent Registration Webhooks API
  slug: cvent-registration-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-webhooks-api-openapi.yml
- filename: cvent-registration-orders-api-openapi.yml
  format: yaml
  label: Cvent Registration Orders and Transactions API
  slug: cvent-registration-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-orders-api-openapi.yml
- filename: cvent-registration-surveys-api-openapi.yml
  format: yaml
  label: Cvent Registration Surveys API
  slug: cvent-registration-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-surveys-api-openapi.yml
- filename: cvent-registration-speakers-api-openapi.yml
  format: yaml
  label: Cvent Registration Speakers API
  slug: cvent-registration-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-speakers-api-openapi.yml
- filename: cvent-registration-seating-api-openapi.yml
  format: yaml
  label: Cvent Registration Seating and Badging API
  slug: cvent-registration-seating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-seating-api-openapi.yml
- filename: cvent-registration-discounts-api-openapi.yml
  format: yaml
  label: Cvent Registration Discounts API
  slug: cvent-registration-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-discounts-api-openapi.yml
- filename: cvent-registration-custom-fields-api-openapi.yml
  format: yaml
  label: Cvent Registration Custom Fields API
  slug: cvent-registration-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-custom-fields-api-openapi.yml
- filename: cvent-registration-event-travel-api-openapi.yml
  format: yaml
  label: Cvent Registration Event Travel API
  slug: cvent-registration-event-travel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-event-travel-api-openapi.yml
- filename: cvent-registration-attendee-activities-api-openapi.yml
  format: yaml
  label: Cvent Registration Attendee Activities API
  slug: cvent-registration-attendee-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-attendee-activities-api-openapi.yml
- filename: cvent-registration-scim-api-openapi.yml
  format: yaml
  label: Cvent Registration SCIM User Provisioning API
  slug: cvent-registration-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-scim-api-openapi.yml
- filename: cvent-registration-usage-api-openapi.yml
  format: yaml
  label: Cvent Registration Usage and Quota API
  slug: cvent-registration-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/openapi/cvent-registration-usage-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Cvent Registration Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Cvent Registration secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Cvent Registration
provider_slug: cvent-registration
scheme_count: 4
schemes:
- description: OAuth2 Authorization Code Flow.
  flows:
  - authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize
    flow: authorizationCode
    scopes: 208
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.authorizationCode
  sources:
  - openapi/cvent-registration-attendee-activities-api-openapi.yml
  - openapi/cvent-registration-attendees-api-openapi.yml
  - openapi/cvent-registration-contacts-api-openapi.yml
  - openapi/cvent-registration-custom-fields-api-openapi.yml
  - openapi/cvent-registration-discounts-api-openapi.yml
  - openapi/cvent-registration-event-travel-api-openapi.yml
  - openapi/cvent-registration-events-api-openapi.yml
  - openapi/cvent-registration-exhibitors-api-openapi.yml
  - openapi/cvent-registration-oauth-api-openapi.yml
  - openapi/cvent-registration-orders-api-openapi.yml
  - openapi/cvent-registration-scim-api-openapi.yml
  - openapi/cvent-registration-seating-api-openapi.yml
  - openapi/cvent-registration-sessions-api-openapi.yml
  - openapi/cvent-registration-speakers-api-openapi.yml
  - openapi/cvent-registration-surveys-api-openapi.yml
  - openapi/cvent-registration-usage-api-openapi.yml
  - openapi/cvent-registration-webhooks-api-openapi.yml
  type: oauth2
- description: OAuth2 Client Credentials Flow.
  flows:
  - flow: clientCredentials
    scopes: 238
    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token
  name: OAuth2.clientCredentials
  sources:
  - openapi/cvent-registration-attendee-activities-api-openapi.yml
  - openapi/cvent-registration-attendees-api-openapi.yml
  - openapi/cvent-registration-contacts-api-openapi.yml
  - openapi/cvent-registration-custom-fields-api-openapi.yml
  - openapi/cvent-registration-discounts-api-openapi.yml
  - openapi/cvent-registration-event-travel-api-openapi.yml
  - openapi/cvent-registration-events-api-openapi.yml
  - openapi/cvent-registration-exhibitors-api-openapi.yml
  - openapi/cvent-registration-oauth-api-openapi.yml
  - openapi/cvent-registration-orders-api-openapi.yml
  - openapi/cvent-registration-scim-api-openapi.yml
  - openapi/cvent-registration-seating-api-openapi.yml
  - openapi/cvent-registration-sessions-api-openapi.yml
  - openapi/cvent-registration-speakers-api-openapi.yml
  - openapi/cvent-registration-surveys-api-openapi.yml
  - openapi/cvent-registration-usage-api-openapi.yml
  - openapi/cvent-registration-webhooks-api-openapi.yml
  type: oauth2
- description: This security scheme is used to indicate that Cvent should use API Key auth when invoking your callback. This scheme is only supported for callback operations, and cannot be used to make calls to Cvent endpoints.
  in: header
  name: CallbackApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/cvent-registration-webhooks-api-openapi.yml
  type: apiKey
- description: This security scheme is used to indicate that Cvent should use basic auth when invoking your callback. This scheme is only supported for callback operations, and cannot be used to make calls to Cvent endpoints.
  name: CallbackBasicAuth
  scheme: basic
  sources:
  - openapi/cvent-registration-webhooks-api-openapi.yml
  type: http
slug: cvent-registration-authentication
source_filename: cvent-registration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: derived\nsource: openapi/cvent-registration-attendee-activities-api-openapi.yml, openapi/cvent-registration-attendees-api-openapi.yml,\n  openapi/cvent-registration-contacts-api-openapi.yml, openapi/cvent-registration-custom-fields-api-openapi.yml,\n  openapi/cvent-registration-discounts-api-openapi.yml, openapi/cvent-registration-event-travel-api-openapi.yml,\n  openapi/cvent-registration-events-api-openapi.yml, openapi/cvent-registration-exhibitors-api-openapi.yml,\n  openapi/cvent-registration-oauth-api-openapi.yml, openapi/cvent-registration-orders-api-openapi.yml,\n  openapi/cvent-registration-scim-api-openapi.yml, openapi/cvent-registration-seating-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2.authorizationCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-platform.cvent.com/ea/oauth2/authorize\n\
  \    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 208\n  description: OAuth2 Authorization Code Flow.\n  sources:\n  - openapi/cvent-registration-attendee-activities-api-openapi.yml\n  - openapi/cvent-registration-attendees-api-openapi.yml\n  - openapi/cvent-registration-contacts-api-openapi.yml\n  - openapi/cvent-registration-custom-fields-api-openapi.yml\n  - openapi/cvent-registration-discounts-api-openapi.yml\n  - openapi/cvent-registration-event-travel-api-openapi.yml\n  - openapi/cvent-registration-events-api-openapi.yml\n  - openapi/cvent-registration-exhibitors-api-openapi.yml\n  - openapi/cvent-registration-oauth-api-openapi.yml\n  - openapi/cvent-registration-orders-api-openapi.yml\n  - openapi/cvent-registration-scim-api-openapi.yml\n  - openapi/cvent-registration-seating-api-openapi.yml\n  - openapi/cvent-registration-sessions-api-openapi.yml\n  - openapi/cvent-registration-speakers-api-openapi.yml\n  - openapi/cvent-registration-surveys-api-openapi.yml\n\
  \  - openapi/cvent-registration-usage-api-openapi.yml\n  - openapi/cvent-registration-webhooks-api-openapi.yml\n- name: OAuth2.clientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-platform.cvent.com/ea/oauth2/token\n    scopes: 238\n  description: OAuth2 Client Credentials Flow.\n  sources:\n  - openapi/cvent-registration-attendee-activities-api-openapi.yml\n  - openapi/cvent-registration-attendees-api-openapi.yml\n  - openapi/cvent-registration-contacts-api-openapi.yml\n  - openapi/cvent-registration-custom-fields-api-openapi.yml\n  - openapi/cvent-registration-discounts-api-openapi.yml\n  - openapi/cvent-registration-event-travel-api-openapi.yml\n  - openapi/cvent-registration-events-api-openapi.yml\n  - openapi/cvent-registration-exhibitors-api-openapi.yml\n  - openapi/cvent-registration-oauth-api-openapi.yml\n  - openapi/cvent-registration-orders-api-openapi.yml\n  - openapi/cvent-registration-scim-api-openapi.yml\n  - openapi/cvent-registration-seating-api-openapi.yml\n\
  \  - openapi/cvent-registration-sessions-api-openapi.yml\n  - openapi/cvent-registration-speakers-api-openapi.yml\n  - openapi/cvent-registration-surveys-api-openapi.yml\n  - openapi/cvent-registration-usage-api-openapi.yml\n  - openapi/cvent-registration-webhooks-api-openapi.yml\n- name: CallbackApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: This security scheme is used to indicate that Cvent should use API Key auth when\n    invoking your callback. This scheme is only supported for callback operations, and cannot\n    be used to make calls to Cvent endpoints.\n  sources:\n  - openapi/cvent-registration-webhooks-api-openapi.yml\n- name: CallbackBasicAuth\n  type: http\n  scheme: basic\n  description: This security scheme is used to indicate that Cvent should use basic auth when\n    invoking your callback. This scheme is only supported for callback operations, and cannot\n    be used to make calls to Cvent endpoints.\n  sources:\n  - openapi/cvent-registration-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cvent-registration/refs/heads/main/authentication/cvent-registration-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Attendee Management
- Attendees
- Conferences
- Event Management
- Event
- Authentication
- On-Site Check-In
- Payments
- Registration
- REST API
- SCIM
- SDKs
- SOAP
- Ticketing
- Webhook
---
