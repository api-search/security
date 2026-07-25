---
api_key_in:
- header
api_specs:
- filename: inaturalist-annotations-api-openapi.yml
  format: yaml
  label: iNaturalist Annotations API
  slug: inaturalist-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-annotations-api-openapi.yml
- filename: inaturalist-comments-api-openapi.yml
  format: yaml
  label: iNaturalist Comments API
  slug: inaturalist-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-comments-api-openapi.yml
- filename: inaturalist-controlled-terms-api-openapi.yml
  format: yaml
  label: iNaturalist Controlled Terms API
  slug: inaturalist-controlled-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-controlled-terms-api-openapi.yml
- filename: inaturalist-flags-api-openapi.yml
  format: yaml
  label: iNaturalist Flags API
  slug: inaturalist-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-flags-api-openapi.yml
- filename: inaturalist-identifications-api-openapi.yml
  format: yaml
  label: iNaturalist Identifications API
  slug: inaturalist-identifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-identifications-api-openapi.yml
- filename: inaturalist-messages-api-openapi.yml
  format: yaml
  label: iNaturalist Messages API
  slug: inaturalist-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-messages-api-openapi.yml
- filename: inaturalist-observation-field-values-api-openapi.yml
  format: yaml
  label: iNaturalist Observation Field Values API
  slug: inaturalist-observation-field-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-observation-field-values-api-openapi.yml
- filename: inaturalist-observation-photos-api-openapi.yml
  format: yaml
  label: iNaturalist Observation Photos API
  slug: inaturalist-observation-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-observation-photos-api-openapi.yml
- filename: inaturalist-observation-tiles-api-openapi.yml
  format: yaml
  label: iNaturalist Observation Tiles API
  slug: inaturalist-observation-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-observation-tiles-api-openapi.yml
- filename: inaturalist-observations-api-openapi.yml
  format: yaml
  label: iNaturalist Observations API
  slug: inaturalist-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-observations-api-openapi.yml
- filename: inaturalist-photos-api-openapi.yml
  format: yaml
  label: iNaturalist Photos API
  slug: inaturalist-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-photos-api-openapi.yml
- filename: inaturalist-places-api-openapi.yml
  format: yaml
  label: iNaturalist Places API
  slug: inaturalist-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-places-api-openapi.yml
- filename: inaturalist-polygon-tiles-api-openapi.yml
  format: yaml
  label: iNaturalist Polygon Tiles API
  slug: inaturalist-polygon-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-polygon-tiles-api-openapi.yml
- filename: inaturalist-posts-api-openapi.yml
  format: yaml
  label: iNaturalist Posts API
  slug: inaturalist-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-posts-api-openapi.yml
- filename: inaturalist-project-observations-api-openapi.yml
  format: yaml
  label: iNaturalist Project Observations API
  slug: inaturalist-project-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-project-observations-api-openapi.yml
- filename: inaturalist-projects-api-openapi.yml
  format: yaml
  label: iNaturalist Projects API
  slug: inaturalist-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-projects-api-openapi.yml
- filename: inaturalist-search-api-openapi.yml
  format: yaml
  label: iNaturalist Search API
  slug: inaturalist-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-search-api-openapi.yml
- filename: inaturalist-taxa-api-openapi.yml
  format: yaml
  label: iNaturalist Taxa API
  slug: inaturalist-taxa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-taxa-api-openapi.yml
- filename: inaturalist-users-api-openapi.yml
  format: yaml
  label: iNaturalist Users API
  slug: inaturalist-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-users-api-openapi.yml
- filename: inaturalist-utfgrid-api-openapi.yml
  format: yaml
  label: iNaturalist UTFGrid API
  slug: inaturalist-utfgrid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/openapi/inaturalist-utfgrid-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Inaturalist Authentication
name_suffix: Authentication
oauth_flows: []
overview: iNaturalist secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: iNaturalist
provider_slug: inaturalist
scheme_count: 1
schemes:
- in: header
  name: api_token
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
slug: inaturalist-authentication
source_filename: inaturalist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/authentication/inaturalist-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Biodiversity
- Nature
- Citizen Science
- Wildlife
- Observations
- Taxa
- Ecology
---
