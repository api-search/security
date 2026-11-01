---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meld-headless-api-openapi.yml
  format: yaml
  label: Meld.io Headless API
  slug: meld-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meld/openapi/meld-headless-api-openapi.yml
- filename: meld-retail-ramp-api-openapi.yml
  format: yaml
  label: Meld.io Retail Ramp API
  slug: meld-retail-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meld/openapi/meld-retail-ramp-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meld.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Meld.io
provider_slug: meld
scheme_count: 1
schemes:
- evidence: Authentication uses an API key passed in the Authorization header with a BASIC prefix.
  header: Authorization
  how_to_obtain: Obtain API key from Meld dashboard (Developer → API Keys) and include as BASIC <key> in the Authorization header.
  location: header
  name: Authorization
  type: apiKey
slug: meld-authentication
source_filename: meld-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.meld.io/docs/stablecoins/sandbox-guide/test
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.meld.io/docs/stablecoins/sandbox-guide/test\nsources:\n- https://docs.meld.io/docs/stablecoins/sandbox-guide/test\n- https://docs.meld.io/docs/bank-linking/creating-connections/create-a-connect-token\n- https://docs.meld.io/docs/meld-api/getting-started\n- https://docs.meld.io/docs/stablecoins/white-label-api-integration/whitelabel-quickstart\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: Authentication uses an API key passed in the Authorization header with a BASIC prefix.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain API key from Meld dashboard (Developer → API Keys) and include as BASIC <key> in the Authorization header.\ndocs: https://docs.meld.io/docs/stablecoins/sandbox-guide/test\n"
source_yaml_url: https://artifacts.apis.io/meld/authentication/meld-authentication.yml
summary_line: 1 scheme
tags:
- Data Integration
- FinTech
- API Platform
- Stablecoin
- Digital Assets
- Enterprise
---
