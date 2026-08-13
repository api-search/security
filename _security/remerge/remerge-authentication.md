---
api_key_in: []
auth_types:
- http
- apiKey
description: Remerge runs two separately-authenticated HTTP surfaces. The Reporting API uses a session-style token minted by a sign-in request with dashboard credentials and presented in a custom Authorization header. The Event Tracking API is authorized with a partner name plus a Remerge-issued key carried as query parameters on every GET.
kind: authentication
layout: security
method: searched
name: Remerge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Remerge secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Remerge
provider_slug: remerge
scheme_count: 2
schemes:
- api: remerge-reporting-api
  description: Custom token scheme on the Reporting API. The header carries two quoted parameters — the user_token returned by the sign-in call and the account email that token belongs to.
  failure_message: Unauthorized — the provided Authorization token was invalid
  failure_status: 401
  format: Token user_token="<user_token>", email="<account email>"
  header: Authorization
  in: header
  name: reportingToken
  required_companion_headers:
  - Content-Type: application/json
  - Accept: application/json
  scheme: custom-token
  source: https://help.remerge.io/hc/en-us/articles/115003440434-Remerge-Reporting-API
  token_acquisition:
    endpoint: https://api.remerge.io/users/sign_in
    method: POST
    note: The response returns both `token` and `user_token`; the documented Authorization header uses `user_token`. Credentials are the same dashboard login used at admin.remerge.io and are issued by an Account Manager.
    request_body_shape: '{"user": {"email": "<email>", "password": "<password>"}}'
    request_headers:
      Accept: application/json
      Content-Type: application/json
    response_fields:
    - email
    - token
    - user_id
    - user_name
    - user_token
  type: http
- api: remerge-event-tracking-api
  description: The Event Tracking API authorizes each GET with a `partner` value (the tracking partner / client name) and a `key` value issued by Remerge. Both are mandatory on every documented payload family (in-app event, attribution, BI, SKAdNetwork).
  example_shape: https://remerge.events/event?app_id=<app_id>&event=<event>&partner=<yourname>&key=<yourkey>&...
  in: query
  issuance: Partner key is provided by Remerge (per the docs, "Partner's key (provided by Remerge)").
  name: partnerKey
  parameter_names:
  - partner
  - key
  source: https://help.remerge.io/hc/en-us/articles/6078711583260-Event-Data-Forwarding
  transport_warning: The key travels in the query string of a GET request, so it is exposed to proxy logs, referrer headers and server access logs. This is inherent to the documented design, not a misconfiguration observed in this probe.
  type: apiKey
slug: remerge-authentication
source_filename: remerge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://help.remerge.io/hc/en-us/articles/115003440434-Remerge-Reporting-API\n  (Reporting API authorization section) and\n  https://help.remerge.io/hc/en-us/articles/6078711583260-Event-Data-Forwarding\n  (Event Tracking API partner/key parameters). Remerge publishes no OpenAPI, so\n  this profile was read from the provider's own Help Center documentation rather\n  than derived from securitySchemes.\ndocs: https://help.remerge.io/hc/en-us/articles/115003440434-Remerge-Reporting-API\ndescription: >-\n  Remerge runs two separately-authenticated HTTP surfaces. The Reporting API\n  uses a session-style token minted by a sign-in request with dashboard\n  credentials and presented in a custom Authorization header. The Event Tracking\n  API is authorized with a partner name plus a Remerge-issued key carried as\n  query parameters on every GET.\n\nsummary:\n  types:\n  - http\n  - apiKey\n  oauth2: false\n  openid_connect: false\n\
  \  mutual_tls: false\n  self_service_credentials: false\n  credential_issuance: >-\n    Account-managed. Dashboard logins for the Reporting API and partner keys for\n    the Event Tracking API are issued by a Remerge Account Manager; there is no\n    public self-service key generation.\n\nschemes:\n- name: reportingToken\n  api: remerge-reporting-api\n  type: http\n  scheme: custom-token\n  in: header\n  header: Authorization\n  format: 'Token user_token=\"<user_token>\", email=\"<account email>\"'\n  description: >-\n    Custom token scheme on the Reporting API. The header carries two quoted\n    parameters — the user_token returned by the sign-in call and the account\n    email that token belongs to.\n  token_acquisition:\n    endpoint: https://api.remerge.io/users/sign_in\n    method: POST\n    request_headers:\n      Content-Type: application/json\n      Accept: application/json\n    request_body_shape: '{\"user\": {\"email\": \"<email>\", \"password\": \"<password>\"}}'\n    response_fields:\n\
  \    - email\n    - token\n    - user_id\n    - user_name\n    - user_token\n    note: >-\n      The response returns both `token` and `user_token`; the documented\n      Authorization header uses `user_token`. Credentials are the same dashboard\n      login used at admin.remerge.io and are issued by an Account Manager.\n  required_companion_headers:\n  - Content-Type: application/json\n  - Accept: application/json\n  failure_status: 401\n  failure_message: Unauthorized — the provided Authorization token was invalid\n  source: https://help.remerge.io/hc/en-us/articles/115003440434-Remerge-Reporting-API\n\n- name: partnerKey\n  api: remerge-event-tracking-api\n  type: apiKey\n  in: query\n  parameter_names:\n  - partner\n  - key\n  description: >-\n    The Event Tracking API authorizes each GET with a `partner` value (the\n    tracking partner / client name) and a `key` value issued by Remerge. Both\n    are mandatory on every documented payload family (in-app event, attribution,\n    BI,\
  \ SKAdNetwork).\n  example_shape: >-\n    https://remerge.events/event?app_id=<app_id>&event=<event>&partner=<yourname>&key=<yourkey>&...\n  issuance: Partner key is provided by Remerge (per the docs, \"Partner's key (provided by Remerge)\").\n  transport_warning: >-\n    The key travels in the query string of a GET request, so it is exposed to\n    proxy logs, referrer headers and server access logs. This is inherent to the\n    documented design, not a misconfiguration observed in this probe.\n  source: https://help.remerge.io/hc/en-us/articles/6078711583260-Event-Data-Forwarding\n\nobservations:\n- id: swagger-gated\n  detail: >-\n    https://api.remerge.io/swagger.json and https://api.remerge.io/docs both\n    exist as routes but answer HTTP 302 to https://admin.remerge.io — the API\n    describes itself behind the operator login. Every other spec path on that\n    host (/openapi.json, /api-docs, /redoc, /v1/openapi.json) answers 404, so no\n    public machine-readable contract could\
  \ be captured.\n  probed: '2026-08-12'\n  evidence:\n  - url: https://api.remerge.io/swagger.json\n    status: 302\n  - url: https://api.remerge.io/openapi.json\n    status: 404\n- id: no-oauth\n  detail: >-\n    No OAuth 2.0 or OpenID Connect surface. /.well-known/oauth-authorization-server\n    and /.well-known/openid-configuration return 404 on www.remerge.io,\n    api.remerge.io and remerge.events.\n  probed: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remerge/refs/heads/main/authentication/remerge-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Advertising
- AdTech
- Mobile
- Retargeting
- Demand-Side Platform
- User Acquisition
- Marketing
---
