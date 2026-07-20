---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fourth Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Fourth secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Fourth
provider_slug: fourth
scheme_count: 2
schemes:
- applies_to:
  - Tasks API
  - Notifications API
  - and other OAuth-enabled Fourth APIs
  bearer_format: 'Authorization: Bearer [access_token]'
  flows:
  - flow: clientCredentials
    notes: Expected approach for almost all use cases; client_id + client_secret issued by Fourth.
    tokenUrl: '[ROOT]/oauth/connect/token'
  - flow: password
    notes: For credentials of a Fourth end user rather than an application.
    tokenUrl: '[ROOT]/oauth/connect/token'
  name: OAuth2
  scope_note: Scopes are per-API and listed on each API reference page under the Authentication heading (e.g. NotificationService for the Notifications API).
  token_lifetime: expires_in seconds (e.g. 3600 = 1 hour); refresh_token may be returned.
  type: oauth2
- name: BasicAuth
  notes: base64(username:password) in the Authorization header; accepted for APIs that otherwise require OAuth when testing in Swagger UI, and used by several Adaco/legacy APIs.
  scheme: basic
  type: http
slug: fourth-authentication
source_filename: fourth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.fourth.com/en-gb/docs/authenticating-oauth\ndocs: https://developer.fourth.com/en-gb/docs/authenticating-oauth\nsummary:\n  types: [oauth2, http]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [clientCredentials, password]\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: '[ROOT]/oauth/connect/token'\n    notes: Expected approach for almost all use cases; client_id + client_secret issued by Fourth.\n  - flow: password\n    tokenUrl: '[ROOT]/oauth/connect/token'\n    notes: For credentials of a Fourth end user rather than an application.\n  bearer_format: 'Authorization: Bearer [access_token]'\n  token_lifetime: expires_in seconds (e.g. 3600 = 1 hour); refresh_token may be returned.\n  scope_note: >-\n    Scopes are per-API and listed on each API reference page under the\n    Authentication heading (e.g. NotificationService for the Notifications API).\n  applies_to:\
  \ [Tasks API, Notifications API, and other OAuth-enabled Fourth APIs]\n- name: BasicAuth\n  type: http\n  scheme: basic\n  notes: >-\n    base64(username:password) in the Authorization header; accepted for APIs that\n    otherwise require OAuth when testing in Swagger UI, and used by several Adaco/legacy APIs.\nprovisioning:\n  notes: >-\n    Production and test host locations and credentials are not published; mutual\n    customers request credentials from Fourth (2-4 week provisioning). Adaco users\n    can self-generate credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourth/refs/heads/main/authentication/fourth-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Workforce Management
- Restaurants
- Hospitality
- Inventory Management
- Payroll
- Scheduling
- Human Capital Management
- Point of Sale
- Food and Beverage
---
