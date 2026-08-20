---
api_key_in:
- query
api_specs:
- filename: qgiv-account-settings-api-openapi.yml
  format: yaml
  label: Qgiv Account Settings API
  slug: qgiv-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-account-settings-api-openapi.yml
- filename: qgiv-custom-amounts-api-openapi.yml
  format: yaml
  label: Qgiv Custom Amounts API
  slug: qgiv-custom-amounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-custom-amounts-api-openapi.yml
- filename: qgiv-custom-fields-api-openapi.yml
  format: yaml
  label: Qgiv Custom Fields API
  slug: qgiv-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-custom-fields-api-openapi.yml
- filename: qgiv-events-api-openapi.yml
  format: yaml
  label: Qgiv Events API
  slug: qgiv-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-events-api-openapi.yml
- filename: qgiv-mappings-api-openapi.yml
  format: yaml
  label: Qgiv Mappings API
  slug: qgiv-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-mappings-api-openapi.yml
- filename: qgiv-recurring-api-openapi.yml
  format: yaml
  label: Qgiv Recurring API
  slug: qgiv-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-recurring-api-openapi.yml
- filename: qgiv-refunds-api-openapi.yml
  format: yaml
  label: Qgiv Refunds API
  slug: qgiv-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-refunds-api-openapi.yml
- filename: qgiv-registrations-api-openapi.yml
  format: yaml
  label: Qgiv Registrations API
  slug: qgiv-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-registrations-api-openapi.yml
- filename: qgiv-statements-api-openapi.yml
  format: yaml
  label: Qgiv Statements API
  slug: qgiv-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-statements-api-openapi.yml
- filename: qgiv-transactions-api-openapi.yml
  format: yaml
  label: Qgiv Transactions API
  slug: qgiv-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Qgiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qgiv secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qgiv
provider_slug: qgiv
scheme_count: 1
schemes:
- description: Documented as a POST body field (`token=<API token>`), not a header or querystring value. Modeled here as an apiKey scheme because OpenAPI 3.0 has no first-class "form field" security type. The token is scoped to one or more specific forms in the Qgiv admin console.
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/qgiv-openapi.yml
  type: apiKey
slug: qgiv-authentication
source_filename: qgiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/qgiv-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: Documented as a POST body field (`token=<API token>`), not a header or querystring\n    value. Modeled here as an apiKey scheme because OpenAPI 3.0 has no first-class \"form field\"\n    security type. The token is scoped to one or more specific forms in the Qgiv admin console.\n  sources:\n  - openapi/qgiv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/authentication/qgiv-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Non-Profit
- Fundraising
- Donations
- Payments
- Peer-to-Peer
- Event
- Bloomerang
---
