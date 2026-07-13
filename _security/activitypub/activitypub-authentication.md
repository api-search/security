---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Activitypub Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActivityPub secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ActivityPub
provider_slug: activitypub
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer token for client-to-server authentication
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/activitypub-openapi.yml
  type: http
- description: HTTP Signatures (draft-cavage-http-signatures) for server-to-server authentication. The Signature header contains keyId, algorithm, headers, and signature fields.
  in: header
  name: HTTPSignature
  parameter: Signature
  sources:
  - openapi/activitypub-openapi.yml
  type: apiKey
slug: activitypub-authentication
source_filename: activitypub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activitypub-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token for client-to-server authentication\n  sources:\n  - openapi/activitypub-openapi.yml\n- name: HTTPSignature\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: HTTP Signatures (draft-cavage-http-signatures) for server-to-server authentication.\n    The Signature header contains keyId, algorithm, headers, and signature fields.\n  sources:\n  - openapi/activitypub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activitypub/refs/heads/main/authentication/activitypub-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Open Standard
- Social Networks
- Federation
- Fediverse
- W3C
---
