---
api_key_in: []
api_specs:
- filename: wattwatchers-rest-api-v3-openapi.json
  format: json
  label: Wattwatchers REST API v3 (Mercury)
  slug: wattwatchers-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wattwatchers/refs/heads/main/openapi/wattwatchers-rest-api-v3-openapi.json
auth_types:
- http
description: 'Wattwatchers REST API v3 (Mercury) uses a single authentication mechanism: an HTTP Bearer token ("API key") issued by hand by Wattwatchers. There is no OAuth, no OpenID Connect, no mTLS and no scope surface. Authorization is not expressed in the token — it is expressed as the SET OF DEVICES Wattwatchers assigns to that key, plus coarse permission levels (added in v3.5) that control whether the key may change device metadata and/or configuration. Derived from the OpenAPI securityScheme and upgraded from the published auth page.'
kind: authentication
layout: security
method: searched
name: Wattwatchers Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wattwatchers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wattwatchers
provider_slug: wattwatchers
scheme_count: 1
schemes:
- applies_to: Every documented operation. Note the spec declares no top-level `security` array — BearerAuth is applied per-operation on listDevices and getDevice and is required in practice everywhere (an anonymous GET /devices returns 401 UNAUTHORIZED).
  description: Bearer token authentication
  header: Authorization
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wattwatchers-rest-api-v3-openapi.json
  token_prefix: key_
  type: http
  value_format: Bearer key_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
slug: wattwatchers-authentication
source_filename: wattwatchers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/wattwatchers-rest-api-v3-openapi.json\ndocs: https://docs.wattwatchers.com.au/api/v3/auth.html\ndescription: >-\n  Wattwatchers REST API v3 (Mercury) uses a single authentication mechanism: an\n  HTTP Bearer token (\"API key\") issued by hand by Wattwatchers. There is no\n  OAuth, no OpenID Connect, no mTLS and no scope surface. Authorization is not\n  expressed in the token — it is expressed as the SET OF DEVICES Wattwatchers\n  assigns to that key, plus coarse permission levels (added in v3.5) that control\n  whether the key may change device metadata and/or configuration. Derived from\n  the OpenAPI securityScheme and upgraded from the published auth page.\nsummary:\n  types:\n    - http\n  api_key_in: []\n  oauth2_flows: []\n  self_serve: false\n  scopes: false\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    description: Bearer token authentication\n    sources:\n      - openapi/wattwatchers-rest-api-v3-openapi.json\n\
  \    header: Authorization\n    value_format: 'Bearer key_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'\n    token_prefix: key_\n    applies_to: >-\n      Every documented operation. Note the spec declares no top-level `security`\n      array — BearerAuth is applied per-operation on listDevices and getDevice\n      and is required in practice everywhere (an anonymous GET /devices returns\n      401 UNAUTHORIZED).\nkey_issuance:\n  self_serve: false\n  signup_form: false\n  free_tier: false\n  sandbox_key: false\n  process:\n    - Own or manage Wattwatchers Auditor hardware.\n    - Obtain access to the Fleet Management app (https://fleet.wattwatchers.com.au) via Wattwatchers support.\n    - The existing key is displayed under the profile menu of the Fleet app.\n    - 'For a new key: contact the Wattwatchers team. They set it up, assign the correct devices and permissions, and distribute it securely.'\n  quote: >-\n    \"Please contact the Wattwatchers team to have an API key setup. We will\n    distribute\
  \ the API key to you securely once we have set it up and assigned\n    the correct devices and related permissions.\"\n  console: https://fleet.wattwatchers.com.au\nauthorization_model:\n  mechanism: device-assignment\n  description: >-\n    \"The API key represents a set of permissions to a pre-defined set of devices\n    that the client application is permitted to access (read and modify).\" To\n    restrict access to a subset of devices you must have Wattwatchers create an\n    additional key. There is no runtime scoping, no delegation and no\n    per-request audience selection.\n  permission_levels:\n    introduced: v3.5 (2020-05-25)\n    description: >-\n      \"Additional permission levels to API keys relating to changing device\n      metadata and/or configuration.\" Read, metadata-write and\n      configuration-write are distinguished at key-issuance time, not requested\n      per call. A key lacking the level returns 403 FORBIDDEN.\n  masking: >-\n    A device not assigned to\
  \ the key returns 404 NOT_FOUND, not 403 — existence\n    is masked as well as access.\ntoken_lifecycle:\n  expiry: none-by-default\n  detail: '\"This token lives until it is expired by Wattwatchers.\" There is no client-driven rotation, refresh or revocation endpoint.'\n  forced_rotation: >-\n    If Wattwatchers become aware of a key being disclosed insecurely (e.g. pasted\n    into an email or a support ticket) they automatically retire and refresh it,\n    and notify the technical contacts on file.\n  disclosure_hygiene: >-\n    Docs instruct customers to identify a key by its LAST 5 CHARACTERS only when\n    communicating with support, never the whole value.\nkey_handling_guidance:\n  - Do not hard-code the key into an application or commit it to source control.\n  - Store it as an environment variable server-side.\n  - Never store it in browser cookies or local storage; a browser app should only receive it over HTTPS after the user is authenticated.\n  - Do not send the key by insecure\
  \ email or web-based communication tools.\ndiscovery_probes:\n  - {url: 'https://api-v3.wattwatchers.com.au/.well-known/openid-configuration', status: 404}\n  - {url: 'https://api-v3.wattwatchers.com.au/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://api-v3.wattwatchers.com.au/.well-known/oauth-protected-resource', status: 404}\n  - {url: 'https://api-v3.wattwatchers.com.au/devices', status: 401, note: 'anonymous request returns {\"code\":\"UNAUTHORIZED\",...} — the gate is real and enforced'}\nscopes:\n  supported: false\n  note: >-\n    No OAuth scope surface exists, so no scopes/ artifact is emitted for this\n    provider. Permission is a property of the issued key, not of the request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wattwatchers/refs/heads/main/authentication/wattwatchers-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- Australia
- Utilities
- Electricity
- Smart Metering
- Energy Data
- IoT
- Solar
- DER
- Demand Response
---
