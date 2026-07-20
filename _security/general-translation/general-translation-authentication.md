---
api_key_in: []
api_specs:
- filename: general-translation-openapi-original.yml
  format: yaml
  label: General Translation API
  slug: general-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/openapi/general-translation-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: General Translation Authentication
name_suffix: Authentication
oauth_flows: []
overview: General Translation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: General Translation
provider_slug: general-translation
scheme_count: 1
schemes:
- alt_header: x-gt-api-key
  alt_header_note: 'The public API reference also documents sending the same key in an `x-gt-api-key` header instead of the Authorization bearer header.

    '
  description: 'API key sent as a bearer token in the standard `Authorization: Bearer <key>` header. Use a project key (`gtx-api-`, `gtx-dev-`) or an organization key (`gtx-org-`). Organization keys must also send `gt-project-id` on project-scoped routes.'
  key_permissions:
  - project:files:read
  - project:files:write
  - project:translations:enqueue
  - project:translations:generate
  - project:context:read
  - project:context:write
  - project:write
  name: Bearer
  scheme: bearer
  sources:
  - openapi/general-translation-openapi-original.yml
  type: http
slug: general-translation-authentication
source_filename: general-translation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/general-translation-openapi-original.yml\ndocs: https://generaltranslation.com/en-US/docs/api\nsummary:\n  types:\n  - http\n  api_key_prefixes:\n    development: gtx-dev-\n    production: gtx-api-\n    organization: gtx-org-\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'API key sent as a bearer token in the standard `Authorization: Bearer <key>`\n    header. Use a project key (`gtx-api-`, `gtx-dev-`) or an organization key (`gtx-org-`).\n    Organization keys must also send `gt-project-id` on project-scoped routes.'\n  alt_header: x-gt-api-key\n  alt_header_note: >\n    The public API reference also documents sending the same key in an\n    `x-gt-api-key` header instead of the Authorization bearer header.\n  key_permissions:\n    - project:files:read\n    - project:files:write\n    - project:translations:enqueue\n    - project:translations:generate\n    - project:context:read\n    - project:context:write\n\
  \    - project:write\n  sources:\n  - openapi/general-translation-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-translation/refs/heads/main/authentication/general-translation-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Internationalization
- Localization
- Translation
- Developer Tools
- Artificial Intelligence
- i18n
- SDKs
- Machine Translation
---
