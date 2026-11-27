---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: desenmascara-me-domain-check-api-openapi.yml
  format: yaml
  label: Desenmascara.me Domain Check API
  slug: desenmascara-me-domain-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desenmascara-me/openapi/desenmascara-me-domain-check-api-openapi.yml
- filename: desenmascara-me-fraud-feed-api-openapi.yml
  format: yaml
  label: Desenmascara.me Fraud Feed API
  slug: desenmascara-me-fraud-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desenmascara-me/openapi/desenmascara-me-fraud-feed-api-openapi.yml
- filename: desenmascara-me-public-api-openapi.yml
  format: yaml
  label: Desenmascara.me Public API
  slug: desenmascara-me-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desenmascara-me/openapi/desenmascara-me-public-api-openapi.yml
- filename: desenmascara-me-search-api-openapi.yml
  format: yaml
  label: Desenmascara.me Search API
  slug: desenmascara-me-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desenmascara-me/openapi/desenmascara-me-search-api-openapi.yml
- filename: desenmascara-me-threat-intel-api-openapi.yml
  format: yaml
  label: Desenmascara.me Threat Intel API
  slug: desenmascara-me-threat-intel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/desenmascara-me/openapi/desenmascara-me-threat-intel-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Desenmascara.me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Desenmascara.me secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Desenmascara.me
provider_slug: desenmascara-me
scheme_count: 1
schemes:
- description: 'API key from your dashboard (format: `dm_...`).'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/desenmascara-me-openapi.yaml
  type: apiKey
slug: desenmascara-me-authentication
source_filename: desenmascara-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/desenmascara-me-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key from your dashboard (format: `dm_...`).'\n  sources:\n  - openapi/desenmascara-me-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/desenmascara-me/authentication/desenmascara-me-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fraud Prevention
- Scam Prevention
- Security
- Risk Intelligence
---
