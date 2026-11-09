---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dregs-com-badge-rules-api-openapi.yml
  format: yaml
  label: Dregs Badge Rules API
  slug: dregs-com-badge-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-badge-rules-api-openapi.yml
- filename: dregs-com-channels-api-openapi.yml
  format: yaml
  label: Dregs Channels API
  slug: dregs-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-channels-api-openapi.yml
- filename: dregs-com-dashboard-api-openapi.yml
  format: yaml
  label: Dregs Dashboard API
  slug: dregs-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-dashboard-api-openapi.yml
- filename: dregs-com-datasets-api-openapi.yml
  format: yaml
  label: Dregs Datasets API
  slug: dregs-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-datasets-api-openapi.yml
- filename: dregs-com-devices-api-openapi.yml
  format: yaml
  label: Dregs Devices API
  slug: dregs-com-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-devices-api-openapi.yml
- filename: dregs-com-escalation-rules-api-openapi.yml
  format: yaml
  label: Dregs Escalation Rules API
  slug: dregs-com-escalation-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-escalation-rules-api-openapi.yml
- filename: dregs-com-escalations-api-openapi.yml
  format: yaml
  label: Dregs Escalations API
  slug: dregs-com-escalations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-escalations-api-openapi.yml
- filename: dregs-com-events-api-openapi.yml
  format: yaml
  label: Dregs Events API
  slug: dregs-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-events-api-openapi.yml
- filename: dregs-com-groups-api-openapi.yml
  format: yaml
  label: Dregs Groups API
  slug: dregs-com-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-groups-api-openapi.yml
- filename: dregs-com-identities-api-openapi.yml
  format: yaml
  label: Dregs Identities API
  slug: dregs-com-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-identities-api-openapi.yml
- filename: dregs-com-mappings-api-openapi.yml
  format: yaml
  label: Dregs Mappings API
  slug: dregs-com-mappings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dregs-com/openapi/dregs-com-mappings-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dregs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dregs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dregs
provider_slug: dregs-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer sk_your_secret_key'
  header: Authorization
  how_to_obtain: Create one in the Settings section of your dashboard
  location: header
  name: Bearer Token
  type: http-bearer
slug: dregs-com-authentication
source_filename: dregs-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dregs.com/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dregs.com/.well-known/oauth-protected-resource/mcp\nsources:\n- https://dregs.com/.well-known/oauth-protected-resource/mcp\n- https://dregs.com/manual/getting-started/\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'Authorization: Bearer sk_your_secret_key'\n  location: header\n  header: Authorization\n  how_to_obtain: Create one in the Settings section of your dashboard\ndocs: https://dregs.com/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/dregs-com/authentication/dregs-com-authentication.yml
summary_line: 1 scheme
tags:
- Fraud Prevention
- Abuse Prevention
- Identity Scoring
- Bot Detection
- Account Verification
---
