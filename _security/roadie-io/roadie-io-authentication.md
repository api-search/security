---
api_key_in: []
api_specs:
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Catalog API
  slug: roadie-io-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Entity Push API
  slug: roadie-io-entity-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Scaffolder API
  slug: roadie-io-scaffolder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie Tech Insights API
  slug: roadie-io-tech-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
- filename: roadie-io-openapi.yml
  format: yaml
  label: Roadie TechDocs API
  slug: roadie-io-techdocs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/openapi/roadie-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Roadie Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Roadie secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Roadie
provider_slug: roadie-io
scheme_count: 1
schemes:
- description: 'Roadie API token passed as `Authorization: Bearer YOUR_ROADIE_API_TOKEN`. Two token types exist - User Tokens (tied to a person, created under Administration then Account then Roadie API Access; requires the "Roadie API Key Access" policy) and Service Tokens (unattached, for automation and CI/CD, created under Administration then Service Tokens). Both grant the same API access and are shown only once at creation. The public API is available on Cloud Hosted Roadie.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/roadie-io-openapi.yml
  - https://roadie.io/docs/api/authorization/
  type: http
slug: roadie-io-authentication
source_filename: roadie-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/roadie-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Roadie API token passed as `Authorization: Bearer YOUR_ROADIE_API_TOKEN`.\n    Two token types exist - User Tokens (tied to a person, created under\n    Administration then Account then Roadie API Access; requires the \"Roadie\n    API Key Access\" policy) and Service Tokens (unattached, for automation and\n    CI/CD, created under Administration then Service Tokens). Both grant the\n    same API access and are shown only once at creation. The public API is\n    available on Cloud Hosted Roadie.\n  sources:\n  - openapi/roadie-io-openapi.yml\n  - https://roadie.io/docs/api/authorization/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roadie-io/refs/heads/main/authentication/roadie-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Software Catalog
- Internal Developer Portal
- Backstage
- Developer Experience
- IDP
- Developer Portal
- Managed Backstage
- Scaffolder
- TechDocs
- Service Catalog
- Platform Engineering
---
