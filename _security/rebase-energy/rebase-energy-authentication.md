---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rebase-energy-account-api-openapi.yml
  format: yaml
  label: Rebase Energy Account API
  slug: rebase-energy-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-account-api-openapi.yml
- filename: rebase-energy-data-api-openapi.yml
  format: yaml
  label: Rebase Energy Data API
  slug: rebase-energy-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-data-api-openapi.yml
- filename: rebase-energy-describe-api-openapi.yml
  format: yaml
  label: Rebase Energy Describe API
  slug: rebase-energy-describe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-describe-api-openapi.yml
- filename: rebase-energy-discover-api-openapi.yml
  format: yaml
  label: Rebase Energy Discover API
  slug: rebase-energy-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-discover-api-openapi.yml
- filename: rebase-energy-expectations-api-openapi.yml
  format: yaml
  label: Rebase Energy Expectations API
  slug: rebase-energy-expectations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-expectations-api-openapi.yml
- filename: rebase-energy-integration-api-openapi.yml
  format: yaml
  label: Rebase Energy Integration API
  slug: rebase-energy-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-integration-api-openapi.yml
- filename: rebase-energy-misc-api-openapi.yml
  format: yaml
  label: Rebase Energy Misc API
  slug: rebase-energy-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-misc-api-openapi.yml
- filename: rebase-energy-model-api-openapi.yml
  format: yaml
  label: Rebase Energy Model API
  slug: rebase-energy-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-model-api-openapi.yml
- filename: rebase-energy-point-api-openapi.yml
  format: yaml
  label: Rebase Energy Point API
  slug: rebase-energy-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-point-api-openapi.yml
- filename: rebase-energy-read-api-openapi.yml
  format: yaml
  label: Rebase Energy Read API
  slug: rebase-energy-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-read-api-openapi.yml
- filename: rebase-energy-site-api-openapi.yml
  format: yaml
  label: Rebase Energy Site API
  slug: rebase-energy-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-site-api-openapi.yml
- filename: rebase-energy-usage-api-openapi.yml
  format: yaml
  label: Rebase Energy Usage API
  slug: rebase-energy-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-usage-api-openapi.yml
- filename: rebase-energy-user-api-openapi.yml
  format: yaml
  label: Rebase Energy User API
  slug: rebase-energy-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rebase-energy/openapi/rebase-energy-user-api-openapi.yml
auth_types: []
description: Authentication schemes for Rebase Grid API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Rebase Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rebase Energy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Rebase Energy
provider_slug: rebase-energy
scheme_count: 1
schemes:
- evidence: Send the key in the X-API-Key header, or as the api_key query parameter.
  header: X-API-Key
  how_to_obtain: Request one with the key request form.
  location: header
  name: API Key
  type: apiKey
slug: rebase-energy-authentication
source_filename: rebase-energy-authentication.yml
source_heading: Authentication Profile
source_url: https://grid.rebase.energy/docs/v1/guides/authentication/
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://grid.rebase.energy/docs/v1/guides/authentication/\nsources:\n- https://grid.rebase.energy/docs/v1/guides/authentication/\n- https://grid.rebase.energy/docs/v1/guides/authentication/#get-a-key\n- https://grid.rebase.energy/docs/v1/guides/authentication/\n- https://grid.rebase.energy/docs/v1/guides/open-access/\ndescription: Authentication schemes for Rebase Grid API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Send the key in the X-API-Key header, or as the api_key query parameter.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Request one with the key request form.\ndocs: https://grid.rebase.energy/docs/v1/guides/authentication/\n"
source_yaml_url: https://artifacts.apis.io/rebase-energy/authentication/rebase-energy-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Electricity
- Data
- Open Source
---
