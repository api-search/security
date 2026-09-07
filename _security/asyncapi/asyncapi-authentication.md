---
anonymous_access: false
api_key_in: []
api_specs:
- filename: asyncapi.md
  format: yaml
  label: AsyncAPI Specification
  slug: asyncapi-spec
  spec_type: AsyncAPI
  url: https://github.com/asyncapi/spec/blob/master/spec/asyncapi.md
- filename: asyncapi-server-api-openapi.yml
  format: yaml
  label: AsyncAPI Server API
  slug: asyncapi-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-server-api-openapi.yml
- filename: asyncapi-bundle-api-openapi.yml
  format: yaml
  label: AsyncAPI Bundle API
  slug: asyncapi-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-bundle-api-openapi.yml
- filename: asyncapi-convert-api-openapi.yml
  format: yaml
  label: AsyncAPI Convert API
  slug: asyncapi-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-convert-api-openapi.yml
- filename: asyncapi-diff-api-openapi.yml
  format: yaml
  label: AsyncAPI Diff API
  slug: asyncapi-diff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-diff-api-openapi.yml
- filename: asyncapi-generate-api-openapi.yml
  format: yaml
  label: AsyncAPI Generate API
  slug: asyncapi-generate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-generate-api-openapi.yml
- filename: asyncapi-help-api-openapi.yml
  format: yaml
  label: AsyncAPI Help API
  slug: asyncapi-help-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-help-api-openapi.yml
- filename: asyncapi-parse-api-openapi.yml
  format: yaml
  label: AsyncAPI Parse API
  slug: asyncapi-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-parse-api-openapi.yml
- filename: asyncapi-validate-api-openapi.yml
  format: yaml
  label: AsyncAPI Validate API
  slug: asyncapi-validate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/openapi/asyncapi-validate-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Asyncapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: AsyncAPI declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AsyncAPI
provider_slug: asyncapi
scheme_count: 0
schemes: []
slug: asyncapi-authentication
source_filename: asyncapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: openapi/asyncapi-server-api-openapi.yml + live anonymous calls to https://api.asyncapi.com/v1\ndocs: https://api.asyncapi.com/v1/docs\nnote: >-\n  The AsyncAPI Server API declares no `components.securitySchemes` and no\n  `security` requirement on any of its eight operations, and an anonymous\n  POST https://api.asyncapi.com/v1/validate returned HTTP 200 with a full\n  ValidateResponse body on 2026-09-06 with no key, token or cookie. This is\n  a deliberately keyless public service operated by the AsyncAPI Initiative,\n  not an undocumented gap — the authentication model IS \"none\", and that is\n  what an agent needs to know.\nsummary:\n  types: []\n  model: none\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_access: true\n  registration_required: false\nschemes: []\nverification:\n  - request: POST https://api.asyncapi.com/v1/validate\n    credentials: none\n    http_status: 200\n    observed: '2026-09-06'\n  - request:\
  \ GET https://api.asyncapi.com/v1/help\n    credentials: none\n    http_status: 200\n    observed: '2026-09-06'\nrelated:\n  - >-\n    The AsyncAPI CLI has its own auth surface for FETCHING protected documents,\n    not for calling this API: `asyncapi config auth add PATTERN TOKEN` stores an\n    HTTP Authorization header to use when the CLI resolves a spec URL behind a\n    gate. Documented at https://www.asyncapi.com/docs/tools/cli/usage\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/authentication/asyncapi-authentication.yml
summary_line: 0 schemes
tags:
- Event-Driven
- Linux Foundation
- Messaging
- Standards
- Specification
---
