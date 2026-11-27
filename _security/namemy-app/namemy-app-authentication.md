---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: namemy-app-brand-conflict-api-openapi.yml
  format: yaml
  label: Namemy Brand Conflict API
  slug: namemy-app-brand-conflict-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-brand-conflict-api-openapi.yml
- filename: namemy-app-brand-kits-api-openapi.yml
  format: yaml
  label: Namemy Brand Kits API
  slug: namemy-app-brand-kits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-brand-kits-api-openapi.yml
- filename: namemy-app-domains-api-openapi.yml
  format: yaml
  label: Namemy Domains API
  slug: namemy-app-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-domains-api-openapi.yml
- filename: namemy-app-keys-api-openapi.yml
  format: yaml
  label: Namemy Keys API
  slug: namemy-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-keys-api-openapi.yml
- filename: namemy-app-landing-pages-api-openapi.yml
  format: yaml
  label: Namemy Landing Pages API
  slug: namemy-app-landing-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-landing-pages-api-openapi.yml
- filename: namemy-app-legal-api-openapi.yml
  format: yaml
  label: Namemy Legal API
  slug: namemy-app-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-legal-api-openapi.yml
- filename: namemy-app-logos-api-openapi.yml
  format: yaml
  label: Namemy Logos API
  slug: namemy-app-logos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-logos-api-openapi.yml
- filename: namemy-app-names-api-openapi.yml
  format: yaml
  label: Namemy Names API
  slug: namemy-app-names-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-names-api-openapi.yml
- filename: namemy-app-public-api-openapi.yml
  format: yaml
  label: Namemy Public API
  slug: namemy-app-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namemy-app/openapi/namemy-app-public-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Namemy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Namemy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Namemy
provider_slug: namemy-app
scheme_count: 2
schemes:
- bearerFormat: nma_live_
  description: API key prefixed with `nma_live_`
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/namemy-app-openapi.yml
  type: http
- description: Session cookie from namemy.app dashboard login
  in: cookie
  name: sessionAuth
  parameter: next-auth.session-token
  sources:
  - openapi/namemy-app-openapi.yml
  type: apiKey
slug: namemy-app-authentication
source_filename: namemy-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/namemy-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: nma_live_\n  description: API key prefixed with `nma_live_`\n  sources:\n  - openapi/namemy-app-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: next-auth.session-token\n  description: Session cookie from namemy.app dashboard login\n  sources:\n  - openapi/namemy-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/namemy-app/authentication/namemy-app-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Naming
- Domain
- Software-as-a-Service
---
