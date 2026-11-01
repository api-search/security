---
anonymous_access: false
api_key_in: []
api_specs:
- filename: etherfax-accounts-api-openapi.yml
  format: yaml
  label: etherFAX Accounts API
  slug: etherfax-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-accounts-api-openapi.yml
- filename: etherfax-devices-api-openapi.yml
  format: yaml
  label: etherFAX Devices API
  slug: etherfax-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-devices-api-openapi.yml
- filename: etherfax-inbox-api-openapi.yml
  format: yaml
  label: etherFAX Inbox API
  slug: etherfax-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-inbox-api-openapi.yml
- filename: etherfax-outbox-api-openapi.yml
  format: yaml
  label: etherFAX Outbox API
  slug: etherfax-outbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-outbox-api-openapi.yml
- filename: etherfax-routes-api-openapi.yml
  format: yaml
  label: etherFAX Routes API
  slug: etherfax-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-routes-api-openapi.yml
- filename: etherfax-status-api-openapi.yml
  format: yaml
  label: etherFAX Status API
  slug: etherfax-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etherfax/openapi/etherfax-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Etherfax Authentication
name_suffix: Authentication
oauth_flows: []
overview: etherFAX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: etherFAX
provider_slug: etherfax
scheme_count: 1
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/etherfax-rest-api-30-api-openapi.yml
  type: http
slug: etherfax-authentication
source_filename: etherfax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/etherfax-rest-api-30-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/etherfax-rest-api-30-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/etherfax/authentication/etherfax-authentication.yml
summary_line: http · 1 scheme
tags:
- Fax
- Cloud
- AI
- Secure
- DocumentAutomation
---
