---
api_key_in:
- header
api_specs:
- filename: spacex-capsules-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Capsules API
  slug: spacex-capsules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-capsules-api-openapi.yml
- filename: spacex-company-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Company API
  slug: spacex-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-company-api-openapi.yml
- filename: spacex-cores-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Cores API
  slug: spacex-cores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-cores-api-openapi.yml
- filename: spacex-crew-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Crew API
  slug: spacex-crew-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-crew-api-openapi.yml
- filename: spacex-dragons-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Dragons API
  slug: spacex-dragons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-dragons-api-openapi.yml
- filename: spacex-history-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) History API
  slug: spacex-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-history-api-openapi.yml
- filename: spacex-landpads-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Landpads API
  slug: spacex-landpads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-landpads-api-openapi.yml
- filename: spacex-launches-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Launches API
  slug: spacex-launches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-launches-api-openapi.yml
- filename: spacex-launchpads-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Launchpads API
  slug: spacex-launchpads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-launchpads-api-openapi.yml
- filename: spacex-payloads-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Payloads API
  slug: spacex-payloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-payloads-api-openapi.yml
- filename: spacex-roadster-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Roadster API
  slug: spacex-roadster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-roadster-api-openapi.yml
- filename: spacex-rockets-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Rockets API
  slug: spacex-rockets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-rockets-api-openapi.yml
- filename: spacex-ships-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Ships API
  slug: spacex-ships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-ships-api-openapi.yml
- filename: spacex-starlink-api-openapi.yml
  format: yaml
  label: SpaceX (Community API) Starlink API
  slug: spacex-starlink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-starlink-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spacex Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpaceX (Community API) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpaceX (Community API)
provider_slug: spacex
scheme_count: 1
schemes:
- description: 'Admin API key for destructive (create/update/delete) operations.

    Not required for any read endpoint.'
  in: header
  name: SpacexKey
  parameter: spacex-key
  sources:
  - openapi/spacex-rest-api-openapi.yml
  type: apiKey
slug: spacex-authentication
source_filename: spacex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spacex-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SpacexKey\n  type: apiKey\n  in: header\n  parameter: spacex-key\n  description: |-\n    Admin API key for destructive (create/update/delete) operations.\n    Not required for any read endpoint.\n  sources:\n  - openapi/spacex-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/authentication/spacex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Space
- Launch
- Satellites
- Starlink
- Falcon 9
- Falcon Heavy
- Dragon
- Rockets
- Open-Source
- Community
- REST
- GraphQL
- Open Data
---
