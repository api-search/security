---
api_key_in:
- header
api_specs:
- filename: simpletexting-campaigns-api-openapi.yml
  format: yaml
  label: SimpleTexting Campaigns API
  slug: simpletexting-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-campaigns-api-openapi.yml
- filename: simpletexting-contact-lists-api-openapi.yml
  format: yaml
  label: SimpleTexting Contact Lists API
  slug: simpletexting-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contact-lists-api-openapi.yml
- filename: simpletexting-contact-segments-api-openapi.yml
  format: yaml
  label: SimpleTexting Contact Segments API
  slug: simpletexting-contact-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contact-segments-api-openapi.yml
- filename: simpletexting-contacts-api-openapi.yml
  format: yaml
  label: SimpleTexting Contacts API
  slug: simpletexting-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contacts-api-openapi.yml
- filename: simpletexting-contacts-batch-operations-api-openapi.yml
  format: yaml
  label: SimpleTexting Contacts - Batch Operations API
  slug: simpletexting-contacts-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contacts-batch-operations-api-openapi.yml
- filename: simpletexting-custom-fields-api-openapi.yml
  format: yaml
  label: SimpleTexting Custom Fields API
  slug: simpletexting-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-custom-fields-api-openapi.yml
- filename: simpletexting-media-items-api-openapi.yml
  format: yaml
  label: SimpleTexting Media Items API
  slug: simpletexting-media-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-media-items-api-openapi.yml
- filename: simpletexting-messages-api-openapi.yml
  format: yaml
  label: SimpleTexting Messages API
  slug: simpletexting-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-messages-api-openapi.yml
- filename: simpletexting-tenant-api-openapi.yml
  format: yaml
  label: SimpleTexting Tenant API
  slug: simpletexting-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-tenant-api-openapi.yml
- filename: simpletexting-webhooks-api-openapi.yml
  format: yaml
  label: SimpleTexting Webhooks API
  slug: simpletexting-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-webhooks-api-openapi.yml
- filename: simpletexting-tenant-phones-api-openapi.yml
  format: yaml
  label: SimpleTexting Tenant phones API
  slug: simpletexting-tenant-phones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-tenant-phones-api-openapi.yml
- filename: simpletexting-webhook-reports-api-openapi.yml
  format: yaml
  label: SimpleTexting Webhook Reports API
  slug: simpletexting-webhook-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-webhook-reports-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Simpletexting Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleTexting secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SimpleTexting
provider_slug: simpletexting
scheme_count: 1
schemes:
- description: 'A single long-lived account bearer token, sent in the Authorization header on every request. SimpleTexting''s reference: "Each time you make a request to our API, we use a bearer token in your header to authenticate your account. API requests without authentication will fail. Your API token can be found under settings." Despite the "Bearer" convention, the scheme is declared in the OpenAPI as apiKey-in-header rather than http/bearer.'
  format: 'Authorization: Bearer <token>'
  in: header
  name: api_key
  parameter: Authorization
  sources:
  - openapi/_original/simpletexting-openapi.yml
  - https://api-doc.simpletexting.com/
  token_source: https://app2.simpletexting.com/integrations/webhooks (API / integrations settings)
  type: apiKey
slug: simpletexting-authentication
source_filename: simpletexting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\ndocs: https://api-doc.simpletexting.com/\nsource: >-\n  https://api-doc.simpletexting.com/ (Authentication section of SimpleTexting's own\n  reference) and the `api_key` securityScheme in the OpenAPI it publishes\n  (openapi/_original/simpletexting-openapi.yml, harvested 2026-08-13), confirmed by a\n  live unauthenticated probe of https://api-app2.simpletexting.com/v2/api/messages\n  returning HTTP 401 ERR_AUTH_TOKEN_MISSING.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  scopes: false\n  mtls: false\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <token>'\n  description: >-\n    A single long-lived account bearer token, sent in the Authorization header on\n    every request. SimpleTexting's reference: \"Each time you make a request to our\n    API, we use a bearer token in your header to authenticate your account. API\n    requests\
  \ without authentication will fail. Your API token can be found under\n    settings.\" Despite the \"Bearer\" convention, the scheme is declared in the\n    OpenAPI as apiKey-in-header rather than http/bearer.\n  token_source: https://app2.simpletexting.com/integrations/webhooks (API / integrations settings)\n  sources:\n  - openapi/_original/simpletexting-openapi.yml\n  - https://api-doc.simpletexting.com/\naccess_gate:\n  approval_required: true\n  evidence: >-\n    \"For additional security, our API is by approval only. If you'd like access, sign\n    up for a trial account and email support@simpletexting.net with details about your\n    use case.\" — https://api-doc.simpletexting.com/\n  contact: support@simpletexting.net\nauthorization_model:\n  scopes: none\n  restricted_keys: none\n  rotation_policy: not published\n  expiry: not published\n  note: >-\n    One token carries full account authority over messaging, contacts, media and\n    webhooks. There is no scope, no read-only key,\
  \ no per-integration credential and\n    no documented rotation or expiry, so least-privilege delegation to an agent is not\n    possible today.\nobserved:\n  probed: '2026-08-13'\n  request: GET https://api-app2.simpletexting.com/v2/api/messages with no Authorization header\n  http_status: 401\n  content_type: application/problem+json;charset=utf-8\n  error_code: ERR_AUTH_TOKEN_MISSING\nlegacy_v1:\n  docs: https://simpletexting.com/api/docs/\n  schemes:\n    - {name: bearer, in: header, parameter: Authorization, status: current for v1}\n    - {name: token, in: query, parameter: token, status: deprecated,\n       note: '\"Api token auth is only available for users that started using the v1 api before 09.01.2021\"'}\n  warning: >-\n    Query-parameter token auth leaks credentials into logs, proxies and referrers. It\n    is closed to new accounts but still served for older ones.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/authentication/simpletexting-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- SMS
- MMS
- Messaging
- Marketing
- Text Messaging
- SMS Marketing
- Communications
- Campaigns
- Contacts
- Webhook
- A2P 10DLC
---
