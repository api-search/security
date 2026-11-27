---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cachethq-cachet-api-openapi.yml
  format: yaml
  label: Cachet Cachet API
  slug: cachethq-cachet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-cachet-api-openapi.yml
- filename: cachethq-component-groups-api-openapi.yml
  format: yaml
  label: Cachet Component Groups API
  slug: cachethq-component-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-component-groups-api-openapi.yml
- filename: cachethq-components-api-openapi.yml
  format: yaml
  label: Cachet Components API
  slug: cachethq-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-components-api-openapi.yml
- filename: cachethq-incident-templates-api-openapi.yml
  format: yaml
  label: Cachet Incident Templates API
  slug: cachethq-incident-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-incident-templates-api-openapi.yml
- filename: cachethq-incident-updates-api-openapi.yml
  format: yaml
  label: Cachet Incident Updates API
  slug: cachethq-incident-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-incident-updates-api-openapi.yml
- filename: cachethq-incidents-api-openapi.yml
  format: yaml
  label: Cachet Incidents API
  slug: cachethq-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-incidents-api-openapi.yml
- filename: cachethq-metric-points-api-openapi.yml
  format: yaml
  label: Cachet Metric Points API
  slug: cachethq-metric-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-metric-points-api-openapi.yml
- filename: cachethq-metrics-api-openapi.yml
  format: yaml
  label: Cachet Metrics API
  slug: cachethq-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-metrics-api-openapi.yml
- filename: cachethq-schedule-updates-api-openapi.yml
  format: yaml
  label: Cachet Schedule Updates API
  slug: cachethq-schedule-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-schedule-updates-api-openapi.yml
- filename: cachethq-schedules-api-openapi.yml
  format: yaml
  label: Cachet Schedules API
  slug: cachethq-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-schedules-api-openapi.yml
- filename: cachethq-subscribers-api-openapi.yml
  format: yaml
  label: Cachet Subscribers API
  slug: cachethq-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-subscribers-api-openapi.yml
auth_types: []
description: Authentication schemes for Cachet API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cachet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cachet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cachet
provider_slug: cachethq
scheme_count: 1
schemes:
- evidence: An API key is a bearer token sent in the Authorization header.
  header: Authorization
  how_to_obtain: Create an API key in the Cachet dashboard under Settings → Manage API Keys.
  location: header
  name: Bearer
  type: http-bearer
slug: cachethq-authentication
source_filename: cachethq-authentication.yml
source_heading: Authentication Profile
source_url: https://cachethq.io/docs/api-reference/authentication
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cachethq.io/docs/api-reference/authentication\nsources:\n- https://cachethq.io/docs/api-reference/authentication\n- https://cachethq.io/docs/v3.x/configuration/api-keys\ndescription: Authentication schemes for Cachet API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: An API key is a bearer token sent in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Cachet dashboard under Settings → Manage API Keys.\ndocs: https://cachethq.io/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/cachethq/authentication/cachethq-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Open Source
- Status Pages
- Incident Management
- Monitoring
---
