---
api_key_in: []
api_specs:
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Shops API
  slug: tekmetric-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Customers API
  slug: tekmetric-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Vehicles API
  slug: tekmetric-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Repair Orders API
  slug: tekmetric-repair-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Jobs API
  slug: tekmetric-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Employees API
  slug: tekmetric-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Appointments API
  slug: tekmetric-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Inventory API
  slug: tekmetric-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Canned Jobs API
  slug: tekmetric-canned-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tekmetric Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tekmetric secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tekmetric
provider_slug: tekmetric
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token
  name: oauth2
  sources:
  - openapi/tekmetric-openapi.yml
  type: oauth2
slug: tekmetric-authentication
source_filename: tekmetric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tekmetric-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://shop.tekmetric.com/api/v1/oauth/token\n    scopes: 0\n  description: OAuth 2.0 client credentials grant. Requires an approved Client ID/Secret issued\n    by Tekmetric after a manual request-access review (reported at roughly 2-3 weeks).\n  sources:\n  - openapi/tekmetric-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/authentication/tekmetric-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Automotive
- Auto Repair
- Shop Management
- Fleet
- Vertical SaaS
---
