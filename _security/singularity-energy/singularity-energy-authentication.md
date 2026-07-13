---
api_key_in:
- header
api_specs:
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Carbon Intensity API
  slug: carbon-intensity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Forecasts API
  slug: forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Generation & Event Data API
  slug: generation-event-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
- filename: singularity-energy-openapi.yml
  format: yaml
  label: Singularity Regions API
  slug: regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/openapi/singularity-energy-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Singularity Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Singularity secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Singularity
provider_slug: singularity-energy
scheme_count: 1
schemes:
- description: API key passed in the X-Api-Key request header. A User-Agent header is also required.
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/singularity-energy-openapi.yml
  type: apiKey
slug: singularity-energy-authentication
source_filename: singularity-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/singularity-energy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: API key passed in the X-Api-Key request header. A User-Agent header is also required.\n  sources:\n  - openapi/singularity-energy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singularity-energy/refs/heads/main/authentication/singularity-energy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Carbon Emissions
- Grid
- Sustainability
- Carbon Intensity
---
