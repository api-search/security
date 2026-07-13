---
api_key_in: []
api_specs:
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Patients API
  slug: nookal-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Appointments API
  slug: nookal-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Clinic API
  slug: nookal-clinic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Invoices API
  slug: nookal-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
- filename: nookal-openapi.yml
  format: yaml
  label: Nookal Verification API
  slug: nookal-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/openapi/nookal-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Nookal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nookal secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nookal
provider_slug: nookal
scheme_count: 1
schemes:
- description: 'Nookal authenticates every request with an account-issued API key passed as the `api_key` parameter - in the query string for GET requests and as a form field for POST requests. The key is created inside the Nookal application (Setup / Integrations), where the account owner assigns it a configurable access level. Confirmed live: calling https://api.nookal.com/production/v2/verify without a key returns `{"status":"failure","details":{"errorCode":"L000_1","alerts":["Missing variable: api_key"]}}`. There is no OAuth flow; the API key is the sole credential. API access is available on the paid Professional and Enterprise plans.'
  in: query
  name: apiKeyQuery
  parameterName: api_key
  scheme: api-key
  sources:
  - https://api.nookal.com/developers
  - https://api.nookal.com/dev/reference/verify
  - openapi/nookal-openapi.yml
  type: apiKey
slug: nookal-authentication
source_filename: nookal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: openapi/nookal-openapi.yml + live probes of https://api.nookal.com/production/v2/\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameterName: api_key\n  scheme: api-key\n  description: >-\n    Nookal authenticates every request with an account-issued API key passed as\n    the `api_key` parameter - in the query string for GET requests and as a form\n    field for POST requests. The key is created inside the Nookal application\n    (Setup / Integrations), where the account owner assigns it a configurable\n    access level. Confirmed live: calling\n    https://api.nookal.com/production/v2/verify without a key returns\n    `{\"status\":\"failure\",\"details\":{\"errorCode\":\"L000_1\",\"alerts\":[\"Missing\n    variable: api_key\"]}}`. There is no OAuth flow; the API key is the sole\n    credential. API access is available on the paid Professional and Enterprise\n    plans.\n  sources:\n\
  \  - https://api.nookal.com/developers\n  - https://api.nookal.com/dev/reference/verify\n  - openapi/nookal-openapi.yml\nnotes: >-\n  The api_key requirement was confirmed against the live production host. The\n  key is transmitted as a request parameter over HTTPS (TLS), not in an\n  Authorization header. Treat the key as a secret and scope its access level in\n  the Nookal application to the minimum required.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nookal/refs/heads/main/authentication/nookal-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Practice Management
- Healthcare
- Allied Health
- Appointments
- Scheduling
- Patients
- Clinics
- Bookings
- Physiotherapy
- SaaS
---
