---
api_key_in:
- query
api_specs:
- filename: race-entry-event-api-openapi.yml
  format: yaml
  label: Race Entry Event API
  slug: race-entry-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-event-api-openapi.yml
- filename: race-entry-get-category-teams-api-openapi.yml
  format: yaml
  label: Race Entry Get Category Teams API
  slug: race-entry-get-category-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-category-teams-api-openapi.yml
- filename: race-entry-get-event-categories-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Categories API
  slug: race-entry-get-event-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-categories-api-openapi.yml
- filename: race-entry-get-event-participants-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Participants API
  slug: race-entry-get-event-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-participants-api-openapi.yml
- filename: race-entry-get-event-pin-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Pin API
  slug: race-entry-get-event-pin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-pin-api-openapi.yml
- filename: race-entry-get-event-questions-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Questions API
  slug: race-entry-get-event-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-questions-api-openapi.yml
- filename: race-entry-get-event-teams-api-openapi.yml
  format: yaml
  label: Race Entry Get Event Teams API
  slug: race-entry-get-event-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-event-teams-api-openapi.yml
- filename: race-entry-get-events-api-openapi.yml
  format: yaml
  label: Race Entry Get Events API
  slug: race-entry-get-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-get-events-api-openapi.yml
- filename: race-entry-login-api-openapi.yml
  format: yaml
  label: Race Entry Login API
  slug: race-entry-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-login-api-openapi.yml
- filename: race-entry-memberships-api-openapi.yml
  format: yaml
  label: Race Entry Memberships API
  slug: race-entry-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-memberships-api-openapi.yml
- filename: race-entry-result-api-openapi.yml
  format: yaml
  label: Race Entry Result API
  slug: race-entry-result-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-result-api-openapi.yml
- filename: race-entry-set-event-app-access-api-openapi.yml
  format: yaml
  label: Race Entry Set Event App Access API
  slug: race-entry-set-event-app-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-set-event-app-access-api-openapi.yml
- filename: race-entry-set-event-pin-api-openapi.yml
  format: yaml
  label: Race Entry Set Event Pin API
  slug: race-entry-set-event-pin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-set-event-pin-api-openapi.yml
- filename: race-entry-update-event-participant-api-openapi.yml
  format: yaml
  label: Race Entry Update Event Participant API
  slug: race-entry-update-event-participant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-update-event-participant-api-openapi.yml
- filename: race-entry-upload-api-openapi.yml
  format: yaml
  label: Race Entry Upload API
  slug: race-entry-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-upload-api-openapi.yml
- filename: race-entry-user-api-openapi.yml
  format: yaml
  label: Race Entry User API
  slug: race-entry-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Race Entry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Race Entry secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Race Entry
provider_slug: race-entry
scheme_count: 1
schemes:
- description: Temporary key returned from /login. Must be supplied alongside tmp_secret query parameter. Credentials expire after 48 hours.
  in: query
  name: TempCredentials
  parameter: tmp_key
  sources:
  - openapi/race-entry-openapi.yml
  type: apiKey
slug: race-entry-authentication
source_filename: race-entry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/race-entry-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: TempCredentials\n  type: apiKey\n  in: query\n  parameter: tmp_key\n  description: Temporary key returned from /login. Must be supplied alongside tmp_secret query\n    parameter. Credentials expire after 48 hours.\n  sources:\n  - openapi/race-entry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/authentication/race-entry-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Race Timing
- Race Registration
- Event Management
- Race Results
- Sports
---
