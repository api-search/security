---
anonymous_access: false
api_key_in: []
api_specs:
- filename: knossot-org-credits-api-openapi.yml
  format: yaml
  label: Knossot Credits API
  slug: knossot-org-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-credits-api-openapi.yml
- filename: knossot-org-keys-api-openapi.yml
  format: yaml
  label: Knossot Keys API
  slug: knossot-org-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-keys-api-openapi.yml
- filename: knossot-org-knossot-agent-api-api-openapi.yml
  format: yaml
  label: Knossot Knossot Agent API
  slug: knossot-org-knossot-agent-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-knossot-agent-api-api-openapi.yml
- filename: knossot-org-recommendations-api-openapi.yml
  format: yaml
  label: Knossot Recommendations API
  slug: knossot-org-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-recommendations-api-openapi.yml
- filename: knossot-org-regions-api-openapi.yml
  format: yaml
  label: Knossot Regions API
  slug: knossot-org-regions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-regions-api-openapi.yml
- filename: knossot-org-usage-api-openapi.yml
  format: yaml
  label: Knossot Usage API
  slug: knossot-org-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knossot-org/openapi/knossot-org-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Knossot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knossot secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knossot
provider_slug: knossot-org
scheme_count: 1
schemes:
- description: kn_live_ key from the claim ceremony.
  name: bearer
  scheme: bearer
  sources:
  - openapi/knossot-org-openapi.json
  type: http
slug: knossot-org-authentication
source_filename: knossot-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/knossot-org-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: kn_live_ key from the claim ceremony.\n  sources:\n  - openapi/knossot-org-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/knossot-org/authentication/knossot-org-authentication.yml
summary_line: http · 1 scheme
tags:
- Community
- Event
- Calendar
- Hudson Valley
- Non-commercial
---
