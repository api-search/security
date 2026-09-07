---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wsc-sports-blaze-feed-api.json
  format: json
  label: WSC Sports Blaze Feed API
  slug: wsc-sports-blaze-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wsc-sports/refs/heads/main/openapi/wsc-sports-blaze-feed-api.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Wsc Sports Authentication
name_suffix: Authentication
oauth_flows: []
overview: WSC Sports secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WSC Sports
provider_slug: wsc-sports
scheme_count: 2
schemes:
- description: Feed API key issued by a WSC Sports account manager, sent on every request as the ApiKey query parameter. Explicitly distinct from the Experiences app API key used to initialize the mobile/Web SDK.
  example_form: https://blazefeed.clipro.tv/v1/stories?ApiKey={MyToken}
  in: query
  name: ApiKey
  parameter: ApiKey
  required: true
  sources:
  - https://dev.wsc-sports.com/docs/blazefeed-api-v1
  - openapi/wsc-sports-blaze-feed-api-reference.json
  type: apiKey
- bearerFormat: JWT
  description: Standard Bearer token, declared as the global security requirement in the generated upstream swagger document.
  name: Bearer
  note: Not described anywhere in the published documentation; treat ApiKey as the operative scheme.
  scheme: bearer
  sources:
  - openapi/wsc-sports-blaze-feed-api.json
  status: declared-in-spec-only
  type: http
slug: wsc-sports-authentication
source_filename: wsc-sports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://dev.wsc-sports.com/docs/blazefeed-api-v1\ndocs: https://dev.wsc-sports.com/docs/blazefeed-api-v1\nsummary:\n  types:\n  - apiKey\n  - http\n  primary: apiKey\n  transport: query parameter\n  note: >-\n    The two OpenAPI documents in openapi/ disagree about the auth scheme, and the documentation is\n    authoritative. The generated upstream swagger (blazefeed.clipro.tv/swagger/v1/swagger.json) declares a\n    global HTTP Bearer/JWT requirement, but the documentation-published reference spec and the Blazefeed\n    API guide both state the API is called with a Feed API key in the ApiKey query parameter, and every\n    published example uses it. The Bearer scheme appears to be a framework default left in the generated\n    document; no WSC Sports documentation describes obtaining or using a JWT for this API.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: ApiKey\n  required: true\n  description: >-\n\
  \    Feed API key issued by a WSC Sports account manager, sent on every request as the ApiKey query\n    parameter. Explicitly distinct from the Experiences app API key used to initialize the mobile/Web SDK.\n  example_form: https://blazefeed.clipro.tv/v1/stories?ApiKey={MyToken}\n  sources:\n  - https://dev.wsc-sports.com/docs/blazefeed-api-v1\n  - openapi/wsc-sports-blaze-feed-api-reference.json\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Standard Bearer token, declared as the global security requirement in the generated upstream swagger document.\n  status: declared-in-spec-only\n  note: Not described anywhere in the published documentation; treat ApiKey as the operative scheme.\n  sources:\n  - openapi/wsc-sports-blaze-feed-api.json\ncredential_issuance:\n  self_serve: false\n  process: Keys are issued by a WSC Sports account manager; there is no public signup or key-provisioning endpoint.\n  source: https://dev.wsc-sports.com/docs/blazefeed-api-v1\n\
  related_credentials:\n- name: Experiences app API key\n  used_by: Experiences SDK (iOS, Android, Web, React Native, Flutter) initialization\n  note: A separate credential from the Blazefeed Feed API key. The docs call this out explicitly to prevent confusion.\n  source: https://dev.wsc-sports.com/docs/personalization-explicit\nobserved:\n- url: https://blazefeed.clipro.tv/v1/stories\n  http_status: 401\n  note: Unauthenticated GET returns 401 with an empty body, confirming the surface is credential-gated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wsc-sports/refs/heads/main/authentication/wsc-sports-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Sports
- Video
- Media
- Artificial Intelligence
- Content
- Streaming
- SDK
- Highlights
- Personalization
---
