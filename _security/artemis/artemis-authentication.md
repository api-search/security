---
api_key_in:
- query
api_specs:
- filename: artemis-apod-api-openapi.yml
  format: yaml
  label: Artemis APOD API
  slug: artemis-apod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-apod-api-openapi.yml
- filename: artemis-donki-api-openapi.yml
  format: yaml
  label: Artemis DONKI API
  slug: artemis-donki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-donki-api-openapi.yml
- filename: artemis-epic-api-openapi.yml
  format: yaml
  label: Artemis EPIC API
  slug: artemis-epic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-epic-api-openapi.yml
- filename: artemis-images-api-openapi.yml
  format: yaml
  label: Artemis Images API
  slug: artemis-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-images-api-openapi.yml
- filename: artemis-neows-api-openapi.yml
  format: yaml
  label: Artemis NeoWs API
  slug: artemis-neows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/openapi/artemis-neows-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Artemis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artemis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Artemis
provider_slug: artemis
scheme_count: 1
schemes:
- description: NASA api_key query parameter. Use DEMO_KEY for low-volume testing.
  in: query
  name: NasaApiKey
  parameter: api_key
  sources:
  - openapi/artemis-openapi.yml
  type: apiKey
slug: artemis-authentication
source_filename: artemis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/artemis-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: NasaApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: NASA api_key query parameter. Use DEMO_KEY for low-volume testing.\n  sources:\n  - openapi/artemis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artemis/refs/heads/main/authentication/artemis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Exploration
- Lunar
- Moon
- NASA
- Space
- Government
---
