---
api_key_in: []
api_specs:
- filename: knotch-events-api-openapi.yml
  format: yaml
  label: Knotch Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/openapi/knotch-events-api-openapi.yml
- filename: knotch-health-api-openapi.yml
  format: yaml
  label: Knotch Health API
  slug: knotch-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/openapi/knotch-health-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Knotch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knotch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knotch
provider_slug: knotch
scheme_count: 1
schemes:
- applies_to: Knotch Events API (https://events.knotch.it)
  header: 'Authorization: Bearer <api-key>'
  name: HTTPBearer
  rotation: contact Knotch Client Success Manager
  scheme: bearer
  sources:
  - openapi/knotch-events-api-openapi.yml
  - https://help.knotch.com/en/articles/159-events-api-v11-technical-overview
  transport: HTTPS required
  type: http
slug: knotch-authentication
source_filename: knotch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.knotch.com/en/articles/159-events-api-v11-technical-overview\ndocs: https://help.knotch.com/en/articles/159-events-api-v11-technical-overview\nnote: >-\n  Upgraded from the derived baseline (which read only the HTTPBearer securityScheme out of\n  https://events.knotch.it/openapi.json) with what Knotch's own Events API documentation states.\n  Knotch runs three distinct credential models across its surfaces and only one of them is an\n  API key.\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  self_service_credentials: false\n  credential_issuance: >-\n    Not self-service. The Events API documentation says \"To obtain or rotate an API key, contact\n    your Knotch Client Success Manager.\" The Event Pixel Account ID and the Verification Pixel\n    kvpid are likewise issued by Knotch staff.\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <api-key>'\n\
  \  transport: HTTPS required\n  applies_to: Knotch Events API (https://events.knotch.it)\n  rotation: contact Knotch Client Success Manager\n  sources:\n  - openapi/knotch-events-api-openapi.yml\n  - https://help.knotch.com/en/articles/159-events-api-v11-technical-overview\nnon_api_key_credentials:\n- name: Measurement Account ID\n  applies_to: Knotch Event Pixel (https://t.knotch.it/receive/beacon.gif)\n  carried_in: account_id query parameter\n  kind: account identifier, not a secret\n  issuance: Knotch Client Success team\n  source: https://docs.knotch.it/event_pixel/\n- name: kvpid\n  applies_to: Knotch Verification Pixel\n  carried_in: data-kvpid HTML5 data attribute on the script element\n  kind: per-publisher verification identifier\n  issuance: request via blueprint@knotch.com\n  source: https://docs.knotch.it/verification_pixel/\n- name: Unit ID\n  applies_to: Knotch Measurement Unit API\n  carried_in: knotch_<id> CSS class on the placeholder container\n  kind: unauthenticated\
  \ public identifier\n  source: https://docs.knotch.it/unit_api/\nwebhook_authentication:\n- name: Segment webhook Bearer + X-Signature HMAC\n  applies_to: POST /conversion_events/segment/{account_id}\n  detail: >-\n    Segment destinations send the same Authorization Bearer header, and additionally include an\n    X-Signature HMAC over the first event in each batch, which Knotch validates.\n  source: https://help.knotch.com/en/articles/159-events-api-v11-technical-overview\nplatform_authentication:\n- name: SSO\n  applies_to: Knotch One web platform (not the API)\n  detail: >-\n    Clients may enable Single Sign-On; Knotch does not receive the authorized user list and only\n    creates a user record after a first successful SSO login.\n  source: https://help.knotch.com/en/articles/49-how-does-sso-user-access-work-in-knotch-one\ngaps:\n- No OAuth 2.0 or OpenID Connect surface is published for the API.\n- No scope or permission model is documented; the Bearer token is account-wide.\n- No\
  \ documented key prefix, key format, expiry, or programmatic rotation endpoint.\n- The published OpenAPI declares HTTPBearer but supplies no bearerFormat and no description.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knotch/refs/heads/main/authentication/knotch-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Content Intelligence
- Content Marketing
- Analytics
- Artificial Intelligence
- Personalization
- Marketing Technology
- Agentic Web
- Conversion Tracking
- Attribution
- Event Ingestion
- Web Analytics
---
