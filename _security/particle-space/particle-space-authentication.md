---
api_key_in: []
api_specs:
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Property Records API
  slug: property-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Address Search API
  slug: address-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Valuations API
  slug: valuations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Comparables API
  slug: comps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
- filename: particle-space-openapi.yml
  format: yaml
  label: Particle Space Listings API
  slug: listings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/openapi/particle-space-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Particle Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Particle Space secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Particle Space
provider_slug: particle-space
scheme_count: 1
schemes:
- description: Authenticate with a Particle Space secret API key (PS_SECRET_KEY) as a bearer token. The key determines live versus test mode. Confirm the exact authentication scheme and header in the live API reference.
  name: SecretKeyAuth
  scheme: bearer
  sources:
  - openapi/particle-space-openapi.yml
  type: http
slug: particle-space-authentication
source_filename: particle-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/particle-space-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: SecretKeyAuth\n  type: http\n  scheme: bearer\n  description: Authenticate with a Particle Space secret API key (PS_SECRET_KEY) as a bearer\n    token. The key determines live versus test mode. Confirm the exact authentication scheme\n    and header in the live API reference.\n  sources:\n  - openapi/particle-space-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/particle-space/refs/heads/main/authentication/particle-space-authentication.yml
summary_line: http · 1 scheme
tags:
- Real Estate
- Property Data
- PropTech
- Listings
- Valuations
---
