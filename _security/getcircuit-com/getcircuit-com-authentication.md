---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getcircuit-com-couriers-api-openapi.yml
  format: yaml
  label: Circuit Couriers API
  slug: getcircuit-com-couriers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-couriers-api-openapi.yml
- filename: getcircuit-com-depots-api-openapi.yml
  format: yaml
  label: Circuit Depots API
  slug: getcircuit-com-depots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-depots-api-openapi.yml
- filename: getcircuit-com-drivers-api-openapi.yml
  format: yaml
  label: Circuit Drivers API
  slug: getcircuit-com-drivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-drivers-api-openapi.yml
- filename: getcircuit-com-live-plans-api-openapi.yml
  format: yaml
  label: Circuit Live Plans API
  slug: getcircuit-com-live-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-live-plans-api-openapi.yml
- filename: getcircuit-com-live-stops-api-openapi.yml
  format: yaml
  label: Circuit Live Stops API
  slug: getcircuit-com-live-stops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-live-stops-api-openapi.yml
- filename: getcircuit-com-members-api-openapi.yml
  format: yaml
  label: Circuit Members API
  slug: getcircuit-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-members-api-openapi.yml
- filename: getcircuit-com-operations-api-openapi.yml
  format: yaml
  label: Circuit Operations API
  slug: getcircuit-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-operations-api-openapi.yml
- filename: getcircuit-com-orders-api-openapi.yml
  format: yaml
  label: Circuit Orders API
  slug: getcircuit-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-orders-api-openapi.yml
- filename: getcircuit-com-pickup-locations-api-openapi.yml
  format: yaml
  label: Circuit Pickup Locations API
  slug: getcircuit-com-pickup-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-pickup-locations-api-openapi.yml
- filename: getcircuit-com-plans-api-openapi.yml
  format: yaml
  label: Circuit Plans API
  slug: getcircuit-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-plans-api-openapi.yml
- filename: getcircuit-com-routes-api-openapi.yml
  format: yaml
  label: Circuit Routes API
  slug: getcircuit-com-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-routes-api-openapi.yml
- filename: getcircuit-com-stops-api-openapi.yml
  format: yaml
  label: Circuit Stops API
  slug: getcircuit-com-stops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-stops-api-openapi.yml
- filename: getcircuit-com-team-api-openapi.yml
  format: yaml
  label: Circuit Team API
  slug: getcircuit-com-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-team-api-openapi.yml
- filename: getcircuit-com-unassigned-stops-api-openapi.yml
  format: yaml
  label: Circuit Unassigned Stops API
  slug: getcircuit-com-unassigned-stops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getcircuit-com/openapi/getcircuit-com-unassigned-stops-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Getcircuit Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circuit secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Circuit
provider_slug: getcircuit-com
scheme_count: 2
schemes:
- description: Pass the API key directly as the token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi-connect-v1.json
  type: http
- description: Use the API key as the username and leave the password empty.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/openapi-connect-v1.json
  - openapi/openapi-v0.2b.json
  - openapi/openapi-v1.json
  type: http
slug: getcircuit-com-authentication
source_filename: getcircuit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/openapi-connect-v1.json, openapi/openapi-v0.2b.json, openapi/openapi-v1.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Pass the API key directly as the token.\n  sources:\n  - openapi/openapi-connect-v1.json\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Use the API key as the username and leave the password empty.\n  sources:\n  - openapi/openapi-connect-v1.json\n  - openapi/openapi-v0.2b.json\n  - openapi/openapi-v1.json\n"
source_yaml_url: https://artifacts.apis.io/getcircuit-com/authentication/getcircuit-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Logistics
- Delivery
- API
- Platform
---
