---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openwaters-io-authentication-api-openapi.yml
  format: yaml
  label: Open Waters Authentication API
  slug: openwaters-io-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-authentication-api-openapi.yml
- filename: openwaters-io-contributing-api-openapi.yml
  format: yaml
  label: Open Waters Contributing API
  slug: openwaters-io-contributing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-contributing-api-openapi.yml
- filename: openwaters-io-currents-api-openapi.yml
  format: yaml
  label: Open Waters Currents API
  slug: openwaters-io-currents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-currents-api-openapi.yml
- filename: openwaters-io-stations-api-openapi.yml
  format: yaml
  label: Open Waters Stations API
  slug: openwaters-io-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-stations-api-openapi.yml
- filename: openwaters-io-status-api-openapi.yml
  format: yaml
  label: Open Waters Status API
  slug: openwaters-io-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-status-api-openapi.yml
- filename: openwaters-io-tides-api-openapi.yml
  format: yaml
  label: Open Waters Tides API
  slug: openwaters-io-tides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-tides-api-openapi.yml
- filename: openwaters-io-vessels-api-openapi.yml
  format: yaml
  label: Open Waters Vessels API
  slug: openwaters-io-vessels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openwaters-io/openapi/openwaters-io-vessels-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Open Waters Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open Waters secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Open Waters
provider_slug: openwaters-io
scheme_count: 1
schemes:
- description: 'An aiscast claim token (`ak1....`), created by `POST /v1/keys` or issued by the operator. Besides `Authorization: Bearer`, the token is accepted as an HTTP Basic password (`anything:<token>`, which is what AIS-catcher''s USERPWD sends) or as `?key=<token>` on the URL. A token that is present but invalid, expired, revoked, used outside its `cidr`, or lacking the role for the action is refused; it ne'
  name: token
  scheme: bearer
  sources:
  - openapi/ais-openapi.json
  type: http
slug: openwaters-io-authentication
source_filename: openwaters-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/ais-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: 'An aiscast claim token (`ak1....`), created by `POST /v1/keys` or issued by\n    the operator. Besides `Authorization: Bearer`, the token is accepted as an HTTP Basic password\n    (`anything:<token>`, which is what AIS-catcher''s USERPWD sends) or as `?key=<token>` on\n    the URL. A token that is present but invalid, expired, revoked, used outside its `cidr`,\n    or lacking the role for the action is refused; it ne'\n  sources:\n  - openapi/ais-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/openwaters-io/authentication/openwaters-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Marine
- Open Source
- Data
- Navigation
---
