---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fwozen-com-api-keys-api-openapi.yml
  format: yaml
  label: Fwozen API keys API
  slug: fwozen-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-api-keys-api-openapi.yml
- filename: fwozen-com-audit-api-openapi.yml
  format: yaml
  label: Fwozen Audit API
  slug: fwozen-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-audit-api-openapi.yml
- filename: fwozen-com-billing-api-openapi.yml
  format: yaml
  label: Fwozen Billing API
  slug: fwozen-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-billing-api-openapi.yml
- filename: fwozen-com-branches-api-openapi.yml
  format: yaml
  label: Fwozen Branches API
  slug: fwozen-com-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-branches-api-openapi.yml
- filename: fwozen-com-enforcement-api-openapi.yml
  format: yaml
  label: Fwozen Enforcement API
  slug: fwozen-com-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-enforcement-api-openapi.yml
- filename: fwozen-com-exceptions-api-openapi.yml
  format: yaml
  label: Fwozen Exceptions API
  slug: fwozen-com-exceptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-exceptions-api-openapi.yml
- filename: fwozen-com-freezes-api-openapi.yml
  format: yaml
  label: Fwozen Freezes API
  slug: fwozen-com-freezes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-freezes-api-openapi.yml
- filename: fwozen-com-organizations-api-openapi.yml
  format: yaml
  label: Fwozen Organizations API
  slug: fwozen-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-organizations-api-openapi.yml
- filename: fwozen-com-repositories-api-openapi.yml
  format: yaml
  label: Fwozen Repositories API
  slug: fwozen-com-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-repositories-api-openapi.yml
- filename: fwozen-com-schedules-api-openapi.yml
  format: yaml
  label: Fwozen Schedules API
  slug: fwozen-com-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-schedules-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fwozen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fwozen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fwozen
provider_slug: fwozen-com
scheme_count: 1
schemes:
- bearerFormat: fwz_<env>_<40 base58>
  description: 'Org-scoped, never user-scoped: the scope list IS the authorization. Calling a

    session-only route with a key returns **403 `credential_type_not_allowed`**, never 401,

    so scripts get an actionable message.


    **Where one comes from.** Sign in at

    [https://fwozen.com/app/settings/api-keys](https://fwozen.com/app/settings/api-keys) as an owner or an

    admin, press **Create key**, tick the narrowest scopes '
  name: bearerApiKey
  scheme: bearer
  sources:
  - openapi/fwozen-com-openapi.yml
  type: http
slug: fwozen-com-authentication
source_filename: fwozen-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/fwozen-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: fwz_<env>_<40 base58>\n  description: \"Org-scoped, never user-scoped: the scope list IS the authorization. Calling\\\n    \\ a\\nsession-only route with a key returns **403 `credential_type_not_allowed`**, never\\\n    \\ 401,\\nso scripts get an actionable message.\\n\\n**Where one comes from.** Sign in at\\n\\\n    [https://fwozen.com/app/settings/api-keys](https://fwozen.com/app/settings/api-keys) as\\\n    \\ an owner or an\\nadmin, press **Create key**, tick the narrowest scopes \"\n  sources:\n  - openapi/fwozen-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fwozen-com/authentication/fwozen-com-authentication.yml
summary_line: http · 1 scheme
tags:
- GitHub
- code freeze
- merge freeze
- deploy gate
- Security
---
