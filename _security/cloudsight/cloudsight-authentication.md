---
api_key_in:
- header
api_specs:
- filename: cloudsight-images-api-openapi.yml
  format: yaml
  label: CloudSight Images API
  slug: cloudsight-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsight/refs/heads/main/openapi/cloudsight-images-api-openapi.yml
auth_types:
- apiKey
- oauth1
description: CloudSight documents two alternative authentication methods for the same API, captured from the "Authentication" section of the API Blueprint CloudSight publishes on Apiary. There is no OAuth 2.0, no OpenID Connect, and no scope surface — the key (or the OAuth 1.0a key/secret pair) is all-or-nothing against the account.
kind: authentication
layout: security
method: searched
name: Cloudsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudSight secures its APIs with apiKey and oauth1 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CloudSight
provider_slug: cloudsight
scheme_count: 2
schemes:
- description: 'Simple key-based authentication. On each request include the header `Authorization: CloudSight [key]`, replacing `[key]` with the key provided for the account.'
  format: 'Authorization: CloudSight [key]'
  in: header
  name: CloudSightKey
  parameter: Authorization
  sources:
  - openapi/cloudsight-images-openapi.yml
  - https://cloudsight.docs.apiary.io/api-description-document
  type: apiKey
- description: '"OAuth1-Simple" — the client calculates a signature from a key, secret, nonce, URL and the request parameters and sends the result in the `Authorization` header. CloudSight requires that the `image` parameter be EXCLUDED from the signature calculation. OpenAPI 3 has no native OAuth 1.0a security scheme, so this alternative is not expressible in openapi/cloudsight-images-openapi.yml and is recorded here only.'
  in: header
  name: OAuth1Simple
  parameter: Authorization
  sources:
  - https://cloudsight.docs.apiary.io/api-description-document
  spec: RFC 5849
  type: oauth1
slug: cloudsight-authentication
source_filename: cloudsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://cloudsight.docs.apiary.io/api-description-document\ndocs: https://cloudsight.docs.apiary.io\ndescription: >-\n  CloudSight documents two alternative authentication methods for the same API,\n  captured from the \"Authentication\" section of the API Blueprint CloudSight\n  publishes on Apiary. There is no OAuth 2.0, no OpenID Connect, and no scope\n  surface — the key (or the OAuth 1.0a key/secret pair) is all-or-nothing\n  against the account.\nsummary:\n  types:\n  - apiKey\n  - oauth1\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: none\nschemes:\n- name: CloudSightKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: CloudSight [key]'\n  description: >-\n    Simple key-based authentication. On each request include the header\n    `Authorization: CloudSight [key]`, replacing `[key]` with the key provided\n    for the account.\n\
  \  sources:\n  - openapi/cloudsight-images-openapi.yml\n  - https://cloudsight.docs.apiary.io/api-description-document\n- name: OAuth1Simple\n  type: oauth1\n  spec: RFC 5849\n  in: header\n  parameter: Authorization\n  description: >-\n    \"OAuth1-Simple\" — the client calculates a signature from a key, secret,\n    nonce, URL and the request parameters and sends the result in the\n    `Authorization` header. CloudSight requires that the `image` parameter be\n    EXCLUDED from the signature calculation. OpenAPI 3 has no native OAuth 1.0a\n    security scheme, so this alternative is not expressible in\n    openapi/cloudsight-images-openapi.yml and is recorded here only.\n  sources:\n  - https://cloudsight.docs.apiary.io/api-description-document\nkey_handling:\n  transport: >-\n    CloudSight recommends HTTPS; over plain HTTP the key is sent in clear text.\n    The documented base URL is https://api.cloudsight.ai/v1 (HTTPS, TLS 1.3\n    observed 2026-08-09).\n  secrecy: >-\n    \"Your\
  \ API key is very important and identifies any request as yours, so be\n    sure to keep it secret.\" — CloudSight API documentation.\n  rotation: not documented\n  key_issuance: >-\n    Keys are issued per account; the account surface is https://cloudsight.ai/login.\n    No self-service key documentation is published anonymously.\ngaps:\n- No OAuth 2.0 / OIDC surface, so no scoped or delegated access.\n- No documented key rotation or expiry policy.\n- No /.well-known/ discovery on any CloudSight host (see well-known/cloudsight-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudsight/refs/heads/main/authentication/cloudsight-authentication.yml
summary_line: apiKey/oauth1 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Computer-Vision
- Image Recognition
- Image Captioning
- Classification
- Media
---
