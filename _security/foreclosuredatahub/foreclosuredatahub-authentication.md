---
anonymous_access: false
api_key_in: []
api_specs:
- filename: foreclosuredatahub-openapi-generated.yml
  format: yaml
  label: Foreclosure Data Hub API API
  slug: foreclosuredatahub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foreclosuredatahub/openapi/_ae-authored/foreclosuredatahub-openapi-generated.yml
auth_types: []
description: Foreclosure Data Hub uses an API key passed in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Foreclosure Data Hub API Authentication
name_suffix: Authentication
oauth_flows: []
overview: Foreclosure Data Hub API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Foreclosure Data Hub API
provider_slug: foreclosuredatahub
scheme_count: 1
schemes:
- evidence: Authenticate requests with your API key. Pass your API key in the x-api-key header on every request.
  header: x-api-key
  how_to_obtain: Generate and manage retail keys in API settings.
  location: header
  name: API Key
  type: apiKey
slug: foreclosuredatahub-authentication
source_filename: foreclosuredatahub-authentication.yml
source_heading: Authentication Profile
source_url: https://www.foreclosuredatahub.com/docs/authentication
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.foreclosuredatahub.com/docs/authentication\nsources:\n- https://www.foreclosuredatahub.com/docs/authentication\n- https://www.foreclosuredatahub.com/signin?next=%2Fdashboard%2Fapi%2Fkeys\n- https://www.foreclosuredatahub.com/docs/quickstart\ndescription: Foreclosure Data Hub uses an API key passed in a request header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Authenticate requests with your API key. Pass your API key in the x-api-key header on every request.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate and manage retail keys in API settings.\ndocs: https://www.foreclosuredatahub.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/foreclosuredatahub/authentication/foreclosuredatahub-authentication.yml
summary_line: 1 scheme
tags:
- Real Estate
- Data
- Property
- Finance
---
