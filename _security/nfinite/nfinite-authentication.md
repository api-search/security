---
api_key_in: []
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Nfinite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nfinite secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nfinite
provider_slug: nfinite
scheme_count: 1
schemes:
- description: An opaque access token supplied as the `token` query parameter. Required (alongside a resource `url`) by the oEmbed endpoint; a request without it returns HTTP 400 code=VALIDATION_ERROR with "Required on path token".
  in: query
  name: token
  parameter: token
  sources:
  - https://my.nfinite.app/api/oembed
  - https://display.nfinite.app/api/oembed
  type: apiKey
slug: nfinite-authentication
source_filename: nfinite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: >-\n  Observed live from the undocumented internal app API at https://my.nfinite.app/api.\n  Nfinite publishes no OpenAPI, developer portal, or auth documentation; the\n  requirement below was inferred from a 400 VALIDATION_ERROR returned by\n  GET /api/oembed listing \"Required on path token\" among the missing parameters.\nsummary:\n  types:\n  - apiKey\n  note: >-\n    No public developer program. This is an internal, session/token-gated app\n    API backing the my.nfinite.app and display.nfinite.app applications. Tokens\n    are not self-serviceable via any documented flow.\nschemes:\n- name: token\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    An opaque access token supplied as the `token` query parameter. Required\n    (alongside a resource `url`) by the oEmbed endpoint; a request without it\n    returns HTTP 400 code=VALIDATION_ERROR with \"Required on path token\".\n  sources:\n  - https://my.nfinite.app/api/oembed\n\
  \  - https://display.nfinite.app/api/oembed\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nfinite/refs/heads/main/authentication/nfinite-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Visual Intelligence
- Digital Shelf
- Product Imagery
- Retail
- E-Commerce
- Artificial Intelligence
- Content Generation
---
