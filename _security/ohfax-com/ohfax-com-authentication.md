---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ohfax-com-auth-api-openapi.yml
  format: yaml
  label: Oh Fax Auth API
  slug: ohfax-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-auth-api-openapi.yml
- filename: ohfax-com-balance-api-openapi.yml
  format: yaml
  label: Oh Fax Balance API
  slug: ohfax-com-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-balance-api-openapi.yml
- filename: ohfax-com-checkout-api-openapi.yml
  format: yaml
  label: Oh Fax Checkout API
  slug: ohfax-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-checkout-api-openapi.yml
- filename: ohfax-com-dev-api-openapi.yml
  format: yaml
  label: Oh Fax Dev API
  slug: ohfax-com-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-dev-api-openapi.yml
- filename: ohfax-com-faxes-api-openapi.yml
  format: yaml
  label: Oh Fax Faxes API
  slug: ohfax-com-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-faxes-api-openapi.yml
- filename: ohfax-com-health-api-openapi.yml
  format: yaml
  label: Oh Fax Health API
  slug: ohfax-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-health-api-openapi.yml
- filename: ohfax-com-pay-api-openapi.yml
  format: yaml
  label: Oh Fax Pay API
  slug: ohfax-com-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-pay-api-openapi.yml
- filename: ohfax-com-quotes-api-openapi.yml
  format: yaml
  label: Oh Fax Quotes API
  slug: ohfax-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ohfax-com/openapi/ohfax-com-quotes-api-openapi.yml
auth_types: []
description: Authentication for Oh Fax API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Oh Fax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oh Fax declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Oh Fax
provider_slug: ohfax-com
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer $OHFAX_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key in the Account page after Google sign‑in; the plaintext key (e.g., afx_live_…) is shown once.
  location: header
  name: Bearer token
  type: http-bearer
slug: ohfax-com-authentication
source_filename: ohfax-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ohfax.com/docs/quickstart
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ohfax.com/docs/quickstart\nsources:\n- https://ohfax.com/docs/quickstart\ndescription: Authentication for Oh Fax API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: '-H \"Authorization: Bearer $OHFAX_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Account page after Google sign‑in; the plaintext key (e.g., afx_live_…) is shown once.\ndocs: https://ohfax.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/ohfax-com/authentication/ohfax-com-authentication.yml
summary_line: 1 scheme
tags:
- Fax
- Payments
- Cloud
- Communications
---
