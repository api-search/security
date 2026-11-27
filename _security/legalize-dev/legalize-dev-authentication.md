---
anonymous_access: false
api_key_in: []
api_specs:
- filename: legalize-dev-changes-api-openapi.yml
  format: yaml
  label: Legalize Changes API
  slug: legalize-dev-changes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-changes-api-openapi.yml
- filename: legalize-dev-countries-api-openapi.yml
  format: yaml
  label: Legalize Countries API
  slug: legalize-dev-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-countries-api-openapi.yml
- filename: legalize-dev-health-api-openapi.yml
  format: yaml
  label: Legalize Health API
  slug: legalize-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-health-api-openapi.yml
- filename: legalize-dev-jurisdictions-api-openapi.yml
  format: yaml
  label: Legalize Jurisdictions API
  slug: legalize-dev-jurisdictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-jurisdictions-api-openapi.yml
- filename: legalize-dev-law-types-api-openapi.yml
  format: yaml
  label: Legalize Law Types API
  slug: legalize-dev-law-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-law-types-api-openapi.yml
- filename: legalize-dev-laws-api-openapi.yml
  format: yaml
  label: Legalize Laws API
  slug: legalize-dev-laws-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-laws-api-openapi.yml
- filename: legalize-dev-stats-api-openapi.yml
  format: yaml
  label: Legalize Stats API
  slug: legalize-dev-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-stats-api-openapi.yml
- filename: legalize-dev-webhooks-api-openapi.yml
  format: yaml
  label: Legalize Webhooks API
  slug: legalize-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legalize-dev/openapi/legalize-dev-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Legalize
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Legalize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Legalize declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Legalize
provider_slug: legalize-dev
scheme_count: 1
schemes:
- evidence: Every request carries a Bearer token.
  header: Authorization
  how_to_obtain: Keys are created from the dashboard. They start with leg_.
  location: header
  name: Bearer
  type: http-bearer
slug: legalize-dev-authentication
source_filename: legalize-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://legalize.dev/docs/authentication
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://legalize.dev/docs/authentication\nsources:\n- https://legalize.dev/docs/authentication\n- https://legalize.dev/docs/quickstart\ndescription: Authentication schemes for Legalize\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every request carries a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are created from the dashboard. They start with leg_.\ndocs: https://legalize.dev/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/legalize-dev/authentication/legalize-dev-authentication.yml
summary_line: 1 scheme
tags:
- OpenLegislation
- Open Source
- Data
- Transparency
- Legal Tech
---
