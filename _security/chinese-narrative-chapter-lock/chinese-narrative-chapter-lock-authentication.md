---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chinese-narrative-chapter-lock-openapi.json
  format: json
  label: cultureBiz chapter-lock
  slug: culturebiz-chapter-lock
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chinese-narrative-chapter-lock/refs/heads/main/openapi/chinese-narrative-chapter-lock-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Chinese Narrative Chapter Lock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chinese Narrative Chapter Lock declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chinese Narrative Chapter Lock
provider_slug: chinese-narrative-chapter-lock
scheme_count: 2
schemes:
- note: POST /v1/lock answered 200 without credentials (2026-09-05).
  style: none
  surface: https://culturebiz-xianxia-lock.onrender.com
  verified: probed
- header: X-RapidAPI-Key
  note: RapidAPI's platform-standard header scheme; keys are issued by RapidAPI on subscription, not by the provider. The origin contract itself does not declare it.
  style: apiKey
  surface: RapidAPI gateway (https://rapidapi.com/zhongzhir/api/chinese-narrative-chapter-lock)
  verified: searched
slug: chinese-narrative-chapter-lock-authentication
source_filename: chinese-narrative-chapter-lock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: >-\n  Derived from openapi/chinese-narrative-chapter-lock-openapi.json (which declares NO\n  securitySchemes — derive-authentication.py correctly produced no profile) and confirmed by a\n  live probed call: POST /v1/lock returned 200 with no credentials on 2026-09-05. RapidAPI\n  gateway details from the docs page and the provider's marketplace listing.\nsummary: >-\n  Two access paths. (1) Direct to the Render origin: no authentication at all — the OpenAPI\n  declares no securitySchemes and unauthenticated calls succeed. (2) Through the RapidAPI\n  marketplace gateway, which fronts the API with RapidAPI's standard key-in-header scheme and\n  meters requests against the subscribed plan.\nschemes:\n  - style: none\n    surface: https://culturebiz-xianxia-lock.onrender.com\n    verified: probed\n    note: POST /v1/lock answered 200 without credentials (2026-09-05).\n  - style: apiKey\n    surface: RapidAPI gateway (https://rapidapi.com/zhongzhir/api/chinese-narrative-chapter-lock)\n\
  \    header: X-RapidAPI-Key\n    verified: searched\n    note: >-\n      RapidAPI's platform-standard header scheme; keys are issued by RapidAPI on subscription,\n      not by the provider. The origin contract itself does not declare it.\noauth2: false\nopenidconnect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinese-narrative-chapter-lock/refs/heads/main/authentication/chinese-narrative-chapter-lock-authentication.yml
summary_line: 2 schemes
tags:
- localization
- translation
- NLP
- terminology-management
- CAT
- MT-preprocessing
- chinese-language
- webnovels
- publishing
- entertainment
---
