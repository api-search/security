---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagelemon-com-account-api-openapi.yml
  format: yaml
  label: Page Lemon Account API
  slug: pagelemon-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-account-api-openapi.yml
- filename: pagelemon-com-automations-api-openapi.yml
  format: yaml
  label: Page Lemon Automations API
  slug: pagelemon-com-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-automations-api-openapi.yml
- filename: pagelemon-com-bookings-api-openapi.yml
  format: yaml
  label: Page Lemon Bookings API
  slug: pagelemon-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-bookings-api-openapi.yml
- filename: pagelemon-com-lists-api-openapi.yml
  format: yaml
  label: Page Lemon Lists API
  slug: pagelemon-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-lists-api-openapi.yml
- filename: pagelemon-com-pages-api-openapi.yml
  format: yaml
  label: Page Lemon Pages API
  slug: pagelemon-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-pages-api-openapi.yml
- filename: pagelemon-com-payments-api-openapi.yml
  format: yaml
  label: Page Lemon Payments API
  slug: pagelemon-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-payments-api-openapi.yml
- filename: pagelemon-com-platform-api-openapi.yml
  format: yaml
  label: Page Lemon Platform API
  slug: pagelemon-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-platform-api-openapi.yml
- filename: pagelemon-com-rules-api-openapi.yml
  format: yaml
  label: Page Lemon Rules API
  slug: pagelemon-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-rules-api-openapi.yml
- filename: pagelemon-com-sign-in-api-openapi.yml
  format: yaml
  label: Page Lemon Sign In API
  slug: pagelemon-com-sign-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-sign-in-api-openapi.yml
- filename: pagelemon-com-views-api-openapi.yml
  format: yaml
  label: Page Lemon Views API
  slug: pagelemon-com-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-views-api-openapi.yml
auth_types: []
description: Authentication via API token
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Page Lemon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Page Lemon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Page Lemon
provider_slug: pagelemon-com
scheme_count: 1
schemes:
- evidence: 'Send it as a header on every request:


    ```bash

    curl -sS -H "Authorization: Bearer $PAGELEMON_TOKEN" https://api.pagelemon.com/v2/sites

    ```'
  header: Authorization
  how_to_obtain: Create a token in the Page Lemon dashboard (dash.pagelemon.com/account/tokens) and copy the value that starts with `pl_apikey_`.
  location: header
  name: API token
  type: http-bearer
slug: pagelemon-com-authentication
source_filename: pagelemon-com-authentication.yml
source_heading: Authentication Profile
source_url: https://pagelemon.com/docs/api-tokens.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pagelemon.com/docs/api-tokens.md\nsources:\n- https://pagelemon.com/docs/api-tokens.md\n- https://pagelemon.com/features/developers\n- https://pagelemon.com/docs/api-tokens\ndescription: Authentication via API token\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: 'Send it as a header on every request:\n\n\n    ```bash\n\n    curl -sS -H \"Authorization: Bearer $PAGELEMON_TOKEN\" https://api.pagelemon.com/v2/sites\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the Page Lemon dashboard (dash.pagelemon.com/account/tokens) and copy the value that starts with `pl_apikey_`.\nnote: No OAuth2 flows, API keys, or other authentication methods are documented on the provided pages.\ndocs: https://pagelemon.com/docs/api-tokens.md\n"
source_yaml_url: https://artifacts.apis.io/pagelemon-com/authentication/pagelemon-com-authentication.yml
summary_line: 1 scheme
tags:
- Website Builder
- Booking
- Payments
- Integration
- Developers
---
