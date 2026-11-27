---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mediaframe-me-actors-api-openapi.yml
  format: yaml
  label: MediaFrame Actors API
  slug: mediaframe-me-actors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-actors-api-openapi.yml
- filename: mediaframe-me-coverage-api-openapi.yml
  format: yaml
  label: MediaFrame Coverage API
  slug: mediaframe-me-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-coverage-api-openapi.yml
- filename: mediaframe-me-datasets-api-openapi.yml
  format: yaml
  label: MediaFrame Datasets API
  slug: mediaframe-me-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-datasets-api-openapi.yml
- filename: mediaframe-me-editorial-api-openapi.yml
  format: yaml
  label: MediaFrame Editorial API
  slug: mediaframe-me-editorial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-editorial-api-openapi.yml
- filename: mediaframe-me-flow-api-openapi.yml
  format: yaml
  label: MediaFrame Flow API
  slug: mediaframe-me-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-flow-api-openapi.yml
- filename: mediaframe-me-framers-api-openapi.yml
  format: yaml
  label: MediaFrame Framers API
  slug: mediaframe-me-framers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-framers-api-openapi.yml
- filename: mediaframe-me-framing-api-openapi.yml
  format: yaml
  label: MediaFrame Framing API
  slug: mediaframe-me-framing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-framing-api-openapi.yml
- filename: mediaframe-me-outlet-framing-api-openapi.yml
  format: yaml
  label: MediaFrame Outlet Framing API
  slug: mediaframe-me-outlet-framing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-outlet-framing-api-openapi.yml
- filename: mediaframe-me-people-api-openapi.yml
  format: yaml
  label: MediaFrame People API
  slug: mediaframe-me-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-people-api-openapi.yml
- filename: mediaframe-me-pieces-api-openapi.yml
  format: yaml
  label: MediaFrame Pieces API
  slug: mediaframe-me-pieces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-pieces-api-openapi.yml
- filename: mediaframe-me-propagation-api-openapi.yml
  format: yaml
  label: MediaFrame Propagation API
  slug: mediaframe-me-propagation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-propagation-api-openapi.yml
- filename: mediaframe-me-pulse-api-openapi.yml
  format: yaml
  label: MediaFrame Pulse API
  slug: mediaframe-me-pulse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-pulse-api-openapi.yml
- filename: mediaframe-me-rhetoric-api-openapi.yml
  format: yaml
  label: MediaFrame Rhetoric API
  slug: mediaframe-me-rhetoric-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-rhetoric-api-openapi.yml
- filename: mediaframe-me-series-api-openapi.yml
  format: yaml
  label: MediaFrame Series API
  slug: mediaframe-me-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-series-api-openapi.yml
- filename: mediaframe-me-signals-api-openapi.yml
  format: yaml
  label: MediaFrame Signals API
  slug: mediaframe-me-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-signals-api-openapi.yml
- filename: mediaframe-me-snapshot-api-openapi.yml
  format: yaml
  label: MediaFrame Snapshot API
  slug: mediaframe-me-snapshot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-snapshot-api-openapi.yml
- filename: mediaframe-me-trajectories-api-openapi.yml
  format: yaml
  label: MediaFrame Trajectories API
  slug: mediaframe-me-trajectories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mediaframe-me/openapi/mediaframe-me-trajectories-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MediaFrame Authentication
name_suffix: Authentication
oauth_flows: []
overview: MediaFrame secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MediaFrame
provider_slug: mediaframe-me
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/mediaframe-me-openapi.json
  type: apiKey
slug: mediaframe-me-authentication
source_filename: mediaframe-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mediaframe-me-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/mediaframe-me-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mediaframe-me/authentication/mediaframe-me-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Media Intelligence
- Narrative Analysis
- Influence Mapping
- Early Signal Detection
- Public Discourse
- Risk Analysis
---
