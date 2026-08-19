---
api_key_in:
- query
auth_types:
- apiKey
- custom-signature
description: ''
kind: authentication
layout: security
method: searched
name: Launchmetrics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Launchmetrics secures its APIs with apiKey and custom-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Launchmetrics
provider_slug: launchmetrics
scheme_count: 2
schemes:
- description: An application identifier issued by Launchmetrics R&D. The docs describe app_id-only requests as the "less secure" of the two supported modes. The legacy spellings appId and appid are documented as deprecated; app_id is the current parameter name.
  in: query
  issuance: Not self-service. The reference says "if you don't have an app_id you should request one" and that the app_id and its secret are "provided by R&D" — there is no public sign-up, developer console or key-provisioning endpoint.
  name: app_id
  parameter: app_id
  required: true
  sources:
  - https://nap.launchmetrics.com/docs/search.html
  - https://nap.launchmetrics.com/docs/documents.html
  - https://nap.launchmetrics.com/docs/documentsV2.html
  - https://nap.launchmetrics.com/docs/medias.html
  - https://nap.launchmetrics.com/docs/auditlogs.html
  type: apiKey
- algorithm: HMAC-SHA1
  description: The "more secure" mode. Requests carry app_id, nonce, timestamp and signature query parameters. The scheme is explicitly modelled on the OAuth 1.0a-era Twitter request-signing recipe, which the docs cite as their source (dev.twitter.com/docs/auth/creating-signature).
  encoding: base64
  in: query
  name: app_id + signature
  parameters:
  - description: Application identifier issued by Launchmetrics R&D.
    name: app_id
  - description: Random string of at least 32 characters.
    name: nonce
  - description: Current time in seconds since the Unix epoch.
    name: timestamp
  - description: Base64-encoded HMAC-SHA1 of the signature base string, keyed with the app secret.
    name: signature
  required: false
  signature_base_string: http_method&url_encoded(request_url)&url_encoded(parameter_string)
  signature_steps:
  - Add timestamp, nonce and app_id to the request parameters.
  - Percent-encode every key and value (spaces as %20, never +, or the signature will not match).
  - Join each key and value with "=" and sort the resulting list alphabetically.
  - Join all parameters with "&" to produce the parameter_string.
  - Build signature_base = HTTP_METHOD & url_encoded(request_url) & url_encoded(parameter_string), where request_url excludes the protocol and any query parameters.
  - For non-form bodies (JSON or plain text), append a newline and the raw body bytes to signature_base.
  - HMAC-SHA1 signature_base with the app secret and base64-encode the binary output.
  - Send signature alongside the other parameters. For POST/PUT with a non-form body, the signature parameters must be placed on the URL query string, not in the body.
  sources:
  - https://nap.launchmetrics.com/docs/search.html
  type: custom-signature
slug: launchmetrics-authentication
source_filename: launchmetrics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://nap.launchmetrics.com/docs/search.html\ndocs: https://nap.launchmetrics.com/docs\nnote: >-\n  Derived by reading the public NAP API reference at nap.launchmetrics.com/docs, which repeats an\n  identical \"Authentication\" section on every one of the five service pages (Search, Documents,\n  Documents v2, Medias, Auditlogs). Launchmetrics publishes no OpenAPI securitySchemes block that\n  could be parsed mechanically, so every field below is transcribed from the published prose.\n  Launchmetrics is not an OAuth provider; there is no authorization server, no scope surface and no\n  /.well-known/openid-configuration on any Launchmetrics host (all probed 404 or SPA-shell).\nsummary:\n  types:\n  - apiKey\n  - custom-signature\n  api_key_in:\n  - query\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\nschemes:\n- name: app_id\n  type: apiKey\n  in: query\n  parameter: app_id\n  required: true\n  description:\
  \ >-\n    An application identifier issued by Launchmetrics R&D. The docs describe app_id-only requests as\n    the \"less secure\" of the two supported modes. The legacy spellings appId and appid are documented\n    as deprecated; app_id is the current parameter name.\n  issuance: >-\n    Not self-service. The reference says \"if you don't have an app_id you should request one\" and that\n    the app_id and its secret are \"provided by R&D\" — there is no public sign-up, developer console or\n    key-provisioning endpoint.\n  sources:\n  - https://nap.launchmetrics.com/docs/search.html\n  - https://nap.launchmetrics.com/docs/documents.html\n  - https://nap.launchmetrics.com/docs/documentsV2.html\n  - https://nap.launchmetrics.com/docs/medias.html\n  - https://nap.launchmetrics.com/docs/auditlogs.html\n- name: app_id + signature\n  type: custom-signature\n  in: query\n  algorithm: HMAC-SHA1\n  encoding: base64\n  required: false\n  description: >-\n    The \"more secure\" mode. Requests\
  \ carry app_id, nonce, timestamp and signature query parameters.\n    The scheme is explicitly modelled on the OAuth 1.0a-era Twitter request-signing recipe, which the\n    docs cite as their source (dev.twitter.com/docs/auth/creating-signature).\n  parameters:\n  - name: app_id\n    description: Application identifier issued by Launchmetrics R&D.\n  - name: nonce\n    description: Random string of at least 32 characters.\n  - name: timestamp\n    description: Current time in seconds since the Unix epoch.\n  - name: signature\n    description: Base64-encoded HMAC-SHA1 of the signature base string, keyed with the app secret.\n  signature_base_string: 'http_method&url_encoded(request_url)&url_encoded(parameter_string)'\n  signature_steps:\n  - Add timestamp, nonce and app_id to the request parameters.\n  - Percent-encode every key and value (spaces as %20, never +, or the signature will not match).\n  - Join each key and value with \"=\" and sort the resulting list alphabetically.\n  - Join\
  \ all parameters with \"&\" to produce the parameter_string.\n  - Build signature_base = HTTP_METHOD & url_encoded(request_url) & url_encoded(parameter_string),\n    where request_url excludes the protocol and any query parameters.\n  - For non-form bodies (JSON or plain text), append a newline and the raw body bytes to signature_base.\n  - HMAC-SHA1 signature_base with the app secret and base64-encode the binary output.\n  - Send signature alongside the other parameters. For POST/PUT with a non-form body, the signature\n    parameters must be placed on the URL query string, not in the body.\n  sources:\n  - https://nap.launchmetrics.com/docs/search.html\nobserved_behaviour:\n- probe: GET https://nap.launchmetrics.com/search/v1/ping\n  http_status: 200\n  note: Health endpoints answer unauthenticated; /ping returned {\"pong\":\"ok\"} inside the NAP envelope.\n- probe: GET https://api-ter.launchmetrics.com/v1/openapi.json\n  http_status: 401\n  body_code: APP_ID_NOT_VALID\n  note: >-\n\
  \    A machine-readable OpenAPI document exists on the api-ter host but is gated behind a valid app_id;\n    an unauthenticated request returns 401 APP_ID_NOT_VALID rather than 404. Recorded as evidence of a\n    gated contract, not saved — see conformance/ and the x-enrichment notes.\n- probe: GET https://api-ter.launchmetrics.com/v0/openapi.json\n  http_status: 400\n  body_code: MISSING_TENANT\n  note: The v0 (test) route additionally requires a tenant parameter.\ngaps:\n- No OAuth 2.0, OpenID Connect or mutual-TLS surface is documented or discoverable.\n- No published token rotation, expiry or revocation policy.\n- No self-service credential issuance; app_id and secret are handed out by Launchmetrics R&D.\n- HMAC-SHA1 is the only signing algorithm offered; no SHA-256 option is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchmetrics/refs/heads/main/authentication/launchmetrics-authentication.yml
summary_line: apiKey/custom-signature · 2 schemes
tags:
- Company
- SaaS
- Marketing
- Public Relations
- Media Monitoring
- Social Media
- Analytics
- Fashion
- Luxury
- Beauty
- Brand Performance
- Event Management
- Search
---
