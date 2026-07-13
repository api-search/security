---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: JamBase Data API
  slug: jambase-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/openapi/openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Jambase Authentication
name_suffix: Authentication
oauth_flows: []
overview: JamBase secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JamBase
provider_slug: jambase
scheme_count: 1
schemes:
- description: API key as Bearer token. Get your key from your account dashboard.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: jambase-authentication
source_filename: jambase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key as Bearer token. Get your key from your account dashboard.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jambase/refs/heads/main/authentication/jambase-authentication.yml
summary_line: http · 1 scheme
tags:
- Artists
- Concerts
- Events
- Festivals
- Live Music
- Music
- Setlists
- Tickets
- Tours
- Venues
---
