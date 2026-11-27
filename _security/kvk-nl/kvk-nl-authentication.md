---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kvk-nl-abonnement-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Abonnement API
  slug: kvk-nl-abonnement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-abonnement-api-openapi.yml
- filename: kvk-nl-basisprofiel-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Basisprofiel API
  slug: kvk-nl-basisprofiel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-basisprofiel-api-openapi.yml
- filename: kvk-nl-naamgeving-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Naamgeving API
  slug: kvk-nl-naamgeving-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-naamgeving-api-openapi.yml
- filename: kvk-nl-signaal-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Signaal API
  slug: kvk-nl-signaal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-signaal-api-openapi.yml
- filename: kvk-nl-vestigingsprofiel-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Vestigingsprofiel API
  slug: kvk-nl-vestigingsprofiel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-vestigingsprofiel-api-openapi.yml
- filename: kvk-nl-zoeken-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Zoeken API
  slug: kvk-nl-zoeken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-zoeken-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kamer van Koophandel (KVK) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kamer van Koophandel (KVK) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kamer van Koophandel (KVK)
provider_slug: kvk-nl
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/kvk-nl-mutatieservice-openapi.yml
  type: apiKey
slug: kvk-nl-authentication
source_filename: kvk-nl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/kvk-nl-mutatieservice-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/kvk-nl-mutatieservice-openapi.yml\ncredential_issuance:\n  location: My Developer Portal (https://developers.kvk.nl/login), after applying at https://developers.kvk.nl/apply-for-apis\n  self_serve: false\n  requires: [user account, API key, paid API subscription]\n  note: >-\n    Real Handelsregister data needs a user account and an API key (\"To use the APIs you need a user account and an API key\",\n    developers.kvk.nl/documentation/quickstart) under a paid API subscription (EUR 6.40/month plus per-call fees for\n    Basisprofiel, Vestigingsprofiel and Naamgeving, developers.kvk.nl/pricing). The published shared test key reaches the\n    test environment only, which serves a small set of fictitious companies.\nenvironments:\n\
  - name: test\n  base_url: https://api.kvk.nl/test/api\n  purpose: Free test environment with a small set of fictitious data; no registration needed.\n  self_service: true\n  credential: shared test API key published on https://developers.kvk.nl/documentation/testing (apikey header)\n  real_data: false\n- name: production\n  base_url: https://api.kvk.nl/api\n  purpose: Live Handelsregister data.\n  self_service: false\n  credential: personal API key issued with a paid API subscription\n  real_data: true\nx-evidence:\n  checked: '2026-11-11'\n  probes:\n  - {url: 'https://developers.kvk.nl/documentation/testing', status: 200, reading: 'test environment, \"a small set of fictitious data\", no registration; publishes the shared test key'}\n  - {url: 'https://developers.kvk.nl/documentation/quickstart', status: 200, reading: 'production needs a user account and an API key'}\n  - {url: 'https://developers.kvk.nl/pricing', status: 200, reading: 'API subscription required, EUR 6.40/month plus\
  \ per-call fees'}\n  - {url: 'https://api.kvk.nl/test/api/v2/zoeken?naam=test', status: 200, reading: 'JSON with the published test key'}\n  - {url: 'https://api.kvk.nl/api/v2/zoeken?naam=test', status: 401, reading: 'refused with the published test key and with no key'}\n"
source_yaml_url: https://artifacts.apis.io/kvk-nl/authentication/kvk-nl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Business Register
- Government
- Netherlands
- Company Data
- KYC
- Open Data
---
