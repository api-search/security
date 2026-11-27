---
anonymous_access: false
api_key_in: []
api_specs:
- filename: farofinance-app-api-openapi.json
  format: json
  label: Faro Api API
  slug: faro-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farofinance-app/openapi/_original/farofinance-app-api-openapi.json
auth_types: []
description: Authentication methods as documented on the Faro Quickstart page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Faro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Faro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Faro
provider_slug: farofinance-app
scheme_count: 1
schemes:
- evidence: 'Send it on every request as a bearer token: Authorization: Bearer <your-key>'
  header: Authorization
  how_to_obtain: Sign up at /signup with your email and location. Faro issues your API key immediately in the browser (shown once), so copy and store it right away.
  location: header
  name: Bearer
  type: http-bearer
slug: farofinance-app-authentication
source_filename: farofinance-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.farofinance.app/docs/quickstart
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.farofinance.app/docs/quickstart\nsources:\n- https://www.farofinance.app/docs/quickstart\ndescription: Authentication methods as documented on the Faro Quickstart page.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it on every request as a bearer token: Authorization: Bearer <your-key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at /signup with your email and location. Faro issues your API key immediately in the browser (shown once), so copy and\n    store it right away.\ndocs: https://www.farofinance.app/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/farofinance-app/authentication/farofinance-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Fraud Prevention
- Verification
- Payments
---
