---
api_key_in: []
api_specs:
- filename: commercetools-http-api-openapi.yml
  format: yaml
  label: Commercetools HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-http-api-openapi.yml
- filename: commercetools-import-api-openapi.yml
  format: yaml
  label: Commercetools Import API
  slug: import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-import-api-openapi.yml
- filename: commercetools-change-history-api-openapi.yml
  format: yaml
  label: Commercetools Change History API
  slug: change-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-change-history-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Commercetools Authentication
name_suffix: Authentication
oauth_flows: []
overview: commercetools secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: commercetools
provider_slug: commercetools
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token obtained from the commercetools authentication service using client credentials flow. Requires the view_audit_log scope.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commercetools-change-history-api-openapi.yml
  - openapi/commercetools-http-api-openapi.yml
  - openapi/commercetools-import-api-openapi.yml
  type: http
slug: commercetools-authentication
source_filename: commercetools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commercetools-change-history-api-openapi.yml, openapi/commercetools-http-api-openapi.yml,\n  openapi/commercetools-import-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token obtained from the commercetools authentication service\n    using client credentials flow. Requires the view_audit_log scope.\n  sources:\n  - openapi/commercetools-change-history-api-openapi.yml\n  - openapi/commercetools-http-api-openapi.yml\n  - openapi/commercetools-import-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/authentication/commercetools-authentication.yml
summary_line: http · 1 scheme
tags:
- Commerce
- Composable Commerce
- E-Commerce
- GraphQL
- REST
- SDK
---
