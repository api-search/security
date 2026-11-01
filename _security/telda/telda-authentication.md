---
anonymous_access: false
api_key_in: []
api_specs:
- filename: telda-openapi-generated.yml
  format: yaml
  label: Telda API
  slug: telda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/telda/openapi/_ae-authored/telda-openapi-generated.yml
auth_types: []
description: Authentication schemes for Telda as described on the Lever OAuth documentation page.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Telda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telda declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Telda
provider_slug: telda
scheme_count: 1
schemes:
- authorize_url: https://sandbox-lever.auth0.com/authorize
  evidence: As of 2020, all Lever integrations are authenticated using OAuth.
  flows:
  - authorization_code
  how_to_obtain: Register your app/integration on Lever's Auth server to receive a client ID and client secret.
  name: OAuth 2.0
  type: oauth2
slug: telda-authentication
source_filename: telda-authentication.yml
source_heading: Authentication Profile
source_url: https://hire.lever.co/developer/oauth
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hire.lever.co/developer/oauth\nsources:\n- https://hire.lever.co/developer/oauth\ndescription: Authentication schemes for Telda as described on the Lever OAuth documentation page.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: As of 2020, all Lever integrations are authenticated using OAuth.\n  flows:\n  - authorization_code\n  authorize_url: https://sandbox-lever.auth0.com/authorize\n  how_to_obtain: Register your app/integration on Lever's Auth server to receive a client ID and client secret.\ndocs: https://hire.lever.co/developer/oauth\n"
source_yaml_url: https://artifacts.apis.io/telda/authentication/telda-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Fintech
- Payments
- MobileApp
- DigitalBanking
---
