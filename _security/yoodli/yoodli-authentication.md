---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yoodli-api-openapi.yml
  format: yaml
  label: Yoodli API
  slug: yoodli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/openapi/yoodli-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Yoodli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yoodli secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yoodli
provider_slug: yoodli
scheme_count: 1
schemes:
- applied_to: all 13 published operations (declared per-operation; there is no top-level security block)
  bearerFormat: null
  header: 'Authorization: Bearer <API key>'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/yoodli-api-openapi.yml
  type: http
slug: yoodli-authentication
source_filename: yoodli-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/yoodli-api-openapi.yml\ndocs: https://developers.yoodli.ai/docs/api-keys\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  model: long-lived bearer API key minted in the Yoodli admin UI\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: null\n  sources:\n  - openapi/yoodli-api-openapi.yml\n  applied_to: all 13 published operations (declared per-operation; there is no top-level security block)\n  header: 'Authorization: Bearer <API key>'\nkey_management:\n  kinds:\n  - name: Organization Management API key\n    scope: one Organization\n    created_by:\n    - Organization Administrator\n    - Organization Owner\n    path: Admin view -> Org Settings -> \"Access and SSO\" -> \"Organization Management API\" -> Manage -> Create API\n      key\n  - name: Multi Org Management API key\n    scope: a Multi Org and its member Organizations\n    created_by:\n\
  \    - Multi Org Administrator\n    path: Admin view -> Org Settings -> \"Manage Multi Org\" -> Settings -> \"Access\" -> \"Multi Org Management API\"\n      -> Manage -> Create API key\n  max_keys_per_entity: 3\n  expiration: 'Set at creation: an explicit expiry date, or \"Never expires\"'\n  shown_once: true\n  rotation: No rotation endpoint; a lost key cannot be re-displayed and must be replaced by creating a new one\n  prefix: null\n  token_id: Yoodli refers to an \"API Key Token ID\" in support guidance and asks for the FIRST HALF only, never the\n    full key\n  docs: https://developers.yoodli.ai/docs/api-keys\nscopes:\n  model: role-based, not scope-based\n  note: There is no OAuth surface and no scope vocabulary. Authorization is carried by which key kind was minted\n    and by the caller's admin role — 403 is returned when the caller is not an admin, and 404 is used in several\n    places to hide resources the caller cannot see. No scopes/ artifact is emitted; there is nothing\
  \ to enumerate.\ngaps:\n- No 401 response is declared on any operation despite BearerAuth on all 13.\n- No token-introspection, key-listing or key-revocation API — key lifecycle is UI-only.\n- No OIDC/OAuth discovery document is served on any host (all /.well-known probes 404 or return an SPA shell).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/authentication/yoodli-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Communication
- Coaching
- Learning and Development
- Sales Enablement
- Speech Analysis
- Human Resources
- Enterprise Software
- SaaS
- Identity Management
---
