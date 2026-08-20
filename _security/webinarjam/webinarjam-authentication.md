---
api_key_in:
- body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Webinarjam Authentication
name_suffix: Authentication
oauth_flows: []
overview: WebinarJam secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WebinarJam
provider_slug: webinarjam
scheme_count: 1
schemes:
- description: A single account-wide 64-character API key, transmitted as a form field named "api_key" in the body of every POST request. The key is identical for WebinarJam and EverWebinar and does not change per webinar.
  format: string(64)
  in: body
  name: api_key
  parameter: api_key
  sources:
  - https://support.webinarjam.com/en/articles/15370144-connect-to-webinarjam-or-everwebinar-api
  - https://support.webinarjam.com/en/articles/15370149-retrieve-a-full-list-of-all-webinars-published-in-your-account-webinarjam-api
  type: apiKey
slug: webinarjam-authentication
source_filename: webinarjam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://support.webinarjam.com/en/articles/15370144-connect-to-webinarjam-or-everwebinar-api\ndocs: https://support.webinarjam.com/en/collections/19655440-api-general\nnote: >-\n  Derived by hand from the provider's own help-center reference, not from an OpenAPI —\n  WebinarJam publishes no machine-readable specification. Every field below is stated in\n  the WebinarJam / EverWebinar developer articles.\nsummary:\n  types: [apiKey]\n  api_key_in: [body]\n  oauth2_flows: []\n  approval_required: true\n  transport_security: TLS required\nschemes:\n  - name: api_key\n    type: apiKey\n    in: body\n    parameter: api_key\n    format: string(64)\n    description: >-\n      A single account-wide 64-character API key, transmitted as a form field named\n      \"api_key\" in the body of every POST request. The key is identical for WebinarJam\n      and EverWebinar and does not change per webinar.\n    sources:\n      - https://support.webinarjam.com/en/articles/15370144-connect-to-webinarjam-or-everwebinar-api\n\
  \      - https://support.webinarjam.com/en/articles/15370149-retrieve-a-full-list-of-all-webinars-published-in-your-account-webinarjam-api\nonboarding:\n  model: request-approval\n  steps:\n    - Hold a paid WebinarJam or EverWebinar subscription; trial accounts must upgrade first.\n    - Open Profile > API in the account dashboard and complete the API application form\n      (app URL, intended use, whether the app subscribes users, supporting notes).\n    - Wait for review — the provider states requests are typically processed within two\n      business days.\n    - Retrieve the issued key from the Webinars dashboard under Advanced > API custom integration.\n  docs:\n    apply: https://support.webinarjam.com/en/articles/15370143-apply-for-an-api-key-for-webinarjam-or-everwebinar\n    locate: https://support.webinarjam.com/en/articles/15370144-connect-to-webinarjam-or-everwebinar-api\n    regenerate: https://support.webinarjam.com/en/articles/15370145-regenerate-a-webinarjam-everwebinar-api-key\n\
  \  scope: >-\n    One set of API credentials is generated per account and grants access to BOTH the\n    WebinarJam and the EverWebinar API.\nkey_management:\n  rotation: >-\n    The key can be regenerated from the account profile; the provider documents regeneration\n    as an explicit self-service action.\n  granularity: account-wide (no per-webinar, per-user or per-environment keys)\n  scopes: none — the key is unscoped; there is no OAuth, no permission model and no\n    read-only variant, so any approved integration holds full account authority.\ntransport:\n  tls_required: true\n  note: >-\n    \"Connections to the API server must be secured with SSL. Non-SSL connections will be\n    dropped.\" — https://support.webinarjam.com/en/articles/15370144-connect-to-webinarjam-or-everwebinar-api\ngaps:\n  - No OAuth 2.0, OpenID Connect or token-exchange surface is published.\n  - The credential travels in the request BODY rather than an Authorization header, so it\n    lands in application\
  \ logs and proxy request bodies more readily than a header credential.\n  - No scopes, so a delegated or agent integration cannot be granted less than full account access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webinarjam/refs/heads/main/authentication/webinarjam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Webinars
- Marketing
- Live Events
- Automated Webinars
- Evergreen Webinars
- Lead Generation
- Registration
- Video Streaming
- Marketing Automation
- Software-as-a-Service
---
