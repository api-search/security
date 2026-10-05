---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crowdwisdomtrading-account-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Account API
  slug: crowdwisdomtrading-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-account-api-openapi.yml
- filename: crowdwisdomtrading-health-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Health API
  slug: crowdwisdomtrading-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-health-api-openapi.yml
- filename: crowdwisdomtrading-signals-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Signals API
  slug: crowdwisdomtrading-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-signals-api-openapi.yml
- filename: crowdwisdomtrading-socialmap-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Socialmap API
  slug: crowdwisdomtrading-socialmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-socialmap-api-openapi.yml
- filename: crowdwisdomtrading-socialmap-preview-api-openapi.yml
  format: yaml
  label: CrowdWisdom Signals API Socialmap Preview API
  slug: crowdwisdomtrading-socialmap-preview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/openapi/crowdwisdomtrading-socialmap-preview-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crowdwisdomtrading Authentication
name_suffix: Authentication
oauth_flows: []
overview: CrowdWisdom Signals API secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CrowdWisdom Signals API
provider_slug: crowdwisdomtrading
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/crowdwisdomtrading-openapi.json
  type: http
slug: crowdwisdomtrading-authentication
source_filename: crowdwisdomtrading-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: derived\nsource: openapi/crowdwisdomtrading-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/crowdwisdomtrading-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdwisdomtrading/refs/heads/main/authentication/crowdwisdomtrading-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Trading
- Signals
- B2B
---
