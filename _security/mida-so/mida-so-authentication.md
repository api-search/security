---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mida-so-account-api-openapi.yml
  format: yaml
  label: Mida Account API
  slug: mida-so-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-account-api-openapi.yml
- filename: mida-so-events-api-openapi.yml
  format: yaml
  label: Mida Events API
  slug: mida-so-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-events-api-openapi.yml
- filename: mida-so-exclusion-groups-api-openapi.yml
  format: yaml
  label: Mida Exclusion groups API
  slug: mida-so-exclusion-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-exclusion-groups-api-openapi.yml
- filename: mida-so-experiments-api-openapi.yml
  format: yaml
  label: Mida Experiments API
  slug: mida-so-experiments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-experiments-api-openapi.yml
- filename: mida-so-goals-api-openapi.yml
  format: yaml
  label: Mida Goals API
  slug: mida-so-goals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-goals-api-openapi.yml
- filename: mida-so-hypotheses-api-openapi.yml
  format: yaml
  label: Mida Hypotheses API
  slug: mida-so-hypotheses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-hypotheses-api-openapi.yml
- filename: mida-so-personalization-api-openapi.yml
  format: yaml
  label: Mida Personalization API
  slug: mida-so-personalization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-personalization-api-openapi.yml
- filename: mida-so-projects-api-openapi.yml
  format: yaml
  label: Mida Projects API
  slug: mida-so-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-projects-api-openapi.yml
- filename: mida-so-surveys-api-openapi.yml
  format: yaml
  label: Mida Surveys API
  slug: mida-so-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mida-so/openapi/mida-so-surveys-api-openapi.yml
auth_types: []
description: Authentication for Mida API is performed by passing the API key either as a Bearer token in the Authorization header or as an API‑key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mida Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mida declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mida
provider_slug: mida-so
scheme_count: 2
schemes:
- evidence: 'Pass your API key in one of these ways (all are equivalent): # Recommended Authorization: Bearer YOUR_GENERATED_API_KEY # Alternatives x-api-key: YOUR_GENERATED_API_KEY api-key: YOUR_GENERATED_API_KEY'
  header: Authorization
  how_to_obtain: Generate an API key in the dashboard at app.mida.so/api-keys.
  location: header
  name: Authorization Bearer
  type: http-bearer
- evidence: 'Pass your API key in one of these ways (all are equivalent): # Recommended Authorization: Bearer YOUR_GENERATED_API_KEY # Alternatives x-api-key: YOUR_GENERATED_API_KEY api-key: YOUR_GENERATED_API_KEY'
  header: x-api-key
  how_to_obtain: Generate an API key in the dashboard at app.mida.so/api-keys.
  location: header
  name: x-api-key / api-key
  type: apiKey
slug: mida-so-authentication
source_filename: mida-so-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mida.so/docs/quickstart
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mida.so/docs/quickstart\nsources:\n- https://docs.mida.so/docs/quickstart\n- https://docs.mida.so/docs/server-side/quickstart\n- https://docs.mida.so/docs/intro\n- https://help.mida.so/en/collections/17771935-getting-started\ndescription: Authentication for Mida API is performed by passing the API key either as a Bearer token in the Authorization header or as an API‑key\n  header.\nschemes:\n- type: http-bearer\n  name: Authorization Bearer\n  evidence: 'Pass your API key in one of these ways (all are equivalent): # Recommended Authorization: Bearer YOUR_GENERATED_API_KEY # Alternatives\n    x-api-key: YOUR_GENERATED_API_KEY api-key: YOUR_GENERATED_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the dashboard at app.mida.so/api-keys.\n- type: apiKey\n  name: x-api-key / api-key\n  evidence: 'Pass your API key in one of\
  \ these ways (all are equivalent): # Recommended Authorization: Bearer YOUR_GENERATED_API_KEY # Alternatives\n    x-api-key: YOUR_GENERATED_API_KEY api-key: YOUR_GENERATED_API_KEY'\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate an API key in the dashboard at app.mida.so/api-keys.\nnote: Both header names (x-api-key and api-key) are accepted; the documentation lists them as alternatives.\ndocs: https://docs.mida.so/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/mida-so/authentication/mida-so-authentication.yml
summary_line: 2 schemes
tags:
- A/B Testing
- Artificial Intelligence
- Marketing
- Analytics
- Software-as-a-Service
- Platform
---
