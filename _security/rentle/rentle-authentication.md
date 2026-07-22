---
api_key_in:
- header
api_specs:
- filename: rentle-admin-openapi.json
  format: json
  label: Twice Admin API
  slug: twice-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/openapi/rentle-admin-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rentle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rentle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rentle
provider_slug: rentle
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. username = API key ID, password = API key secret. Each key is limited to the scopes selected when it was created, and only accesses data for its own merchant account.
  name: apiKeyBasic
  scheme: basic
  sources:
  - https://api.rentle.io/admin/
  type: http
slug: rentle-authentication
source_filename: rentle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.rentle.io/admin/\ndocs: https://api.rentle.io/admin/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    All requests authenticate with a standard API key using HTTP Basic\n    Authentication. The API key ID is the Basic username and the API key\n    secret is the Basic password. Keys are generated in the Admin UI\n    Integrations page and are scoped per merchant account. The OpenAPI\n    document does not declare the securityScheme; the model here is captured\n    from the Authentication section of the published docs.\nschemes:\n  - name: apiKeyBasic\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic Authentication. username = API key ID, password = API key\n      secret. Each key is limited to the scopes selected when it was created,\n      and only accesses data for its own merchant account.\n    sources: [https://api.rentle.io/admin/]\n\
  scopes:\n  model: >-\n    Scopes are selected per API key in the Admin UI when the key is created;\n    each endpoint documents the scope it requires. Rentle recommends enabling\n    only the scopes a key needs. The scope list is not enumerated in the\n    OpenAPI document.\nkey_management:\n  console: https://admin.rentle.io/account/integrations\n  secret_display: shown once at creation; store securely\n  revocation: delete the key from the Admin UI\nrequired_headers:\n  - name: X-Rentle-Version\n    required: true\n    description: Date-based API version, currently 2023-02-01, required on every request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentle/refs/heads/main/authentication/rentle-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Rental
- Commerce
- E-commerce
- Circular Economy
- Resale
- Subscriptions
- Bookings
- Webhooks
- SaaS
---
