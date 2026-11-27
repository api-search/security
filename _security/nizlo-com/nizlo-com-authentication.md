---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nizlo-com-nizlo-rmm-api-openapi.yml
  format: yaml
  label: Nizlo RMM API
  slug: nizlo-rmm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nizlo-com/openapi/nizlo-com-nizlo-rmm-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nizlo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nizlo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nizlo
provider_slug: nizlo-com
scheme_count: 1
schemes:
- bearerFormat: Nizlo personal access token
  description: Create a permission-limited token from an active technician account. Tokens remain tenant-scoped and inherit that technician's permissions.
  docs_text: A technician selects 1–32 permissions and a 30, 90, 180, or 365-day lifetime. Effective access is always the intersection of those token permissions and the technician's current role, so removing role authority takes effect immediately.
  lifetimes_days:
  - 30
  - 90
  - 180
  - 365
  name: personalAccessToken
  permissions: 1-32 permissions, intersected with the technician current role
  scheme: bearer
  service_accounts: Not currently. Personal access tokens remain accountable to an active technician identity and tenant.
  sources:
  - openapi/nizlo-com-nizlo-rmm-api-openapi.yml
  token_prefix: nizlo_pat_
  type: http
slug: nizlo-com-authentication
source_filename: nizlo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: searched\nsource: https://nizlo.com/rmm-api\nsummary:\n  types:\n  - http\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: Nizlo personal access token\n  description: Create a permission-limited token from an active technician account.\n    Tokens remain tenant-scoped and inherit that technician's permissions.\n  sources:\n  - openapi/nizlo-com-nizlo-rmm-api-openapi.yml\n  token_prefix: nizlo_pat_\n  lifetimes_days:\n  - 30\n  - 90\n  - 180\n  - 365\n  permissions: 1-32 permissions, intersected with the technician current role\n  docs_text: A technician selects 1–32 permissions and a 30, 90, 180, or 365-day lifetime.\n    Effective access is always the intersection of those token permissions and the\n    technician's current role, so removing role authority takes effect immediately.\n  service_accounts: Not currently. Personal access tokens remain accountable to an\n    active technician identity and tenant.\n\
  docs: https://nizlo.com/rmm-api\nnotes: Browser sessions manage tokens; bearer credentials cannot manage their own\n  token lifecycle. Agent and enrollment credentials are separate and are not interchangeable\n  with technician API tokens.\n"
source_yaml_url: https://artifacts.apis.io/nizlo-com/authentication/nizlo-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- RMM
- Remote Monitoring
- MSP
- Windows
---
