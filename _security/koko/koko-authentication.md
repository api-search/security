---
api_key_in: []
api_specs:
- filename: koko-crisis-helplines-openapi.yml
  format: yaml
  label: Koko Crisis Helplines API
  slug: crisis-helplines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koko/refs/heads/main/openapi/koko-crisis-helplines-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: searched
name: Koko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koko secures its APIs with none and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Koko
provider_slug: koko
scheme_count: 1
schemes:
- api: Koko Keywords API
  in_env: KOKO_KEYWORDS_AUTH
  name: KokoKeywordsBasic
  scheme: basic
  sources:
  - https://developers.kokocares.org/docs/quickstart
  type: http
slug: koko-authentication
source_filename: koko-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developers.kokocares.org/docs/quickstart\ndocs: https://developers.kokocares.org/docs/quickstart\nnotes: >-\n  Koko runs two distinct APIs with two different auth postures. The Crisis Helplines\n  API is public and unauthenticated (its OpenAPI declares `security: []` and the info\n  description states \"No authentication required (public API)\"); access is instead\n  gated by a server-side CORS origin allowlist, which returns 403 to any origin that\n  is not registered. The Koko Keywords API requires HTTP Basic credentials issued by\n  Koko on request.\nsummary:\n  types: [none, http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\napis:\n  - api: Crisis Helplines API\n    auth: none\n    source: openapi/koko-crisis-helplines-openapi.yml\n    detail: >-\n      OpenAPI declares an empty top-level `security: []`. Access control is by CORS\n      origin allowlist enforced server-side; unregistered origins\
  \ receive HTTP 403 with\n      a text/plain body (\"Forbidden: no allowed origins configured\" or\n      \"Forbidden: Origin <origin> not allowed\"). Verified live 2026-07-19.\n  - api: Koko Keywords API\n    auth: http-basic\n    source: https://developers.kokocares.org/docs/quickstart\n    detail: >-\n      Credentials are supplied as `username:password` via the KOKO_KEYWORDS_AUTH\n      environment variable and sent as HTTP Basic authorization to\n      https://api.kokocares.org/keywords. The host answers 401 with\n      `WWW-Authenticate: Basic realm=\"Restricted Area\"` when unauthenticated\n      (verified 2026-07-19). Invalid credentials surface as a fatal client error.\n    credential_request: https://r.kokocares.org/api_signup\n    version_header: {name: X-API-VERSION, value: v3}\n    support_contact: api@kokocares.org\nschemes:\n  - name: KokoKeywordsBasic\n    type: http\n    scheme: basic\n    api: Koko Keywords API\n    in_env: KOKO_KEYWORDS_AUTH\n    sources: [https://developers.kokocares.org/docs/quickstart]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koko/refs/heads/main/authentication/koko-authentication.yml
summary_line: none/http · 1 scheme
tags:
- Company
- Mental Health
- Crisis Support
- Suicide Prevention
- Trust and Safety
- Content Moderation
- Nonprofit
- Health
- Helplines
---
