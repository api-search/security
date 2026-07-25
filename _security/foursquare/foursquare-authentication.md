---
api_key_in: []
api_specs:
- filename: foursquare-ask-api-openapi.yml
  format: yaml
  label: Foursquare Ask API
  slug: foursquare-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-ask-api-openapi.yml
- filename: foursquare-autocomplete-api-openapi.yml
  format: yaml
  label: Foursquare Autocomplete API
  slug: foursquare-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-autocomplete-api-openapi.yml
- filename: foursquare-details-api-openapi.yml
  format: yaml
  label: Foursquare Details API
  slug: foursquare-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-details-api-openapi.yml
- filename: foursquare-geotagging-api-openapi.yml
  format: yaml
  label: Foursquare Geotagging API
  slug: foursquare-geotagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-geotagging-api-openapi.yml
- filename: foursquare-match-api-openapi.yml
  format: yaml
  label: Foursquare Match API
  slug: foursquare-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-match-api-openapi.yml
- filename: foursquare-photos-api-openapi.yml
  format: yaml
  label: Foursquare Photos API
  slug: foursquare-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-photos-api-openapi.yml
- filename: foursquare-search-api-openapi.yml
  format: yaml
  label: Foursquare Search API
  slug: foursquare-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-search-api-openapi.yml
- filename: foursquare-tips-api-openapi.yml
  format: yaml
  label: Foursquare Tips API
  slug: foursquare-tips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/openapi/foursquare-tips-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Foursquare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Foursquare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Foursquare
provider_slug: foursquare
scheme_count: 1
schemes:
- description: 'Service Key passed as a Bearer token in the Authorization header ("Authorization: Bearer <service-key>").'
  name: serviceKey
  scheme: bearer
  sources:
  - openapi/foursquare-places-openapi.yml
  type: http
slug: foursquare-authentication
source_filename: foursquare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/foursquare-places-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: serviceKey\n  type: http\n  scheme: bearer\n  description: 'Service Key passed as a Bearer token in the Authorization header (\"Authorization:\n    Bearer <service-key>\").'\n  sources:\n  - openapi/foursquare-places-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/authentication/foursquare-authentication.yml
summary_line: http · 1 scheme
tags:
- Restaurant
- Locations
- Places
- Geocoding
- Recommendations
- Reviews
- Movement
---
