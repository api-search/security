---
anonymous_access: false
api_key_in: []
api_specs:
- filename: farofinance-app-alerts-api-openapi.yml
  format: yaml
  label: farofinance-app Alerts API
  slug: farofinance-app-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-alerts-api-openapi.yml
- filename: farofinance-app-attestations-api-openapi.yml
  format: yaml
  label: farofinance-app Attestations API
  slug: farofinance-app-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-attestations-api-openapi.yml
- filename: farofinance-app-credentials-api-openapi.yml
  format: yaml
  label: farofinance-app Credentials API
  slug: farofinance-app-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-credentials-api-openapi.yml
- filename: farofinance-app-dashboard-api-openapi.yml
  format: yaml
  label: farofinance-app Dashboard API
  slug: farofinance-app-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-dashboard-api-openapi.yml
- filename: farofinance-app-keys-api-openapi.yml
  format: yaml
  label: farofinance-app Keys API
  slug: farofinance-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-keys-api-openapi.yml
- filename: farofinance-app-receipts-api-openapi.yml
  format: yaml
  label: farofinance-app Receipts API
  slug: farofinance-app-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-receipts-api-openapi.yml
- filename: farofinance-app-reports-api-openapi.yml
  format: yaml
  label: farofinance-app Reports API
  slug: farofinance-app-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-reports-api-openapi.yml
- filename: farofinance-app-suite-api-openapi.yml
  format: yaml
  label: farofinance-app Suite API
  slug: farofinance-app-suite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-suite-api-openapi.yml
- filename: farofinance-app-system-api-openapi.yml
  format: yaml
  label: farofinance-app System API
  slug: farofinance-app-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-system-api-openapi.yml
- filename: farofinance-app-verify-api-openapi.yml
  format: yaml
  label: farofinance-app Verify API
  slug: farofinance-app-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-verify-api-openapi.yml
- filename: farofinance-app-webhooks-api-openapi.yml
  format: yaml
  label: farofinance-app Webhooks API
  slug: farofinance-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/farofinance-app-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Farofinance App Authentication
name_suffix: Authentication
oauth_flows: []
overview: farofinance-app secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: farofinance-app
provider_slug: farofinance-app
scheme_count: 1
schemes:
- description: 'Faro API key. Send as `Authorization: Bearer <key>`. Get a key at https://farofinance.app or via `/v1/keys/request`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/farofinance-app-openapi-www.json
  - openapi/farofinance-app-openapi.json
  type: http
slug: farofinance-app-authentication
source_filename: farofinance-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/farofinance-app-openapi-www.json, openapi/farofinance-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Faro API key. Send as `Authorization: Bearer <key>`. Get a key at https://farofinance.app\n    or via `/v1/keys/request`.'\n  sources:\n  - openapi/farofinance-app-openapi-www.json\n  - openapi/farofinance-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/farofinance-app/authentication/farofinance-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
---
