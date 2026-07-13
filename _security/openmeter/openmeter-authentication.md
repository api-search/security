---
api_key_in: []
api_specs:
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Events Ingestion API
  slug: openmeter-events-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Meters API
  slug: openmeter-meters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Usage Query API
  slug: openmeter-usage-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Subjects API
  slug: openmeter-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Entitlements API
  slug: openmeter-entitlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Features API
  slug: openmeter-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Grants API
  slug: openmeter-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Notifications API
  slug: openmeter-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
- filename: openmeter-openapi.yml
  format: yaml
  label: OpenMeter Billing and Plans API
  slug: openmeter-billing-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/openapi/openmeter-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openmeter Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMeter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenMeter
provider_slug: openmeter
scheme_count: 1
schemes:
- description: OpenMeter Cloud API token supplied as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openmeter-openapi.yml
  type: http
slug: openmeter-authentication
source_filename: openmeter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openmeter-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OpenMeter Cloud API token supplied as a Bearer token.\n  sources:\n  - openapi/openmeter-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openmeter/refs/heads/main/authentication/openmeter-authentication.yml
summary_line: http · 1 scheme
tags:
- Usage Metering
- Billing
- Entitlements
- CloudEvents
- Open Source
- AI
---
