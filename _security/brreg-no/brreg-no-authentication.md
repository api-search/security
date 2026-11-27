---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brreg-no-enheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Enheter API
  slug: brreg-no-enheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-enheter-api-openapi.yml
- filename: brreg-no-frivillighetsregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Frivillighetsregisteret API
  slug: brreg-no-frivillighetsregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-frivillighetsregisteret-api-openapi.yml
- filename: brreg-no-generelt-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Generelt API
  slug: brreg-no-generelt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-generelt-api-openapi.yml
- filename: brreg-no-kommuner-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Kommuner API
  slug: brreg-no-kommuner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-kommuner-api-openapi.yml
- filename: brreg-no-kopi-av-rsregnskap-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Kopi av årsregnskap API
  slug: brreg-no-kopi-av-rsregnskap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-kopi-av-rsregnskap-api-openapi.yml
- filename: brreg-no-matrikkelenheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Matrikkelenheter API
  slug: brreg-no-matrikkelenheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-matrikkelenheter-api-openapi.yml
- filename: brreg-no-mellombalanse-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Mellombalanse API
  slug: brreg-no-mellombalanse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-mellombalanse-api-openapi.yml
- filename: brreg-no-oppdateringer-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Oppdateringer API
  slug: brreg-no-oppdateringer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-oppdateringer-api-openapi.yml
- filename: brreg-no-organisasjonsformer-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Organisasjonsformer API
  slug: brreg-no-organisasjonsformer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-organisasjonsformer-api-openapi.yml
- filename: brreg-no-partiregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Partiregisteret API
  slug: brreg-no-partiregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-partiregisteret-api-openapi.yml
- filename: brreg-no-regnskapsregisteret-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Regnskapsregisteret API
  slug: brreg-no-regnskapsregisteret-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-regnskapsregisteret-api-openapi.yml
- filename: brreg-no-roller-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Roller API
  slug: brreg-no-roller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-roller-api-openapi.yml
- filename: brreg-no-statistikk-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Statistikk API
  slug: brreg-no-statistikk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-statistikk-api-openapi.yml
- filename: brreg-no-underenheter-api-openapi.yml
  format: yaml
  label: Brønnøysundregistrene Underenheter API
  slug: brreg-no-underenheter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brreg-no/openapi/brreg-no-underenheter-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Brønnøysundregistrene Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brønnøysundregistrene secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brønnøysundregistrene
provider_slug: brreg-no
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/brreg-no-enhetsregisteret-openapi.yml
  type: http
slug: brreg-no-authentication
source_filename: brreg-no-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/brreg-no-enhetsregisteret-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/brreg-no-enhetsregisteret-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/brreg-no/authentication/brreg-no-authentication.yml
summary_line: http · 1 scheme
tags:
- Government
- Business Registry
- Open Data
- Norway
- Company Data
- Public Sector
- Financial Statements
---
