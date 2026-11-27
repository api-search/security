---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ownware-io-customers-api-openapi.yml
  format: yaml
  label: Ownware Customers API
  slug: ownware-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-customers-api-openapi.yml
- filename: ownware-io-licenses-api-openapi.yml
  format: yaml
  label: Ownware Licenses API
  slug: ownware-io-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-licenses-api-openapi.yml
- filename: ownware-io-orders-api-openapi.yml
  format: yaml
  label: Ownware Orders API
  slug: ownware-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-orders-api-openapi.yml
- filename: ownware-io-ping-api-openapi.yml
  format: yaml
  label: Ownware Ping API
  slug: ownware-io-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-ping-api-openapi.yml
- filename: ownware-io-redeem-codes-api-openapi.yml
  format: yaml
  label: Ownware Redeem Codes API
  slug: ownware-io-redeem-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-redeem-codes-api-openapi.yml
- filename: ownware-io-stats-api-openapi.yml
  format: yaml
  label: Ownware Stats API
  slug: ownware-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-stats-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ownware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ownware declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ownware
provider_slug: ownware-io
scheme_count: 1
schemes:
- evidence: 'It is authenticated with a static bearer key issued by the owner from the admin settings screen.


    Authorization: Bearer <key>'
  header: Authorization
  how_to_obtain: Contact the store owner to obtain the static bearer key.
  location: header
  name: Bearer
  type: http-bearer
slug: ownware-io-authentication
source_filename: ownware-io-authentication.yml
source_heading: Authentication Profile
source_url: https://ownware.io/auth.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ownware.io/auth.md\nsources:\n- https://ownware.io/auth.md\n- https://ownware.io/p/tokora\n- https://ownware.io/p/onboardora\n- https://ownware.io/guides/onboarding-checklists-derive-the-dates-dont-store-them\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'It is authenticated with a static bearer key issued by the owner from the admin settings screen.\n\n\n    Authorization: Bearer <key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Contact the store owner to obtain the static bearer key.\ndocs: https://ownware.io/auth.md\n"
source_yaml_url: https://artifacts.apis.io/ownware-io/authentication/ownware-io-authentication.yml
summary_line: 1 scheme
tags:
- Self‑Hosted Software
- Invoicing
- Appointment Booking
- Point-of-Sale
- Compliance Tools
- Expense Management
---
