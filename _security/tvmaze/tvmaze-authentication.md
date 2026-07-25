---
api_key_in: []
api_specs:
- filename: tvmaze-auth-api-openapi.yml
  format: yaml
  label: TVmaze auth API
  slug: tvmaze-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-auth-api-openapi.yml
- filename: tvmaze-episodes-api-openapi.yml
  format: yaml
  label: TVmaze Episodes API
  slug: tvmaze-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-episodes-api-openapi.yml
- filename: tvmaze-followed-networks-api-openapi.yml
  format: yaml
  label: TVmaze followed networks API
  slug: tvmaze-followed-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-networks-api-openapi.yml
- filename: tvmaze-followed-people-api-openapi.yml
  format: yaml
  label: TVmaze followed people API
  slug: tvmaze-followed-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-people-api-openapi.yml
- filename: tvmaze-followed-shows-api-openapi.yml
  format: yaml
  label: TVmaze followed shows API
  slug: tvmaze-followed-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-shows-api-openapi.yml
- filename: tvmaze-followed-webchannels-api-openapi.yml
  format: yaml
  label: TVmaze followed webchannels API
  slug: tvmaze-followed-webchannels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-followed-webchannels-api-openapi.yml
- filename: tvmaze-marked-episodes-api-openapi.yml
  format: yaml
  label: TVmaze marked episodes API
  slug: tvmaze-marked-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-marked-episodes-api-openapi.yml
- filename: tvmaze-people-api-openapi.yml
  format: yaml
  label: TVmaze People API
  slug: tvmaze-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-people-api-openapi.yml
- filename: tvmaze-schedule-api-openapi.yml
  format: yaml
  label: TVmaze Schedule API
  slug: tvmaze-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-schedule-api-openapi.yml
- filename: tvmaze-scrobbling-api-openapi.yml
  format: yaml
  label: TVmaze scrobbling API
  slug: tvmaze-scrobbling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-scrobbling-api-openapi.yml
- filename: tvmaze-search-api-openapi.yml
  format: yaml
  label: TVmaze Search API
  slug: tvmaze-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-search-api-openapi.yml
- filename: tvmaze-seasons-api-openapi.yml
  format: yaml
  label: TVmaze Seasons API
  slug: tvmaze-seasons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-seasons-api-openapi.yml
- filename: tvmaze-shows-api-openapi.yml
  format: yaml
  label: TVmaze Shows API
  slug: tvmaze-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-shows-api-openapi.yml
- filename: tvmaze-tagged-shows-api-openapi.yml
  format: yaml
  label: TVmaze tagged shows API
  slug: tvmaze-tagged-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-tagged-shows-api-openapi.yml
- filename: tvmaze-updates-api-openapi.yml
  format: yaml
  label: TVmaze Updates API
  slug: tvmaze-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-updates-api-openapi.yml
- filename: tvmaze-voted-episodes-api-openapi.yml
  format: yaml
  label: TVmaze voted episodes API
  slug: tvmaze-voted-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-voted-episodes-api-openapi.yml
- filename: tvmaze-voted-shows-api-openapi.yml
  format: yaml
  label: TVmaze voted shows API
  slug: tvmaze-voted-shows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/openapi/tvmaze-voted-shows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tvmaze Authentication
name_suffix: Authentication
oauth_flows: []
overview: TVmaze secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TVmaze
provider_slug: tvmaze
scheme_count: 1
schemes:
- name: usertoken
  scheme: basic
  sources:
  - openapi/tvmaze-premium-openapi.yml
  type: http
slug: tvmaze-authentication
source_filename: tvmaze-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tvmaze-premium-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: usertoken\n  type: http\n  scheme: basic\n  sources:\n  - openapi/tvmaze-premium-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvmaze/refs/heads/main/authentication/tvmaze-authentication.yml
summary_line: http · 1 scheme
tags:
- Video
- Television
- Streaming
- Schedule
- Metadata
- Entertainment
- Public APIs
---
