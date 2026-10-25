---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fleetsu-accounts-api-openapi.yml
  format: yaml
  label: Fleetsu Accounts API
  slug: fleetsu-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-accounts-api-openapi.yml
- filename: fleetsu-assets-api-openapi.yml
  format: yaml
  label: Fleetsu Assets API
  slug: fleetsu-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-assets-api-openapi.yml
- filename: fleetsu-devices-api-openapi.yml
  format: yaml
  label: Fleetsu Devices API
  slug: fleetsu-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-devices-api-openapi.yml
- filename: fleetsu-driver-api-openapi.yml
  format: yaml
  label: Fleetsu Driver API
  slug: fleetsu-driver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-driver-api-openapi.yml
- filename: fleetsu-events-api-openapi.yml
  format: yaml
  label: Fleetsu Events API
  slug: fleetsu-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-events-api-openapi.yml
- filename: fleetsu-faults-api-openapi.yml
  format: yaml
  label: Fleetsu Faults API
  slug: fleetsu-faults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-faults-api-openapi.yml
- filename: fleetsu-fences-api-openapi.yml
  format: yaml
  label: Fleetsu Fences API
  slug: fleetsu-fences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-fences-api-openapi.yml
- filename: fleetsu-general-api-openapi.yml
  format: yaml
  label: Fleetsu General API
  slug: fleetsu-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-general-api-openapi.yml
- filename: fleetsu-groups-api-openapi.yml
  format: yaml
  label: Fleetsu Groups API
  slug: fleetsu-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-groups-api-openapi.yml
- filename: fleetsu-installs-api-openapi.yml
  format: yaml
  label: Fleetsu Installs API
  slug: fleetsu-installs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-installs-api-openapi.yml
- filename: fleetsu-kpi-api-openapi.yml
  format: yaml
  label: Fleetsu KPI API
  slug: fleetsu-kpi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-kpi-api-openapi.yml
- filename: fleetsu-logbooks-api-openapi.yml
  format: yaml
  label: Fleetsu Logbooks API
  slug: fleetsu-logbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-logbooks-api-openapi.yml
- filename: fleetsu-maps-api-openapi.yml
  format: yaml
  label: Fleetsu Maps API
  slug: fleetsu-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-maps-api-openapi.yml
- filename: fleetsu-reports-api-openapi.yml
  format: yaml
  label: Fleetsu Reports API
  slug: fleetsu-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-reports-api-openapi.yml
- filename: fleetsu-subscriptions-api-openapi.yml
  format: yaml
  label: Fleetsu Subscriptions API
  slug: fleetsu-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-subscriptions-api-openapi.yml
- filename: fleetsu-tags-api-openapi.yml
  format: yaml
  label: Fleetsu Tags API
  slug: fleetsu-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-tags-api-openapi.yml
- filename: fleetsu-trips-api-openapi.yml
  format: yaml
  label: Fleetsu Trips API
  slug: fleetsu-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-trips-api-openapi.yml
- filename: fleetsu-user-api-openapi.yml
  format: yaml
  label: Fleetsu User API
  slug: fleetsu-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-user-api-openapi.yml
- filename: fleetsu-users-api-openapi.yml
  format: yaml
  label: Fleetsu Users API
  slug: fleetsu-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/openapi/fleetsu-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fleetsu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fleetsu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fleetsu
provider_slug: fleetsu
scheme_count: 1
schemes:
- credential: Fleetsu platform username and password (user login credentials); no API keys or OAuth are documented.
  description: 'Docs (Postman collection description): "The Fleetsu API uses HTTP Basic Authentication use your Fleetsu username and password to authenticate." Example header: "Authorization: Basic OgXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=="'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fleetsu-openapi.yml
  - openapi/_original/fleetsu-postman-collection.json
  - https://api-docs.fleetsu.com/
  transport: All API Requests must be made over HTTPS
  type: http
  unauthenticated_response: Unauthenticated requests will fail with a 401 Unauthorized HTTP Response
slug: fleetsu-authentication
source_filename: fleetsu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://api-docs.fleetsu.com/\ndocs: https://api-docs.fleetsu.com/\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Docs (Postman collection description): \"The Fleetsu API uses HTTP Basic Authentication use your Fleetsu username and password to authenticate.\" Example header: \"Authorization: Basic OgXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX==\"'\n  credential: Fleetsu platform username and password (user login credentials); no API keys or OAuth are documented.\n  unauthenticated_response: 'Unauthenticated requests will fail with a 401 Unauthorized HTTP Response'\n  transport: 'All API Requests must be made over HTTPS'\n  sources:\n  - openapi/fleetsu-openapi.yml\n  - openapi/_original/fleetsu-postman-collection.json\n  - https://api-docs.fleetsu.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fleetsu/refs/heads/main/authentication/fleetsu-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Fleet Management
- Telematics
- GPS Tracking
- Connected Vehicles
- Logistics
- Driver Safety
- Australia
---
