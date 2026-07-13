---
api_key_in:
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: ETH Library Discovery API
  slug: discovery
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library ETHorama API
  slug: ethorama
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library Geo Information API
  slug: geo
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library Persons API
  slug: persons
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Zurich Research Collection API
  slug: research-collection
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
- filename: openapi.yaml
  format: yaml
  label: ETH Library Vector API
  slug: vector
  spec_type: OpenAPI
  url: https://eth-library.github.io/opendata-apis/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Eth Zurich Authentication
name_suffix: Authentication
oauth_flows: []
overview: ETH Zurich – Swiss Federal Institute of Technology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ETH Zurich – Swiss Federal Institute of Technology
provider_slug: eth-zurich
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/eth-zurich-discovery.yaml
  - openapi/eth-zurich-ethorama.yaml
  - openapi/eth-zurich-geo.yaml
  - openapi/eth-zurich-persons.yaml
  - openapi/eth-zurich-research-collection-v1.yaml
  - openapi/eth-zurich-research-collection-v2.yaml
  - openapi/eth-zurich-vector.yaml
  type: apiKey
slug: eth-zurich-authentication
source_filename: eth-zurich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eth-zurich-discovery.yaml, openapi/eth-zurich-ethorama.yaml, openapi/eth-zurich-geo.yaml,\n  openapi/eth-zurich-persons.yaml, openapi/eth-zurich-research-collection-v1.yaml, openapi/eth-zurich-research-collection-v2.yaml,\n  openapi/eth-zurich-vector.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/eth-zurich-discovery.yaml\n  - openapi/eth-zurich-ethorama.yaml\n  - openapi/eth-zurich-geo.yaml\n  - openapi/eth-zurich-persons.yaml\n  - openapi/eth-zurich-research-collection-v1.yaml\n  - openapi/eth-zurich-research-collection-v2.yaml\n  - openapi/eth-zurich-vector.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eth-zurich/refs/heads/main/authentication/eth-zurich-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Data
- Switzerland
---
