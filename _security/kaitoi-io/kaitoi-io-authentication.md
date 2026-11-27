---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kaitoi-io-account-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Account API
  slug: kaitoi-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-account-api-openapi.yml
- filename: kaitoi-io-files-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Files API
  slug: kaitoi-io-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-files-api-openapi.yml
- filename: kaitoi-io-node-types-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Node Types API
  slug: kaitoi-io-node-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-node-types-api-openapi.yml
- filename: kaitoi-io-projects-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Projects API
  slug: kaitoi-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-projects-api-openapi.yml
- filename: kaitoi-io-runs-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Runs API
  slug: kaitoi-io-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-runs-api-openapi.yml
- filename: kaitoi-io-storyboards-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Storyboards API
  slug: kaitoi-io-storyboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-storyboards-api-openapi.yml
- filename: kaitoi-io-templates-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Templates API
  slug: kaitoi-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-templates-api-openapi.yml
- filename: kaitoi-io-timelines-api-openapi.yml
  format: yaml
  label: Kaitoi Labs Timelines API
  slug: kaitoi-io-timelines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaitoi-io/openapi/kaitoi-io-timelines-api-openapi.yml
auth_types: []
description: Authentication schemes for Kaitoi Labs REST API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kaitoi Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaitoi Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kaitoi Labs
provider_slug: kaitoi-io
scheme_count: 1
schemes:
- evidence: 'Public REST requests use an API key in Authorization: Bearer <key> .'
  header: Authorization
  how_to_obtain: Create keys through Settings → Developer → API Keys and grant only the scopes the integration needs.
  location: header
  name: API Key
  type: http-bearer
slug: kaitoi-io-authentication
source_filename: kaitoi-io-authentication.yml
source_heading: Authentication Profile
source_url: https://kaitoi.io/docs/core/authentication/
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kaitoi.io/docs/core/authentication/\nsources:\n- https://kaitoi.io/docs/core/authentication/\n- https://kaitoi.io/docs/core/authentication/\n- https://kaitoi.io/docs/core/quickstart/\n- https://kaitoi.io/docs/cli/local-models/\ndescription: Authentication schemes for Kaitoi Labs REST API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Public REST requests use an API key in Authorization: Bearer <key> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys through Settings → Developer → API Keys and grant only the scopes the integration needs.\ndocs: https://kaitoi.io/docs/core/authentication/\n"
source_yaml_url: https://artifacts.apis.io/kaitoi-io/authentication/kaitoi-io-authentication.yml
summary_line: 1 scheme
tags:
- AI production
- Creative Platform
- Studio workspace
- Core API
- Advertising tools
- Integration
---
