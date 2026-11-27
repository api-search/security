---
anonymous_access: false
api_key_in: []
api_specs:
- filename: suresms-authenticate-api-openapi.yml
  format: yaml
  label: SureSMS Authenticate API
  slug: suresms-authenticate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-authenticate-api-openapi.yml
- filename: suresms-coverage-api-openapi.yml
  format: yaml
  label: SureSMS Coverage API
  slug: suresms-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-coverage-api-openapi.yml
- filename: suresms-message-api-openapi.yml
  format: yaml
  label: SureSMS Message API
  slug: suresms-message-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-message-api-openapi.yml
- filename: suresms-messagestatus-api-openapi.yml
  format: yaml
  label: SureSMS Message Status API
  slug: suresms-messagestatus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-messagestatus-api-openapi.yml
- filename: suresms-price-api-openapi.yml
  format: yaml
  label: SureSMS Price API
  slug: suresms-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/suresms/openapi/suresms-price-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: SureSMS Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: SureSMS secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: SureSMS
provider_slug: suresms
scheme_count: 1
schemes:
- description: OAuth2 Password Grant
  flows:
  - flow: password
    scopes: 2
    tokenUrl: json/token
  name: oauth2
  sources:
  - openapi/suresms-openapi.json
  type: oauth2
slug: suresms-authentication
source_filename: suresms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/suresms-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: json/token\n    scopes: 2\n  description: OAuth2 Password Grant\n  sources:\n  - openapi/suresms-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/suresms/authentication/suresms-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- SMS Gateway
- Communications Platform
- Industry Solutions
- Integration Services
---
