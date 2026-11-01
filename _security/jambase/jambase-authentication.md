---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jambase-artists-api-openapi.yml
  format: yaml
  label: JamBase Artists API
  slug: jambase-artists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-artists-api-openapi.yml
- filename: jambase-events-api-openapi.yml
  format: yaml
  label: JamBase Events API
  slug: jambase-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-events-api-openapi.yml
- filename: jambase-genres-api-openapi.yml
  format: yaml
  label: JamBase Genres API
  slug: jambase-genres-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-genres-api-openapi.yml
- filename: jambase-geographies-api-openapi.yml
  format: yaml
  label: JamBase Geographies API
  slug: jambase-geographies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-geographies-api-openapi.yml
- filename: jambase-lookups-api-openapi.yml
  format: yaml
  label: JamBase Lookups API
  slug: jambase-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-lookups-api-openapi.yml
- filename: jambase-streams-api-openapi.yml
  format: yaml
  label: JamBase Streams API
  slug: jambase-streams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-streams-api-openapi.yml
- filename: jambase-venues-api-openapi.yml
  format: yaml
  label: JamBase Venues API
  slug: jambase-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-venues-api-openapi.yml
- filename: jambase-festivalseries-api-openapi.yml
  format: yaml
  label: JamBase Festival Series API
  slug: jambase-festivalseries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-festivalseries-api-openapi.yml
- filename: jambase-usage-api-openapi.yml
  format: yaml
  label: JamBase Usage API
  slug: jambase-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jambase/openapi/jambase-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
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
source_yaml_url: https://artifacts.apis.io/jambase/authentication/jambase-authentication.yml
summary_line: http · 1 scheme
tags:
- Artists
- Concerts
- Event
- Festivals
- Live Music
- Music
- Setlists
- Ticketing
- Tours
- Venues
---
