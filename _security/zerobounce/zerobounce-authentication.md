---
api_key_in: []
api_specs:
- filename: zerobounce-validation-api-openapi.yml
  format: yaml
  label: ZeroBounce Validation API
  slug: zerobounce-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerobounce/refs/heads/main/openapi/zerobounce-validation-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Zerobounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZeroBounce declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: ZeroBounce
provider_slug: zerobounce
scheme_count: 3
schemes:
- applies_to:
  - GET /v2/validate
  - GET /v2/getcredits
  - GET /v2/getapiusage
  - GET /v2/scoring
  - GET /v2/activity
  - GET /v2/guessformat
  - GET bulkapi.zerobounce.net/v2/filestatus
  - GET bulkapi.zerobounce.net/v2/getfile
  - GET bulkapi.zerobounce.net/v2/deletefile
  - GET bulkapi.zerobounce.net/v2/scoring/*
  - GET bulkapi.zerobounce.net/listS3files
  description: Every GET operation on api-us / api-eu / api.zerobounce.net /v2 and on bulkapi.zerobounce.net takes `api_key` as a query-string parameter, e.g. GET /v2/validate?api_key=<key>&email=<address>.
  evidence: collections/zerobounce-api-v2-official.postman_collection.json
  id: api_key_query
  in: query
  name: api_key
  type: apiKey
- applies_to:
  - POST /v2/validatebatch
  - POST /v2/filters/add
  - POST /v2/filters/delete
  - POST bulkapi.zerobounce.net/v2/sendfile
  - POST bulkapi.zerobounce.net/v2/scoring/sendfile
  description: POST operations carry `api_key` in the JSON body (validatebatch, filters/add, filters/delete) or as a multipart form field (sendfile, scoring/sendfile, validateS3file, scoreS3file, exportS3file).
  evidence: collections/zerobounce-api-v2-official.postman_collection.json
  id: api_key_body
  in: body
  name: api_key
  type: apiKey
- applies_to:
  - validate
  - validateBatch
  description: 'The ChatGPT-plugin endpoints on members-api.zerobounce.net accept an OPTIONAL api_key: an unauthenticated caller gets up to 3 single-validation requests per day. Batch validation on that host requires a key.'
  evidence: openapi/zerobounce-validation-api-openapi.yml
  id: api_key_optional_plugin
  in: body
  name: api_key
  optional: true
  type: apiKey
slug: zerobounce-authentication
source_filename: zerobounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.zerobounce.net/docs/api-dashboard\ndocs: https://www.zerobounce.net/docs/email-validation-api-quickstart\nsummary: >-\n  ZeroBounce v2 uses a single account-level API key passed as a plain request parameter.\n  There is no OAuth, no OpenID Connect, no scopes, no bearer-token header, and no mutual\n  TLS. One key carries full authority over the account, including spending validation\n  credits, so an agent handed this key can incur cost without further constraint.\nschemes:\n  - id: api_key_query\n    type: apiKey\n    in: query\n    name: api_key\n    description: >-\n      Every GET operation on api-us / api-eu / api.zerobounce.net /v2 and on\n      bulkapi.zerobounce.net takes `api_key` as a query-string parameter, e.g.\n      GET /v2/validate?api_key=<key>&email=<address>.\n    applies_to:\n      - 'GET /v2/validate'\n      - 'GET /v2/getcredits'\n      - 'GET /v2/getapiusage'\n      - 'GET /v2/scoring'\n   \
  \   - 'GET /v2/activity'\n      - 'GET /v2/guessformat'\n      - 'GET bulkapi.zerobounce.net/v2/filestatus'\n      - 'GET bulkapi.zerobounce.net/v2/getfile'\n      - 'GET bulkapi.zerobounce.net/v2/deletefile'\n      - 'GET bulkapi.zerobounce.net/v2/scoring/*'\n      - 'GET bulkapi.zerobounce.net/listS3files'\n    evidence: collections/zerobounce-api-v2-official.postman_collection.json\n  - id: api_key_body\n    type: apiKey\n    in: body\n    name: api_key\n    description: >-\n      POST operations carry `api_key` in the JSON body (validatebatch, filters/add,\n      filters/delete) or as a multipart form field (sendfile, scoring/sendfile,\n      validateS3file, scoreS3file, exportS3file).\n    applies_to:\n      - 'POST /v2/validatebatch'\n      - 'POST /v2/filters/add'\n      - 'POST /v2/filters/delete'\n      - 'POST bulkapi.zerobounce.net/v2/sendfile'\n      - 'POST bulkapi.zerobounce.net/v2/scoring/sendfile'\n    evidence: collections/zerobounce-api-v2-official.postman_collection.json\n\
  \  - id: api_key_optional_plugin\n    type: apiKey\n    in: body\n    name: api_key\n    optional: true\n    description: >-\n      The ChatGPT-plugin endpoints on members-api.zerobounce.net accept an OPTIONAL\n      api_key: an unauthenticated caller gets up to 3 single-validation requests per day.\n      Batch validation on that host requires a key.\n    applies_to:\n      - validate\n      - validateBatch\n    evidence: openapi/zerobounce-validation-api-openapi.yml\n\nkey_management:\n  created_in: ZeroBounce member dashboard (API / Developer section)\n  docs: https://www.zerobounce.net/docs/api-dashboard\n  signup: https://www.zerobounce.net/members/createaccount\n  rotation: >-\n    ZeroBounce documents an \"API Keys Management\" section in the dashboard docs; key\n    rotation is performed from the dashboard. The provider's own MCP README advises using\n    separate keys per environment and rotating them periodically, which implies multiple\n    keys per account are supported.\n\
  \  scopes: none\n  expiry: none documented\n\ntransport:\n  https_required: true\n  tls_support_page: https://www.zerobounce.net/docs/api-dashboard/tls-support\n  regions:\n    - host: https://api-us.zerobounce.net\n      residency: United States only\n    - host: https://api-eu.zerobounce.net\n      residency: European Union only\n    - host: https://api.zerobounce.net\n      residency: >-\n        Legacy endpoint; per ZeroBounce's own endpoints page it now serves EU validations\n        and interactions only.\n\nrisks:\n  - >-\n    The key travels in the query string on the majority of operations, so it lands in\n    proxy logs, browser history and referrer headers. Any integration that logs full URLs\n    is logging the credential.\n  - >-\n    No scopes means read-only agent use (get_credits, get_api_usage) cannot be separated\n    from spend-incurring use (validate, sendfile, scoring).\n  - >-\n    ZeroBounce applies a punitive auth-failure policy rather than a scoped one: 200 bad\n\
  \    API key requests in 1 hour triggers a 1-hour to 1-day block on the whole account key.\n\nnot_present:\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  http_bearer: false\n  jwt: false\n  webhook_signing: >-\n    ZeroBounce POSTs bulk-completion callbacks to a caller-supplied return_url but\n    documents no signature, shared secret or verification header on that request. See\n    asyncapi/zerobounce-webhooks.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerobounce/refs/heads/main/authentication/zerobounce-authentication.yml
summary_line: 3 schemes
tags:
- Email Validation
- Email Deliverability
- Email Verification
- Marketing
- Lead Scoring
- Anti-Spam
- Data Quality
- Email Finder
- Deliverability Monitoring
- DMARC
---
