---
anonymous_access: false
api_key_in: []
api_specs:
- filename: unwired-labs-balance-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) BALANCE API
  slug: unwired-labs-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-balance-api-openapi.yml
- filename: unwired-labs-geolocation-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) GEOLOCATION API
  slug: unwired-labs-geolocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-geolocation-api-openapi.yml
- filename: unwired-labs-reverse-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) REVERSE API
  slug: unwired-labs-reverse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-reverse-api-openapi.yml
- filename: unwired-labs-search-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) SEARCH API
  slug: unwired-labs-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-search-api-openapi.yml
- filename: unwired-labs-timezone-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) Timezone API
  slug: unwired-labs-timezone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-timezone-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Unwired Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unwired Labs (incl. OpenCelliD) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Unwired Labs (incl. OpenCelliD)
provider_slug: unwired-labs
scheme_count: 1
schemes:
- evidence: Every request to Unwired Labs' APIs must be authenticated with a scoped access token.
  how_to_obtain: Generate access tokens on your User Dashboard; create a separate token for each application.
  location: body
  name: token
  type: apiKey
slug: unwired-labs-authentication
source_filename: unwired-labs-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.unwiredlabs.com/docs/authentication
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.unwiredlabs.com/docs/authentication\nsources:\n- https://docs.unwiredlabs.com/docs/authentication\n- https://docs.unwiredlabs.com/docs/geolocation/getting-started\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: token\n  evidence: Every request to Unwired Labs' APIs must be authenticated with a scoped access token.\n  location: body\n  how_to_obtain: Generate access tokens on your User Dashboard; create a separate token for each application.\ndocs: https://docs.unwiredlabs.com/docs/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/unwired-labs/authentication/unwired-labs-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Location API
- Geolocation
- Mapping
- OpenCelliD
---
