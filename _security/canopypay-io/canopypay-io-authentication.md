---
anonymous_access: false
api_key_in: []
api_specs:
- filename: canopypay-io-openapi-generated.yml
  format: yaml
  label: canopypay-io API
  slug: canopypay-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/canopypay-io/openapi/_ae-authored/canopypay-io-openapi-generated.yml
auth_types: []
description: Authentication schemes for Canopy Pay API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Canopypay Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: canopypay-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: canopypay-io
provider_slug: canopypay-io
scheme_count: 1
schemes:
- evidence: 'Send it as an Authorization: Bearer token on every /api/v1/* request.'
  header: Authorization
  how_to_obtain: Get a secret key from the Canopy dashboard (see Quickstart page).
  location: header
  name: Secret Key
  type: http-bearer
slug: canopypay-io-authentication
source_filename: canopypay-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.canopypay.io/guides/credentials
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.canopypay.io/guides/credentials\nsources:\n- https://www.canopypay.io/guides/credentials\n- https://www.canopypay.io/quickstart\ndescription: Authentication schemes for Canopy Pay API\nschemes:\n- type: http-bearer\n  name: Secret Key\n  evidence: 'Send it as an Authorization: Bearer token on every /api/v1/* request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Get a secret key from the Canopy dashboard (see Quickstart page).\ndocs: https://www.canopypay.io/guides/credentials\n"
source_yaml_url: https://artifacts.apis.io/canopypay-io/authentication/canopypay-io-authentication.yml
summary_line: 1 scheme
tags:
- FinTech
- Crypto
- Payments
- API
- Deposit
---
